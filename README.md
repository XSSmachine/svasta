You are helping migrate a legacy PHP application called Konfidat to Symfony 7.2 with PHP 8.3. The legacy code is in the legacy/ folder and the new Symfony application is in backend/.
Your task:
Analyze the legacy PHP code in legacy/ — identify all modules, features, database queries, and business logic
Pick the single simplest self-contained feature (e.g. a list view or simple form) and migrate it to Symfony 7
Follow the architecture from the backend development guide: thin controllers in src/WebService/, business logic in src/App/Service/, entities in src/App/Entity/
Use PHP 8.3 features: constructor property promotion, readonly, attributes, enums
Use Doctrine attributes for entity mapping
The database is Oracle — keep existing SQL compatible
Create a route, controller, service, and Twig template for the migrated feature
Do not touch legacy/, public/, or any generated files
Start by listing what modules/features exist in legacy/ and recommend which one to migrate first based on simplicity.
