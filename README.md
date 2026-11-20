# Piletirakenduse backend

Ehitan selle rakenduse koolitöö raames. Rakendus on loodud Node.js ja Express raamistikus ning selle eesmärk on pakkuda kasutajatele võimalust hallata erinevaid sündmusi, sealhulgas registreeruda, vaadata sündmuste ajakava ja saada teavitusi.

Issued tehakse järjekorras ja iga hilisem sõltub varasematest.

**Alusta siit: [ALUSTA.md](ALUSTA.md)**

> [!IMPORTANT]
> Pane tähele, mida meil selle projekti jaoks vaja läheb ning valmista oma arenduskeskkond vastavalt sellele. Nimekirjas on Docker, NodeJS versioonid ja palju muud.

**Käsud**

#1: node -v

#2: npm init -y

#3: npm install express

#4: npm install -D typescript tsx @types/node @types/express

#5: npm run typecheck

#6: npm run server

#7: npm install -D prettier oxlint

#8: npx oxlint --init

#9: npm run format

#10: npm run lint

#11: npm run format:check

#12: docker --version

#13: docker compose version

#14: docker compose up -d

#15: npm install zod

#16: npm install drizzle-orm pg

#17: npm install -D drizzle-kit @types/pg

#18: npm run auth:generate

#19: npm run db:generate -- --name=create_auth_tables  

#20: npm run db:migrate

// kui auth.ts seadistus muutub, korda auth:generate → db:generate → db:migrate

---

**Seadistus**

DATABASE_USER=
DATABASE_PASSWORD=
DATABASE_NAME=
PORT=
NODE_ENV=
DATABASE_URL=

---
Kood on kaustades domeeni kaupa, mitte kihi kaupa. Kõik ürituse failid on koos, mitte "kõik controllerid ühes kaustas":

![alt text](images/image.png)

![alt text](images/image-1.png)

![alt text](images/image-2.png)
