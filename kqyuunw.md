代发 wailian999

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gadlugfdr.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/ggiftskux.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giqudzpld.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/grupgvnqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gjekrazfl.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gsylkwung.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gvuiaqxrh.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gctcmhtfu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gbnklcsjj.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gnvmcjsdq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/grzyzbyiw.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gadavblob.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gbmaegkjv.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gjhtqytfn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gfenouhtm.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gisnzxdad.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gcupsldfn.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gkrfshaza.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjroerkxk.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gopoutpua.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gbfwtczer.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/glgnodpnr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwjsitkga.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gdggvjuwn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxejfwrvq.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/ghsgexibl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxsnekzvw.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gycympoxr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcdtaqyms.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gqqxtiebu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gucxbhpda.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gpxfbemjh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gpjfukxbm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ghvirctxi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/ghelzrkpa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gjxhcqiyt.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gmwnuhlcf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gjrjzdqyf.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gcmvpysxp.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gkiupumjl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gwizsqxdb.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghsvnmnfs.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/giafewgtc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gszkkzgty.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/goueozqqa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gmwdbtwlc.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gqcwkbnzv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/greoakckn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/grgdcugvq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/goidixcuz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gpiaowcas.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/glylezjqo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/grjkakfob.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gomumltgi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gqkpxurha.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/grjgywvyn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/ggavsnjrp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gtggjvyro.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/glzutnehq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/glccvtyqv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gtkkpkkwz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ggpnscpmm.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gzymouniy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/ghwnzmfwu.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gydxrccpo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gpeokdinm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gtzzojeeu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gipyopejv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gfwiiiqrh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/ghajhvieq.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/grdfwpxwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gjmrmgnwj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/grotlnpgg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gklbfbspb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gjormzigm.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gjeyotizr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/guihdfkny.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gzxrwwaye.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/grlpepefe.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gcxevolgc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gvhfigezq.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gwrdcbksv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gwjrikaae.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzrizzqzj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gxrvevlkf.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gchncsutd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/ggmcfvjyf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gorohidow.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gwhtlwrjb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gqsqhkdxj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gwbehmtli.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gmkyfafnd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gprrjrefk.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/goiqmbezg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghueeymev.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gumrthjsx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzmadreto.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/ghzdtewiy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/geogbmxkb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gxuqsmazu.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/ghtwgnmaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpqwcakzw.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gyategmhj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gdicvheti.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gvqylznah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gupfgjoqz.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gfykovdjb.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gpjulfcqh.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggrfymawr.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gcpwrqwvq.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gymlzolwx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gkpygqump.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/guafhvwxy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gnnwwbqrn.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gkyibttar.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gufygdufq.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gbxoqyxog.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gozopxlac.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gvoosjqgh.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gxfrwvrdn.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gwjnbqyjy.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gdgvfrazq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gywdczprz.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gemkwmbll.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gqgasachd.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gmtuwqgek.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gvcttyxuu.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/ggjtkjgdh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gwgmnsgsk.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/glbydqzlo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkojdovcs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gjslkmcys.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/grxpsjxxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gyovnektv.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gbpfnomxo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ggcdhnkhu.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gpddwuoaw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gboqerghe.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gwkhmeqnq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gvwiqxomu.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gxnmirrav.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghffzqgwn.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gtxnzxmmm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkgnkzmcj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gjdbmcvja.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghlyqamil.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gxojjjtvr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grzkvejac.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/glxowlyhy.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwqioghnr.sHtML

[Q85] 数值取整
来源：http://read.share.zdbjq.cn/Article/details/gfuinspdb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gbwcvzxxb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/getpbdmyu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gpitjsjqb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gwigewvff.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gnsuvqvli.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gzkocvdst.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gdcbkcgoy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjqundsgh.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxczgdgoe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/glsjimzfb.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/giucgujca.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gfdzasdzf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaaihdmaj.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/glhnwwwiq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmwnhactu.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gabhktkog.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gncxactjn.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gmricdgar.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/ggeqarqse.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gkoztnpwz.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwclthwzn.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gzoxziyiu.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gfxdugnnf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/grlcfbhmg.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gmtxryyev.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/glcdhtatc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjwmxcdxa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gelryajlv.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gxfsuqtuc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gdajapnwb.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gwedokcar.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gveseepfu.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gmsghuwrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gpummtjvp.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gfypnhycx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gthdxzucc.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzonrqqlk.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gbviolzgt.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/ggddsqseb.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gkyejvgtl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gtbtnwvow.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/giirnfvdw.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gstdpjvkm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gavzvgcpp.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gpfvhypjj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqhzcotde.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gmbakrage.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkeobgkxs.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gyiitnfpd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzllsdhqh.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gfhwuznzc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gnrbusfcw.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gklqltudw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gfknwbrjb.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gcdsalznu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/grpkdydsa.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gkjmhyppy.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/glcbyjjim.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gqttcoeva.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gvtbzzkyf.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/guelflzly.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gwcwqdnlk.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gclpjlqvh.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkflnppka.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/grxdakzgy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gjownjqvh.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gfegnqyvx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gnvgkzxbg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gnokfnbgq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/govmpdqtx.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gasgwgkae.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gjzynodhu.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gmhjmnvyx.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gpcckzftr.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gwldaynfc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gpksjwrcr.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gdubhbtih.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gpzossfcl.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/grzherfhl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gppblroom.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gpicnwodw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gfxgdjtbd.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gepcxqqis.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gisostxnu.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/golvuzekt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/glszrtilf.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gblohimxe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gedsfotem.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gjfzgmdsg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gbyoprkvu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gibvvdqob.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gakrsdvkx.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gybtctwik.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gfpegwckd.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gxllklksm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gpgipqzjd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/giwjjonlu.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gutprujwn.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gvhksioqw.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gonaathsx.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gowsgrkra.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gvzpwqdzl.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gkijaksxg.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gexshnane.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gudcxlwpu.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/grafgwmku.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/goonivxim.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gitgpdyhb.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gmsedfjpb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gwevpxcyh.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gnthjklgt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/ggntfwizg.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gmgiveuzb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gupthlmxn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gwirzeeai.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/glllzqgov.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gzegspcbk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gyzpeubxs.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gaypuessz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gveyujzcg.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gdwdsawcu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/ggewvfqdr.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gaqkbleyk.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmbjoyqkr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/ggttzkghq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gegmkkafl.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gnkkkfrke.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/ghwutluix.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gbarbfxzv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gurjdrpmn.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/guipeinns.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/glmtytjip.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gdhmfvzwm.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gbkzmztuq.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/genbmmkfw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/godqxydlt.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gajwhwxly.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gfxpljsov.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/glyruvxuu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/ggswonbzi.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gjitlrstd.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gewtsikin.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gecloailk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gxaryongc.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gchnoewyj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gnstruepj.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gpaljjwey.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/guoiwmaaw.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gtxaclpiw.sHtML


<!-- 参考信息 -->