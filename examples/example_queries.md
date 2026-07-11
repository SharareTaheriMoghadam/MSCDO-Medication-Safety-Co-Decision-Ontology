# Example SPARQL Queries

## Retrieve medications associated with adverse drug events

```sparql
SELECT ?medication ?event
WHERE {
  ?medication msdo:associatedWith ?event .
}
```

---

## Retrieve medication errors

```sparql
SELECT ?error
WHERE {
  ?error rdf:type msdo:MedicationError .
}
```

---

## Retrieve patients requiring enhanced monitoring

```sparql
SELECT ?patient
WHERE {
  ?patient rdf:type msdo:RequiresEnhancedMonitoring .
}
```
