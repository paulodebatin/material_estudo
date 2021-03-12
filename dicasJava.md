# Gerar uma chave Random
System.out.println(new SimpleDateFormat("yyyyMMddHHmmss").format(new Date()) + "-"  + UUID.randomUUID() );
