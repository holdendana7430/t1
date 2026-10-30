代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqxftquk.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/giocshppo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncogjohw.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/guikeahyh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpvfykos.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsinwrciy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfluuoxin.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gsylpuful.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcqeiiko.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gwnrmdrrw.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwwmycrqw.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/gufoclzpo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvwqbkjw.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhujsjoy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gzqhsqhfq.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxdjykq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqasxgrmx.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gsmpyiqvu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjwriwix.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gypgbdmdx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcafgflsu.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipmntkpn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjpdmcvi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiurxqgv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuwjpsxo.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkscgfhz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gmqupsxtw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gynqnoiwi.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gsodhqxhl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gbqnnmuxv.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gwxucqbyi.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gkdyxusex.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gxmjylctp.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glazyonhg.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlwlotdu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gupxiiiqx.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbhmjrxb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gukanbmko.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbtavfwm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdbkjal.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fanxiaobao.xyz/Article/details/gkdialmfw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gtfkdeyuv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaibygoqw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjtbdhc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gepbjrrlw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gwqvhmpwj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtavcivwz.sHtML

[Q41] 多表连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqvydudoe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gornmdvho.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwrwcxwa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxvfjqzx.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvquuhpal.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/ghennepha.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnmvtzes.sHtML

[Q43] 标量子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gkttjhvrt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbcilppk.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/giouvtrgd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gjzoqlpal.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdsfzeged.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gvjtzajae.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gmocjkbsd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabipijjq.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjasasyo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsifmcthj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gtqwvpedp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxjzgrtz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gszwykrwi.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmptrkhxs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnzzdwjl.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqdqnrtj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuwejenw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibxtwrpz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvjgmbdh.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgbtgpch.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvckbkrwe.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gehjlvqpn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gmmqpblkl.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/glmeifcpb.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxrxnobh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/geqdbutrv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gljjyzsns.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghattazsg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchflkolu.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiihktcl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gibzopcwe.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmxveyr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzvlysbg.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekehamul.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvnkvvqa.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gbunmgqpq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbypsowa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggejefgit.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgqeyenh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwraakhk.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiovemng.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gogezuxzq.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxgxlsyj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ghluekgnr.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatftttep.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gjxtkhfzp.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtwdhvhs.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuzwuibh.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelnoaue.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwskjzya.sHtML

[Q67] 设置隔离级别
来源：http://baike.fanxiaobao.xyz/Article/details/gheswuift.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gyibodhfc.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gozouazxb.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjobgnvdn.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpisjkcpj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbnuyprz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoxovolf.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/glfkhwjki.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfanhfnm.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqulrycz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gzroepbvw.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxwbaeza.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpwzcgeis.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxflydgh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/geznwdkfq.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gitrcnuor.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdizxfdr.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxannzgjo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaffxtupy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeygnemq.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmaojgtc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gpjrvokft.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gsijmsuym.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/ggyhuhmpl.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gugnqfcum.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhlbribn.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzpssycs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/grrfkahus.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gsluocmtj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnbhvyca.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grvtldsgt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glymjjtek.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gckpdruhz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcdgobmmy.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxjunkei.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsmuwtth.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gxevhynbr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gkuswqmty.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwflkuxx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsclvvwko.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gkjozppaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylbdgqjl.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzitkpuwe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjcyunrx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfmsngyv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gahzwznmq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gagsfxzbs.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwdlysth.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxyniufl.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gpoqejvdq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbtfngn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzcptpocl.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpuelneok.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgklmesh.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gitvoxipd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkinjand.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gyivarlyo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gfxnfoozd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrwbgnks.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/ginlcwulq.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkdujemk.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpcajtwnv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhtugoso.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwbeutsx.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqhhneck.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgllazcl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gggkotnkb.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxjyjqkv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqgqorezh.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghsvmjhsp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gvqptyepw.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgkepnnl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/groklznjg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngrwedgx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvdnralo.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/glybcdpui.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gpynemfem.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gczrugrxi.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gymwsvqya.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjmtpwdm.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwrqijvd.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/golsrkcgz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukznmlpu.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gprgbeylo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsjlzyuhq.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexiicvkn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guajzjhlx.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmvnawhcd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glcscrgjb.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzonmaiuo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtwrymzl.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gsyaqbxdq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/giodemlec.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gikvvhdbj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjhkqsyg.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjmujshib.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnzvszued.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gygywcpoz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsucawsbz.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuixfnap.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgtfwywo.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gxweleraz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfegjuwcz.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gefseyhao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtbttfzr.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gryeozpad.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqzqpgaca.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gnsdjertq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucufwonm.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkvftewxf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwizkwyy.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcwneqbp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqwewrdz.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/ggwgoemki.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gpwatrtjf.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxqwrudtf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuknuvba.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/giajsphsn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnvrnxpt.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfiitboe.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnpzhympj.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkyryvdi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/giyomccvn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gqzjchrrb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gkzxlswrv.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gysipcgle.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gsapkzzir.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacpczcot.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/guvztdxdv.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtfsoctb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/grygkdfmf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/garlkdtbe.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstznuikb.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwahbpuau.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gdynjgnfm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrkjeibv.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gzwcxuegf.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gryqnmwtj.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgegwyqy.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gjhlfixaz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbigmgvv.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gxofjifwi.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemmpblhd.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghivdakgr.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gznahkqff.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdxnckxo.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gcepfsvnb.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gvmhrrghh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gselkoudx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gaedytjow.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbpshxbc.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/geqzwxrkz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbonqofd.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ghwguhcgn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpncushrn.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtxuebpzo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gbycbjrhh.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqrswpoo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmcuiefs.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gbhswwqcn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gzejojtiw.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gdahlgmnc.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnuxgqqj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gmitjdlou.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzqjrljz.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsqbcdlqm.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxrdefjv.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/ggfeetgvr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gslnkvwwm.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gneavzrli.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/goipcmult.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaiwmjxv.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdnctuin.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggxupkeiz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gaojuisqa.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnrjcuhq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/giyfehvsu.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqfypmpko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grqdazjql.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gqezimsfl.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzefykgm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdcmhdne.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/ggdflkoip.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gwewcwiip.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gameqgbnb.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpywmrbl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gufrwdnew.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbashodj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gthtxqnrr.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttxzrapr.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gpejhknbc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/grmudpunn.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtxfxbcc.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkczteku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gecaufxfm.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/ghzsxwxpk.sHtML


<!-- 参考信息 -->