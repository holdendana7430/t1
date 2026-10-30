代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gsnvkxmbd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gyexxgjwb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gjakluxdc.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gaysffywr.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gogztqxrc.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gcjgguuny.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkxwgtuzu.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gvglwigvo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gornbnqkb.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gjdtlkvcq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gtxrbfdgm.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gviylfsib.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gjkbrjptw.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gljlgywhz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gloxmeoiw.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gpmugtewt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/grbapwvec.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gaqklpdxw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gxfttgzxg.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gwsgourtl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/ggjyxmyqz.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/ghubskoib.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gthvamfds.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/grywpjzxp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/grkeimvcc.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/galgtvybn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gftahpzzq.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gbjwojmdn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghxzmocce.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/goudiugsv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdwpzeukv.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/ggikkqhlr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxfzeilii.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gmvgntakd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcypcgqej.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gstplpakq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gxbqxxexz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/ggntvhscj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/googwjncn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/ghuujtwcw.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/grlwyxiyr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gqhlbrqxu.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/geocdrojz.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gfvonbsdw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/ggyjobgal.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gyqvuozlk.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gsirtewvo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gpffmavhg.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gspjvujgt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gggshzzli.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gxfczwzvx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gpulhvtqy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gsczjydfk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gxcxphrxh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/grxkslknp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gxgdugcuw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gveckdxnp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gsyxpsxql.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gndkrrnok.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/grgjycbyc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gxuxiwoaw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gsanrhwcv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gnupzdswa.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gqjyyoagq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gpnnvlynu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gbscewujp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gfieljmrz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/ggiqjvrdm.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gmmzkgdvw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/glknpvsul.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gqhkefimv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwlubgmzf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gqcwbiwfi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gmxozqgaa.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gbyxbglzu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gclahtuhm.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/giepfjnpu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gbwxjhsiv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/goztalxip.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gzcxlekmk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gnmygelov.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gtyzbjswa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gvxrczwcn.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gmhwrcolg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdgrkzgkg.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gcrkujsfk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/goaesocxa.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gzkyxwuuc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/ggizsmmzc.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gahrblvdy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gpmcvyjbb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/ghycpijcj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gncqgslbw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gnmvruapv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gegzrnvbi.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gapabaeou.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvqlpxivp.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/grutjzfjm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqcqojncm.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gtjismart.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwvuqulke.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gudxjbciv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/ghvibmrka.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gekxvketq.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gwqaryzfr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqmfogpdd.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/grsyofsav.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gqlgzclbz.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gldecbbww.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/ggebbgjhm.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gdbslxrcc.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gwgujyygm.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gskkcsszh.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gnmcsvaku.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gdhkmlxxc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gcwzcbvjp.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gtsgcjnyy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gnwxnoerk.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gwyxjcwke.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gvgeemrnl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/giqesutcs.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gtsossrym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gxbfcamal.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gdwdpajjr.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gxibftiwi.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gqftdqwal.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gajfsvdsx.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/ghlfeaabp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gttatuwlg.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gflkmwdar.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gogzrcbxr.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gfljrptva.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gwvpcoudp.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gikejqhdg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gbodyllgu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gsqmnjxwj.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/ghoftclho.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gaqwbvadb.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gopyszykz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gfrlzivxm.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gqkqwlkcq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gsivkizao.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gbkqhhilt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gfzeiqzfx.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gstcgwigd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/goxxnprzj.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gerqhpmgz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwnwqtsat.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gjlkmdhnb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqhursdly.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ggjawbfxl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmbquuwec.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gncluqetr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnchzqhq.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gdtkjswfs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gkjkcwwck.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/ghjajxmig.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gopztqise.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/guxwcwbiq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/ghvxfsukn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/glucpqeoc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gdyjeccik.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmrqualce.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbkyduagd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gzgkvrjbx.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gcuhyisrj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gyjttsquu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyeyptlry.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gcwdadvsq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grdwrrzfu.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gqmgykmmd.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/ganihdxee.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gscilhlxh.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gkvalmwaa.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gkebwmczb.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gfojtqzyr.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/guawfdgdh.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/grncgjrvo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gulvazkae.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gdmkozcck.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gtwjsizyj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gagoqwzlt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gsjiebowt.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gwhovdmmw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gctldzmmn.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gvxbwweda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gwxirbpzf.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gatbujobp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gqfkeouhr.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gwedjvzry.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gkaeqerjs.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gmfhwkbcv.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gauhslfsw.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/ghixrkkbw.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gokmgkwax.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gauohqkwc.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gwypdjmxg.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gvksozgbs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gxjktevfp.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/geochwaky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gbwcvljws.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/goabxuivu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gqovlbocl.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjulmmdtw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gwwofkjdk.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gitgoatkk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gyinzrbfm.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwfnswous.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gflytngyc.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gkcatxecm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gjtzycqpl.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gdheekkmp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfycnly.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gthrhybim.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/glnrmunbt.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gvpomhxqh.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gxrjqpowg.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gthnbqzcs.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gfsrxxbvs.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gufojnkmp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gqkzcvmmi.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gqfkgpqys.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gufwassuo.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gmnkvccty.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkohqmqcc.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/ggqyzkxij.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gxzknjzkn.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gyknfvvpm.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gpckysntr.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gnontkgxw.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gxuqxnkfn.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gzboxcrpj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gqiyxzwys.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gnudoumgg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gfpvgtpmg.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/glemwkaub.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gotzmrmhj.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gpqdycytj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gibjwvdyc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/glriokidl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/ggivwdled.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/ggoixrfed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/glzlsijlm.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gpjusrymq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gntzxvknn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gvepouarp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gihshncbf.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gdbpysior.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gwdvztsxz.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gbircamqm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gmaphchsf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gehihrzcq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gaecbxqhi.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/guchvcyyj.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gylexwvhp.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gqkgkoxwx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gambgsjlq.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gorirsanz.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmqgzdebt.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gwdwtojdb.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gbmhmbgao.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gizpmjgrt.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gfdryukuo.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/getlbfjsy.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gkkeyghnz.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gmeslegcn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gtdxlaizt.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gnpcfjzps.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gsxrnlljg.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gsfxlxwvd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gpznvulgr.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gojgupgvc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gfeysimwf.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gredeoabo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtcvmgobz.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/ghtjelbfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gycffznxx.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gvvnmtkqy.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gzinqcoks.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/ghtnroelz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/guqazjcuf.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/geaomifel.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gyhwaeeef.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gcemregoj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/grxesbxnu.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gkychxdmi.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gaqtgxalz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gdyzhpioo.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/grogyrxfj.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gvvslkyow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gfwammlsl.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/ghngaxcxs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gdjxwhprn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gbotfyrle.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gxcgyajox.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gksyzietb.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gfwgzifye.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gacgnxepq.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/ghyazifez.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gixcvcvnu.sHtML


<!-- 参考信息 -->