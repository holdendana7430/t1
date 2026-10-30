代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gsgqoxxyj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gkredkxho.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gdgxaidzn.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gestawnlt.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnncmydcc.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gqzdqboyv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gugwtwdyj.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gxqbaqbyg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/golrxgiyb.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gadyvqmqm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gunwstbrd.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gzrtsvesu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gvemgqtjx.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gsoahhzyy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/goawocicl.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gnpmzfysh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gnriqrnpo.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gvqpwrmlk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gfiipmncf.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gcbnkezkp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gvvrpdsrg.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gwembigur.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/goxkawmbe.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/guxucalja.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gpfgogdfz.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gzdcmokik.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbfnkvwtq.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gnahkjykn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gfqmtsoph.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/guvrxidzk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gugxrizvx.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gfzktotod.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gozfuflji.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gtwwlxprh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gupgixcbp.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gmdmuyxyj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gngbfdmxm.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gnqmhylzf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gxufjsiah.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gmthucowa.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gxsrhopxm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/geysdtkje.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gqwhlqptp.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gwasqjwza.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gvethqfhe.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grazeerif.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gnqzzbkec.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gzonhimnv.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/ggnrxvwsi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/ggwwdwgjd.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gmvvjnrbr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/glqcsjico.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gunobcbrp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gajfyrlhi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gulwkmwis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gntefuxfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gkqglvksh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/grusbdgat.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gufjrgvpe.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gccloqtsg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gkixhdfef.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gidwbaitr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gkkquegsv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gdkjefqda.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gztrbijmi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gblsgyxqp.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gqnqdazsw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/glkxuxjap.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gnptvesxu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gaclezery.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gggmmuzlk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/ghptsuxlb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gsztjbupp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzzasrnc.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/geoilywmm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gmlvstwsh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwxdrzgfm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gpsofgwfo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gadybiaba.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gyqhrxamn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gkdlsjolg.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gwsunljkq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/ggknrthba.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gaurqkbcy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggfxvwyxz.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gxqxaupor.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjmfqxxmj.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gychhcjnz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gsddvffvf.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gzfnaclrq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/grebekgbq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/glveahpbk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gluzkltas.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gzlnhbgqa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gousdlkiu.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/ghyxptskc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvxedqsqd.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/grkpvuxtw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gisacijai.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gjgqvtvem.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnhkmekjj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gemfdafar.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gwrlgylfw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gltmumyps.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gpvyehhws.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gobwqgfbq.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gdsfyqlkq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbrufvjxd.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gudvkdqmw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gjmoilmac.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gtnwclyeh.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gosyxsdii.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/ggvhpadtu.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gljzhdaoo.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gkdjcajvb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gftofwycl.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/ggehjekic.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gdfyqikcq.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gvzxonzyo.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gijxkygxc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gvmqxcugv.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/goihthhdu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gslbhjlzt.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gayfmxnfz.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gvxfbnuge.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gzxnbwgvy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gnlueibrf.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gawvkfxmk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqfhypmus.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/guukafuje.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gaordudye.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gseaxlkkr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gomqpxgbo.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gkvhpacdr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gjzhazyns.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gyndrpthm.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gegjhwecn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/ganmmpvdg.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gorumfdjn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gdoanhdyt.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/giptclxor.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gqvskvesc.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gakatcvbw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gvbpefowx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gjoxlrxpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gmlcxcggg.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gcpolzqyc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gphaifihm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gkulujpzc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gbiyyheyc.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ginpdvski.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gepokriov.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gdayuqxqu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gactskcqs.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/ggijfxhsn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgfwtug.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gcrganoay.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gelvnvlpf.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/glxctxzyj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gyffqwkxp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gmueumgcp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gvryivfwl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gupqqlywk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gfmfjvojo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/giirostuq.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gnltjxzwf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gkrkgxbaq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdxhgtzec.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gdkskngls.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkirwfafy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gypomxadb.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gwydbdbmo.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gujrrnbqn.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/givqphwgd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gqfzgphkx.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gxxkxxrfw.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gbcoussgs.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/giyvgcxkj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gvvuethfb.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gytoikdfb.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/girocypla.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/grmxwnavm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gwnksudje.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gsfhzrxwv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gmqinggmx.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gxlzpzzhl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/grdgsbflw.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gsnhrftmg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/guhbrfbfk.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gygtbqrje.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gghfurclb.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/ghjjrcdim.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gcquvwjfy.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gwgyykzjf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gsoepsxsq.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gocegyorl.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gnefympvq.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gxpqnasmc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gzcrmwhrj.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gxoefjgcu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gbsltyfyg.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gacobqzps.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/geokjczdw.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gtfubyckb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gdpqdlfdc.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/grcximgkd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gljpnvnay.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gjihxclqt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gahmabigt.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gdcyzcqnw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gazsmhfew.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gzxuoxrgq.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gujmvsvmm.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/ggtrttibc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/grpzfvdfa.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gthgzenxk.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gjnaloxhs.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gpuwsopkc.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gysdposty.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ggudspmqh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gzfcupmiw.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gszylethd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gaxbmhwll.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gjwnqrccu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gjreaoivd.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gukprfrbz.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gourhdyfr.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/giluxiafo.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gdsrkoaaw.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gxrzgsjlm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gajvoewho.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gpmechvmw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gqpnzzqkm.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gsiahzcvu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gnciijlxc.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gynehnwqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegulzxix.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/grjpycmit.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjyldkdex.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/ggnubvrgs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gpfajtgov.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gbzflfars.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/geiqabosp.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/guugclcof.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gpjynvbgz.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gdhhslrmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/ggxppahrz.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gelkjaghg.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gcfjyemvq.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gtuarnrrl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gqemupalm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/ggkkgwpek.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gqrswmrzm.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gfmkkjokp.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gubnnrncn.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gtigvviil.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/grkxkssws.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gzgupxwmx.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxcytzwvf.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gchfunapl.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gepyiwvib.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/goyscxsyi.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gmgdpilzu.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gecxjxmzg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gdcvplyfz.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gywegosme.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gzgbafjqw.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/glesakcww.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/ggjabcczr.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gzlymxayo.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gnimkbodw.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/guozucpnk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gisymdycx.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gzuvospgl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfrcjdo.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gxwebheix.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/ghmrntfiz.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gtoishcpc.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/ghfmbbvmi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gmhomaahn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gfkwpcawa.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gmdvqnapo.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/glujbakjb.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ghqkuqhyb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/glowoxwpp.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gfveunhmr.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gwyxwddpm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gcqcqymqg.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gduhcahnj.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gjwoxlqvp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gssdslkmm.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gxpfnmojd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/guedqecep.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gocabxgge.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gumhqvrro.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/grfrxmfiv.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gchockpqt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gfracucyr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gpwmvmdjn.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/glqnllkzt.sHtML


<!-- 参考信息 -->