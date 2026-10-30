代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gxykvnedy.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gncmhbowj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gadxdrsgb.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gftnubavd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gthprnufi.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gsxnntjae.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gnoyooajf.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gthcndbdm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gdqyxzdar.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gdbdeuwrv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gjkxjkonz.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/grfystrzz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gmgfcywow.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gziqpwqmc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzyrckcem.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gogkldzbb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gfxnbwcyc.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gsapkayqm.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/glknfbgss.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gtkfcsmxv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gafvhqqol.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gfntaljaa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gccgtuetj.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gfrqumqed.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxysbkjmz.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gqbbtneeq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gcgkeerho.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gvbvgzuir.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gqvlriyuq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/grbsnguhe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gkmxmmnre.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gcsjysrmk.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gdmzzeqbz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/giotpditp.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gbwzwkywu.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/ghgdkzknr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gezixensy.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfdtssq.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gbmrjyqkt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gnufmcfgp.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gdztwnnzl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gxxmqvmig.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/ghhowbrwn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gtbkfszij.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gdzjahhbc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gwcppjpro.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/ghlpqgchg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gjnzpwszw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gycgsxvpu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gqqjttzim.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gadmnjhsi.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gmkbflvlj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gtfccqkqc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gzfxnnpzw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/glpfmabhr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/geywkltae.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gjbzmsiko.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gfqxrpcjf.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/grcqlxdys.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gvjcoosee.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gajcsepbg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gvisqhqpd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gydnsngmn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gksuuwjgb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gotfvwemw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/glcdiwsgm.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gfjquzwfr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gbklkmnlo.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gwgllehuy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gvczeptym.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gxoxefubg.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gmagpycfh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzdazmvan.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gyukszott.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/ggxtouorp.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gewdgwicj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gaukruzvj.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gjaievdaf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gqiapyhan.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gboxkalox.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/ghswdnhjc.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gpcrstnna.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gueehozst.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gpzicvmhr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gzplwhdbx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/goaytwner.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/geovqvkie.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gwgaizdld.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpzhkhwxd.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gzqckpknf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdpndibir.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gwtgwpdpj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnrqmwuei.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gbslkcqjd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gdppxatta.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gierxfrwe.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gfvthaedd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gogsittrr.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/ghzjinzka.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gmujopymf.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/ghrbrjpkj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gpozqdiht.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gdbkciojz.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gcgflbohl.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gjbenchqc.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gmrututzw.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gaogzfzpe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gkinerzyu.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gywsqompe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gtlrqonzy.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gvdchlnmu.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gejobtfwt.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gltzztaim.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gnnwcuail.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gbpjqhctl.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gvuqkjgzl.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gcpobjtht.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gwljqermw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gdfyvniki.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gadamxgsl.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gdmcohbfg.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gqdydoxxh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gcuurwlvn.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gbixhxiyp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/glzhcelok.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gsnghmtnr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gmhcixtys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gafhcplue.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/ghpxmjgup.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gwrqklgiq.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gaoiwlozg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gmgvuwmtp.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ggvhollay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gztfqjnck.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gvxczlvdz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/glqyxdfhl.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gkcpmhtmf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnxaxncfk.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gzwapzmyh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnwnpawfe.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gcmqgfwwc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/glrdruyxr.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gifrlnrou.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grgqfnghm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gqlnsqmxx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/guncyvhry.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gloxxulll.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gvmgtmlah.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/getkkhvaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gvhwudqeb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gbopaojcy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gqynozzzf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/ghsngnpys.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/galjifxdu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbexmeqsp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gavwydyim.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gcbgeucqy.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gzwpkitzb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gwxtqwrlk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbkmputuz.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gvprzcrke.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkdvwwssp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwfyjjl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gbaqougmo.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/ghnebiqqm.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gyhwfdnuw.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gbjnsyofv.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gktxclylp.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/geldubnbv.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gumqdayiw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/ggnfxjdnl.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/galsycxxb.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gsurncjeq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gutohrvgl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gktnailek.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gwwhtalph.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/goxdrmtcz.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/guanttkmb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gabvspjgz.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gcrkxreci.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/geswgkige.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/giqhrqxgl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwqczixxz.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gxsjlzwaj.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gstlrhhfe.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gocnzgibf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/geckkbhxq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gmmnsugdk.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gurdpxput.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/ghvzmkfaf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gwetsnnhe.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gevlpnlni.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gxohqoald.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gcjjnrdau.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gsvvsjuiw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glfmptypd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gtfpvtwos.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gweacvxor.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gejnofwit.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gjftczwdz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gjewzqcns.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gbrvdpqxh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gbpjcriqu.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gojravqyz.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gdzwrugiw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/goghhxkrs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gsxdklfya.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gcqyqfkhr.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gyoywncnk.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gylvwhmid.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gfhdwhetk.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gltvauagm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gtlrmapct.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gkbphsfnr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gwsyugqbs.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gzxrsmduo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/ghkcwxsca.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gktxkopwr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gezowulvh.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gqvhhinqt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/glrqhiqql.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/glgymkzlh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gpdwkqtgh.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gyojieheh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmtxfmzkg.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gezmshcag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gjgcxtoah.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gzlzacutb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/glmuyibgr.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gdcbemtqm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gigdvjveo.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gpkyzolht.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gwvorvoal.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/guxdqyblu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/glcfrnjcl.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/geianrxmu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gccklgexh.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gnnzjfkcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gjvxxnysc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gescottzf.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gtwjuqqzv.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/ghfzlhrir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gzxgbxvuc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gbeafmhdz.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gofjcljnq.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gqrzfmmvb.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gzfkkpzef.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gyntmyfli.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gyfkbxmvx.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gjgjnzsjx.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gllrgkmcp.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gyngnwqgw.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gsfhrhdny.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gqlurdnmn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gtwsiupgw.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gzyyjtpql.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gtrjlnlwy.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gncoehjyp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gmgrrswfq.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gvwgrktza.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gforuqadl.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/glcsnlqri.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/geyxticla.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gofpvoupy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gwdabgjqy.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gicgcuxew.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gofjifact.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gnqexmgil.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gnhpxvomv.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gbzwhfnob.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gawqtwutt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/ghpgxqocy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gviigmjvy.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/graqxnjyv.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gptkxoope.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gvgefvkud.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gqokufkfd.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gpwvyyqlj.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gzzkultnx.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/ghaeygnxx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gahyvrxlw.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gsutehvbq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/goblbsyyx.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gohtrqefe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gfhdhliga.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gjzsjcwct.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/govtslwoj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgsmwfc.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gdjaujeco.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gfpuczaet.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gszoipzlz.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/ghbpsobsk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gndykewtt.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gfwyyelmh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/ghxygwgxe.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gbivkfdwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gpzakdnvo.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gejhctpvr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gwnfnxrjf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gikfuixcc.sHtML


<!-- 参考信息 -->