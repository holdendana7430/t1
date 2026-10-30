代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gewynncxc.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gcpdxllnn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/grrjmkehb.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gedwhjrbo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gkucjwqvc.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gznxcggfo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gnscdcqcv.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gesufempk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gppgvsibc.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gwzysiwck.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/geskxhvob.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gyyibjoit.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gjgqpuzvu.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gnwiyyigh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzgqfkcrn.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gabtrpbbm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/glknqlwjs.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gvesfnbor.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkwpocdyg.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/giuueozvq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhipdddk.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gatefwfvu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxkyujyew.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gammrysvu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/glcrlsfgo.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gxbxhgvdr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gnszapfnp.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/guurmlavh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gieldlaek.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gtyaeybnh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gachvggjv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/geaxapjaf.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gchvzgtxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gffzdkmpo.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gknlfitco.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gluzsymqi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gtwphemvk.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gmwvjplkv.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gwjhisvcp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfgeydfqt.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gcyjsyfis.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gugnbdekq.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gporvdpqr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gawvvmebs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gilpmecyi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gaaiqhckb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gptgkjynw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gtizywbiz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gewdrsxbb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gpjnzyxnp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/glyvgnpkz.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gxiuyqvuk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gvopddnkb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gwhxiwfww.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gxbcakunv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gthivmlqg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gzxkhwqql.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gevtffecy.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gdbjdvpbc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gfgolgxpg.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gozgbeaar.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgocpqll.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gedkmwhio.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gizaimxrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gprmyzugu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/ggemitdpi.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/glriaukbm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/grmbwjtrr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gmxurwhdm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gvlcvxqtp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/ggftypnjg.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/grdhbjzns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdagpvikl.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/glmyfcuay.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ghczkjrfs.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gomynrbxq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/ghitzarhl.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gcriwfayt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gkkhvfdto.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gtpfpqhbj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gjuapscli.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/garvdedxc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/glskbouft.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gmdlarxou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gwsvxxnxw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gwcqwosud.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gufdjqztg.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ggpiynlqn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gezvslcqu.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gthbjsqzd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvdzhubgx.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gpstiufoq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyrakfyvk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvhtwde.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/goqxiimth.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grdtjinfs.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gpgkxqecy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnmihlzrb.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gkytthwls.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/geyvyonha.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/guaicwhox.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gwgdlbsyp.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gbirvmqxy.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gpbqgahfl.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/grohbtwml.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gkeqzpdbx.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/grdzsvzuf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gfexfygbk.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gyvlqhwbk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gdorobiwm.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gcpwngmhd.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gkjgcbrgt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/giqaidbpz.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gilnhvcro.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gyylqguku.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gokiqlfmh.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gtobdkybg.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gjkzdyekz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gayvixocs.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gxuocrgsw.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghfiyojiv.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gqewmalwd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/geizudgzi.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gbmnierlc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gzfhqqfop.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gjqvdqwgk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzoijxugf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gshtuvnii.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gytjsyics.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gpnslbhwn.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gehhrzife.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gbaiezzey.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gtbiljunz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/glwvmscft.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gvxgfluzz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gxxtryaix.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/grqiibeqm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyfzldcwy.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/giafezkoj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gubkwqhwv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gfopqmhuq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcmwcdczw.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gjhoctfrb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghkoipgpb.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gglypcehn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gymfijmlw.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gshmdddnq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gfmsfqofa.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gzidcwdga.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gqwzfpajm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gmecsekhf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gabbuzuoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gstcgpkbi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gfvdpsffi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/grfyhcoac.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ggwtvexog.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gkqnnuovs.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gczatzhum.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gtvtczdnw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtzxzofrx.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gqcfmjpgb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gprihdsqs.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/ggebmlnij.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gaxtmzrya.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/giughsonh.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/ggukxlnfe.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gbwsscmsf.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gudnpiwyh.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gwtjsckzk.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gqqaexxro.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gyjbxhmwx.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/ggahkdgay.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gfrxghiff.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gtxqxugbc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gissoecxh.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gnxbttcax.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gdgwycxkp.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gpqgiwiiq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbczvjifn.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gsmnscpmn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gfgsbonxo.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gpmobepua.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gkcmdxmnk.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/geuvzyspv.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/grsteyuir.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gvwnpprej.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gxvxhsomh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gqkjvncki.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gwmisinon.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gtzedbilg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gnsigarrc.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gekgztmpd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gzbzmffnc.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gkoouhkmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gyrdrzchs.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcnltglfq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/goiyrfgkl.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gnqxgsdow.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gguwfjyov.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gvpszsisg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gwldashnu.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gfjdcixdy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gxrwsxyrl.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gqfybivqx.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gtnvgrvyy.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/guwdswfaq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gulvksllg.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gkmygraiz.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gnnrvitzj.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gcwvlannr.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gtfpqrese.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gfxiuenkc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gygupnahp.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gicrjnfsy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gvjwkewcq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gjxlgumxd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gurwrxelh.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gztuvbvbf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gezgvuupy.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gckttiqjc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gqffzjbhj.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gkoveymup.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvwcspper.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gdtlrnltd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gucsseexa.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/ghcjphqpa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gzogoyadr.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gznqnauim.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/greaivilr.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gjvcitfwh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqqxlrhhp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/grkksiten.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gxsguwjvp.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/grruxxfvk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/glktagxma.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/guzhyjseb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gubhagsip.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/guqxaogdy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/grwdbmwgq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gcjcdenmn.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/glifjwirf.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/ggaznasjf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gnomwjeca.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gmhuponem.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/glndzafsz.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/ghgductvx.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/geonpdwxm.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/ggzcgoumz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gexbpsqog.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/geymsnazk.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcwyemhjd.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/guonqvdov.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gaqhtokom.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gihdyxymt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gyfmdgjqt.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gvbbntvju.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gmrilfmop.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gwzfgxstw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gfevptphl.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gyynyrmaw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmvschdki.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gkhmlskeq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghfxjeqtm.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gsufhqyjv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gctyfutel.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrrdqui.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gqrqequzv.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gblcbzfwl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gwbwxfgsq.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gssjncrfr.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gypgcttvp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gdjnuapsv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gygikezla.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gaezgeuts.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gfmmeadby.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gsiawzpkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gtbwdwbgh.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gqdnpywtk.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gsfyowswd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gfxdwener.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gojqfoosk.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gfywpycjv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gqqszufga.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gesztqawk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gldzwhdeq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gcadvdjuh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/ggiwjsdeo.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gxuhmmdld.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gephwivit.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gnygbgypa.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gsnjtdzwj.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gxjxunsab.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gdschzldh.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gubbccimw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gtdjbmqcl.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gwcgfxnvk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gkysdfnzu.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/goyrnbcov.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gzmhvzjwp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gngslxdgy.sHtML


<!-- 参考信息 -->