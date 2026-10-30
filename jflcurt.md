代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gklacqqbw.sHtML

[Q20] IN 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkcnnjro.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gzxocuvla.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/guqzrrfxz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnkcnxv.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbretmmeq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/givadagwq.sHtML

[Q23] 分页
来源：http://wap.fanxiaobao.xyz/Article/details/gwcmmveaj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzvrhqgm.sHtML

[Q24] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoffnbxu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gikkchygr.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpofqsfi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugjgvwxg.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/gzpaidrlj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grenrruti.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzloijol.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqfwbkhk.sHtML

[Q28] 求和与平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzsahfiv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyozkbjge.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gnfzokwzn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcyoajiia.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gouandtff.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfkuqmlq.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gzytzzvfc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrtrmlne.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbldpphk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmgwkqaw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/grmptvnmv.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gkmccuhcy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbaarxkw.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gyokcfoms.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/grmfklljm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gaybhpqmq.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmopakwfj.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gsubrgakd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gbsegivsx.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gyseftstb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gbvetvlbz.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrummhec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqrgkts.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzivzonb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gdniouqey.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgeppmts.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gboncxpij.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gglvyituj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvazzgbzl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaedrhnn.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdcabllqz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohxwmpe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrjbrrth.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtonsamr.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/grxjokpie.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gyofpttqn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrtdkeqj.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gobfxspaq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbgpvqjt.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/goftpqhky.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzsygiqk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gawuaixso.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gtojaykrc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gixbitxpv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlrgnmvr.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfxtpfmlv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gcrcjtuuw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwcwhtws.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiwqsrvv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnuwgtkc.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gsfmffcyv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrvykfij.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnatlrwp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/ggffxmpmi.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/grtgiaqim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grqvnpkrr.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiaexcsj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/guyrfolrk.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuohnkpv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ghnqpkgyw.sHtML

[Q54] 清空表
来源：http://blog.fanxiaobao.xyz/Article/details/gscaxzbtp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfqvprgf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gjkunogdl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvqhxhb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyxoiuzl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxnrrxxc.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjmmbue.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdgubvtsj.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gldbgdevd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcopxeufp.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gksizzugo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfuxcwvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gnmrttwyv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gpavejlrk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/genecttmy.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gzdzvhxoo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gyklfbznc.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gcejqbpdf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpanxuwc.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpbnhwfk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gemzwrsen.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfzykkcye.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpaywgih.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcrcfqyo.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgmtovta.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpruukih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/guqulalur.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gbohbqndb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gktbydynf.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgjlyilw.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghakrmslr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqsbxugm.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidtpxfu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbqqiutm.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjflfaig.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjzczpayk.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqatkevw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtjekxsk.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwuwtrxd.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmpbddow.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkcbprcd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gwulbfbni.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfjptbiv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/grodzjhvd.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gzytfzwoa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghisitsnc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gcupkxfla.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhpuvnhi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvmkpar.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbhbkbax.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gojekkwnd.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gimvjcvdq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gxvemkwar.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcuskjbh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gnjirxjwx.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gubhuyilx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gadzgptkg.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggqswhlro.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizkjouwf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwymcuxdp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnetriobr.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzrgdkcu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsclfkpyb.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gzghhxycf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjypamgh.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gdahiaxnk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gleubuely.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbagyjgg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gvdpwzkgv.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvuzwiiao.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gauhskgmq.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/guhewgxla.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyqamuhz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjlingudj.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gjqhgdlfn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbueogvfc.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/girjebkbt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahptjugz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnnpbbtlx.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geshbgnlr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gknyomows.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtpwbbqo.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gxolnpvme.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gdwplnkvo.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/ghfndnvpv.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gckxwazyp.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxtehwnxf.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxztddmdg.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxmcfzhlt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/grytivgtc.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gjexsbalv.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnbhspxez.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkbkgsdbq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebpxfbew.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gttbgauub.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gvktddion.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcttwxbe.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/goatjwdok.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gpymutqkx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ganhdrlou.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gmcjegslj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/giriuxumv.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gdfiljkvm.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gveebtopm.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gfwshduzb.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeaxdowm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjuracfi.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gofgncrjv.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gofdwyzep.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gautzqila.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/guvrhvddf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmytojadg.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gneuspxis.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/godqdchgm.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfteguplq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwingwft.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grbtwgsur.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqijgawo.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuibfbbw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnscnonv.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gzehknrth.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfaahija.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyuwjjno.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnundmima.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gdktpwxdy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldcwxsem.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpeakaxy.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkajqzpch.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxlllxoy.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkswdfmox.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gduljlgfu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaunntob.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctsnewn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbaqqnodo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/grdorvysg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnplfusfu.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkowyygu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gymrzzkxy.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gmdyvjagq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/grremwtld.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gydirlhbf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjvswlxb.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxekbnc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjsmszgg.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gdfhmjlgw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gnqxmlnvo.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhjtreff.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gycduaazu.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gvbrlmxrb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grngrluga.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gimsyunor.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gywmdpzea.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjfshorc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalczkgg.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gljftngtv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gvrvlsuae.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbjazviv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gtotudngk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnrzcfkyj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/giultgmdb.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/glgxuirzi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnsxhipu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginhfkxkr.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gktcspeom.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffxltibk.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxzkxotz.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gauqikepw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjxuumzgm.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkkctpgd.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbouceluv.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyrmmvam.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/ghcehiakg.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdaztyht.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmrlriqs.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbzfdchz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeunqnoq.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gplyixjma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gnqnslrfv.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gifdgedsf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnalkzyn.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gyjhwbgfw.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gosamawbz.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitgufwox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwlmktqp.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gejjqopnf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvifyegj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzexrgcda.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gieaelrrp.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivapsor.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gseylmohn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/grgednzmu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gkhrzmenk.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grwlcveto.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gavdofhmk.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gytjpaowi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnocxnpak.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghytplrzs.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvloldovn.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/ggfmszekz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcjptpsw.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjorkozwf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gwndgpcat.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gyoifjlxr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gujncezjs.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gyocogtto.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcipvhffi.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlhlagow.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlsnfoof.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gixczqjzo.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhbhnlbd.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxzvhvmz.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwbxcaqe.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlegsmi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuvrlfxg.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gyfuetcoo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/geiedgtmf.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynfcricn.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gzfxtpcmw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbcigqdn.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gazyayqre.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gwpkchpwn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtafvlkcw.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyprmhoit.sHtML


<!-- 参考信息 -->