Evo test caseova za Word dokument:

KONFIDAT — Test scenariji

TC-01: Pokretanje aplikacije
Scenarij: Korisnik otvara aplikaciju u browseru.
Očekivani rezultat: Aplikacija se učitava, prikazuje se početna stranica sa svim modulima.
Status: ✅ Može se testirati
Rezultat: Prolazi

TC-02: THOR autentikacija
Scenarij: Korisnik se prijavljuje u aplikaciju putem PBZ THOR sustava.
Očekivani rezultat: Korisnik se uspješno autenticira i preusmjerava na početnu stranicu.
Status: 🔴 Blokirano
Bloker: Korisnik kkovacevic2 još nije dodan u THOR dev okolinu za aplikaciju A121. Čekamo PBZ tim da dodaju korisnika.

TC-03: Pregled radnih stanica
Scenarij: Prijavljeni korisnik otvara modul Radne stanice, primjenjuje filtre po statusu i organizacijskom dijelu.
Očekivani rezultat: Lista radnih stanica se prikazuje filtrirano prema odabranim parametrima.
Status: 🔴 Blokirano
Bloker: Ovisi o TC-02 — bez autentikacije ne možemo pristupiti modulu.

TC-04: Konfiguracije poslovnica
Scenarij: Korisnik otvara modul Konfiguracije poslovnica i pregledava podatke.
Očekivani rezultat: Podaci se učitavaju ispravno iz Oracle baze.
Status: 🔴 Blokirano
Bloker: Ovisi o TC-02.

TC-05: Oracle DB konekcija
Scenarij: Aplikacija se spaja na Oracle DEV bazu i dohvaća podatke.
Očekivani rezultat: Podaci se prikazuju bez grešaka.
Status: ✅ Može se testirati
Rezultat: Konekcija radi, podaci se dohvaćaju.

TC-06: Povijest verzija
Scenarij: Korisnik pregledava povijest verzija za određeni zapis.
Očekivani rezultat: Prikazuju se sve verzije kronološkim redom.
Status: 🔴 Blokirano
Bloker: Ovisi o TC-02.

TC-07: Podatkovni skupovi — KUM brojevi
Scenarij: Korisnik pretražuje podatkovne skupove po KUM broju.
Očekivani rezultat: Rezultati pretrage se prikazuju ispravno.
Status: 🔴 Blokirano
Bloker: Ovisi o TC-02.

Ovo su osnovni scenariji — možeš ih proširiti s detaljnijim koracima za svaki. Treba li u Word formatu?

daj mi prompt koji ce sve ovo rijesiti kada ga dam u chat gdje smo developali i radili na migraciji

Evo prompta:

Please generate a comprehensive test case document for the Konfidat application in Croatian language.

Look through the entire codebase — all controllers in src/WebService/, services in src/App/Service/, Twig templates in templates/, and the legacy code in legacy/ — and create test cases for every feature and module you find.

For each test case include:

Test case ID (TC-01, TC-02, etc.)
Module name
Test scenario description (what the user does)
Pre-conditions (what needs to be set up before testing)
Step by step test steps
Expected result
Status: ✅ Can be tested OR 🔴 Blocked
If blocked: explain exactly what the blocker is and what needs to happen to unblock it

Known blockers to reference:

THOR authentication: user kkovacevic2 needs to be added to THOR dev environment for application A121 before any authenticated features can be tested
Any features requiring specific Oracle data or stored procedures should note this

Format the output as a structured markdown document that can be easily copied into Word.

Start by listing all modules/features you found in the codebase, then generate the test cases.

Paste ovo u Cursor chat u projektu i on će proći kroz cijeli kod i generirati sve test caseove.
