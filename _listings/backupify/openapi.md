swagger: "2.0"
x-collection-name: Backupify
x-complete: 1
info:
  title: Backupify
  description: the-backupify-api-allows-you-to-integrate-the-leading-saas-backup-solution-into-your-software-making-it-easy-to-give-your-customers-the-data-protection-they-need--
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/backup_instances/{backup_instance_id}/exports:
    get:
      summary: Retrieve a list of exports for the specified backup_instance
      description: You can only retrieve exports for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceExports
      x-api-path-slug: v1backup-instancesbackup-instance-idexports-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve exports for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
    post:
      summary: Perform an export of the most recent backup of the specified backup_instance
      description: Perform an export of the most recent backup of the specified backup_instance.
      operationId: postV1BackupInstancesBackupInstanceExports
      x-api-path-slug: v1backup-instancesbackup-instance-idexports-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to export
      - in: formData
        name: export_run[backup_run_id]
        description: ID of a specific backup_run to export
      - in: formData
        name: export_run[content_types]
        description: Comma separated list of blob content-types to export
      - in: formData
        name: export_run[export_datetime]
        description: 'Date (format: YYYY-MM-DD) from which to export'
      - in: formData
        name: export_run[export_formats]
        description: Comma separated list of export format options
      - in: formData
        name: export_run[force_full]
        description: Flag to force a full export, as opposed to re-authorizing an
          old export if the data is the same
      - in: formData
        name: export_run[send_confirmation]
        description: Flag to send a confirmation email w/export link upon completion
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
  /v1/backup_instances/{backup_instance_id}/exports/{export_id}:
    get:
      summary: Retrieve a specific export for the specified backup_instance
      description: You can only retrieve exports for backup_instances you have access
        to
      operationId: getV1BackupInstancesBackupInstanceExportsExport
      x-api-path-slug: v1backup-instancesbackup-instance-idexportsexport-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an export for
      - in: path
        name: export_id
        description: ID of the export to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
      - Export
      - Id
  /v1/backup_instances/{backup_instance_id}/exports/{export_id}/reauth:
    post:
      summary: Retrieve an updated exported_data_url for a specific export for the
        specified backup_instance
      description: Retrieve an updated exported_data_url for a specific export for
        the specified backup_instance.
      operationId: postV1BackupInstancesBackupInstanceExportsExportReauth
      x-api-path-slug: v1backup-instancesbackup-instance-idexportsexport-idreauth-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an export for
      - in: path
        name: export_id
        description: ID of the export to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Exports
      - Export
      - Id
      - Reauth