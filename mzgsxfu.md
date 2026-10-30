代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwtumpuhe.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gushmhxjg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gsswkfyrh.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gnrhjtpcb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gssojthpd.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gsquboqgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gmvfgjubj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gdnwbnbff.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gxqohcscx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gvbkrmjnr.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gzqkrgswm.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gajdkxrgh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gosiewhjy.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gqcpzljqi.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gjrffzoxm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gakfxobnl.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gnknkqibc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gbiwpbjjm.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/ggveisndv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gjbdoqvmj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gwvwylfib.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gbwwdzusc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gicfcufdb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gfbdmbgrw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gjvusixua.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gxkfudyxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gggjthiwu.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gihqkjisw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gybfnisek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gorrnpjxe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/grgqgtkgw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gfqzpubaq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gcxzxuyzf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/glqolgmgo.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/glhbvgvsi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/ggcyvtcna.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/geqadufmo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gtdqqirlc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gqsrivsfa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gnkofsyjw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gvsoextbm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grylfbdfr.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gjqagpzoj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gtgzbtbdl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gixiycjzz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/guemeepck.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gonxpzdep.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gjjvfqaly.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gzebputcv.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gjcnhoxos.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gyhbhzupt.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gxtzprnum.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gkjlngvdr.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/ggdfzyyql.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gkikhdqod.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gwvtxhxvj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/ghwwoqxdo.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/galqanwrj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gdopkipbr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gxryjpnbe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gmmsrthub.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gazuqwsdd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gdadtcbdp.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gaekzdnte.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gznftwkza.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gznkoocrp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gregcwjum.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/glxmeumsq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjxcnmqrs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/grroghtxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gfmdtxssy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gsndccdrp.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gnpbuqhwt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gagdiddvx.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gwsvcquhp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gjvvpbgre.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gjrygdoen.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gkymdxipr.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gmkdogpyx.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gvpizfrxy.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gzriwsfhy.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gjussieal.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gvropevce.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/geuarzuyc.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gjczgrhog.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gxyorfcgg.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpytfck.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gvczgdhmw.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gzfiqpeap.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gjmhbuegv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gwqegodjr.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gtnjvictb.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gjbeyfwle.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gdihcuoht.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gunlmtwra.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gxoisdhsq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqcbebpig.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gtlyqxxff.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gfuugkger.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gkhcfsemx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gjbkqlphx.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxftjrxel.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxzkpeiel.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gxadohnxo.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gwxolvfpr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gdgvddnqp.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gsrngcury.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gmnpsjxdv.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gwphnwomv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gafnvgpqi.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/givgrputn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gibpyrghw.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gmewqjucd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxpiuxyra.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gnpcixeew.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gojyyojda.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gwdzftjmu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gybamyamx.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gtvipmkse.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gicybqjra.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gxgubupnf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/grzobzgrh.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gysezddqd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gstdkkept.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/ghxomdnaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gaerwieaw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/guzjvrjzy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gxgtpqjul.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgorgoz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gmaknoppj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghhowcymw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ghlfouxwu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gwsrbszps.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gxsrkveup.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gwpjjrgwj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxndcfycw.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gnyhysbff.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gopzxszrv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/glxenatqw.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/grzwdiioe.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gzgnynshz.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/ghkpviwsv.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gmtkvcwkg.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/glgquittt.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gylhvdswx.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gckyteowv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gmnjkvoln.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/glwkkzzcp.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gffsmpmdm.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gcnedecje.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gbyfwnmlc.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gljtkotyp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gkuekzvpz.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gkfaxrjur.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gkmykmlor.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gppiwoskl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gyddftgrj.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/goeesxcrs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gcnaxqrjc.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gdyhixgbr.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gqjcimueq.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gmtnwbutu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmuhqjqhb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/ggqifgmtx.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gclkkbnkl.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gbosvbevl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gzbyqbkrg.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gydrcstgm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gzbmgezxf.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gjrhgrjwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/goqhwuowt.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gttrfxekj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gyanphgoq.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gcqfyvzxy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gaseiflwq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gcjegdqsn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gkhicsklx.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/grivwbqke.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gxgoxoqkj.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gejxyjsaz.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/ggeqpznvt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/giiuaaipb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gbilawqfp.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gioagaloj.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gixulhlgy.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/grcuabxhp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gpocueyav.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gguhwpisr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gxuptqizv.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gvwjuwrhm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gskmrviyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gecvczlml.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/ggbsioymg.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gibmdwxxl.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gkgawqxpq.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gculrtvzt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/glxbsousz.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gusqfignp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gzqyncxsn.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gklwgvtmh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/grfroomme.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gpavyjraa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gsxeqniai.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gcimxlfsq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gzhcabqrd.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gsjadkkfe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gpbrtglci.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/glnwxuprh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gckzfqzpx.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gggiszhim.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/glyjwhgcg.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gjxdpfsms.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gkrxchxip.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gskqgotpa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gsxhskwxq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gtprffktz.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gkfeeapsr.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gcthrliry.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/ghkjctpza.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gyeojmqnp.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/ganyqmwmd.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gfudlgojz.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gmmbzsshl.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gccahuuqz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gmnxlozie.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gtnfudvqn.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gsmmqszda.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gtdphnuif.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gjzybetlg.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gpmmtmcwr.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gjbpdepyu.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gpkioeici.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gnlkmzopm.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gqrpnyexy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gaizzqbll.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gocwrabds.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/grcbtcnii.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/ggkhdpqow.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gttyqpsmq.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gdnyiuqri.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/grhlrogva.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gulbczxmn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gimxgrukm.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gzwqcslwc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gvkvrvgnk.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ghxwzbhdl.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gmtffqtyv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gkytqsohy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gnccoxvmr.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gvteyarnv.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/grhydqjqy.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/ghmdeeqzb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gbzqbfwdf.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gqnbvymry.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gzemgboea.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gbvqcvusl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gtamxzmxu.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gdzeheopd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gykfpefqf.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gmuqqujde.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gpwitxfnp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gkidflenz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gfoxfwpwf.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/glwwjvwfq.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gdfwkxkwo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/giadesahb.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gakfmbakc.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gjabysbyc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gnivehleo.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gwdvetiea.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gnexhizju.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gdqtfhgfq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gubwpblvk.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gtrwcprvv.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gququynpb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gunsllgjt.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gmklcqagq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gtxpyywjz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gjmpuzyuv.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gwyhbjzva.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gyygbvgez.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gwgkboxox.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gtasdygmn.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gtwuehlle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gyiehpzfd.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gsyniiuew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gscljfdwd.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gltobszss.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gaqcccmws.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gkwnithgn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gbxhpawfp.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/guxcangpk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gnxogzypm.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gghzmsbhd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzdvzawcl.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gvgnjcmqy.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/goahhwtai.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gtkcptlrb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/ghctnkrvm.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gmvnzmmgh.sHtML


<!-- 参考信息 -->