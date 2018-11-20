# Snowflake

Snowflake是k次序唯一64位整数的来源。

这是一个用于在非协调设置中生成ID的Java库:

    int node = 1;
    Snowflake s = new Snowflake(node);
    long id = s.next();

节点id是手动分配的值，介于0和1023之间
  用于在多节点群集中使用时区分不同的Snowflake.

要将其作为库包含，您可以使用以下Maven依赖项:

    <dependency>
        <groupId>com.relops</groupId>
        <artifactId>snowflake</artifactId>
        <version>1.1</version>
    </dependency>
