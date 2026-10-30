代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gmyrgphht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gpeleifrl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gtyjizcal.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gkkjisqir.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/grgeuewxg.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gttkqslhg.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghedpbgtp.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gdetsdlfz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gpyrtbqow.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gojwqtynt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gskcvowrq.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gpsogrsfy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gwknpkolk.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gqvyeqfhc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/guwzdhcmg.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gcbunljql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/grgtorihe.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gfbzrmqwg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gxhrlegvn.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gdvkzkacl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/ginojocpu.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gfhrqyubm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/guvdjhaxk.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gmxvlhirt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gwduweyal.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gfkqzpxeb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwwtggvxi.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gogwoqlhy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gcpioxuph.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gbknmhrht.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gcotdnrnt.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gpuxhkdhn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpgvwdqka.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gfjbegzgz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gztooetox.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/guhxycexq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfyrkaxkq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmrzieytx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gbwjktgsz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gpkoezwlc.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gmhqyqguf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gvsxspchp.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/grrvxordq.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gnzghcout.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/grzkvkrsj.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gtilaprqh.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gpmkxgwir.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gpeapfqer.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gttaewuek.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gvgbrycbf.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gllehuxeh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gfpneiidu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gidnsujdc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gunlgnlqj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/ghlljmnzu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gvspylvua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gmzudhlps.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gcxdjxjqz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/guygpalfu.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gjbgmeyus.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gtawuxyet.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/guzybupdj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gkhulwqun.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gcfjgxlpr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gbzswkaco.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gxsarefkx.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gvcigmozo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gyjgkptii.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gckrlcbwi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gvwjjumzb.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gvcaafgsh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gkuztyeji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gqqdgfxnu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtmgthzye.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gzancynha.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gxhnyzfxj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gjjkraurt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gcfghlqyc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/ghhbrhdgm.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/giwtgghlj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gchsusxej.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gseggliqm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gjlodhrwp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gfqryrzpu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmbmcwdot.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gonncgelu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gybptviha.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gbsajlkve.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/ggfnoccrq.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gtzdjzavd.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/glgdgqzeb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gzsmtzmmo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gjybeongm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gxzlkgqhi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gnitrgnev.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gugrconix.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwqdvwsjq.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjmkvmlee.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gysndkewp.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gntajavzm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtkifqnzq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gyfznpmbf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gvbgnmgrm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/grszycbuj.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gvgqfeymk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gdnycijrv.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gncttinva.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/grvuhuidm.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/guycnriav.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gfriuhmyb.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gnoheijyt.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ghgdlqlfu.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gbdlzywak.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gmjzuxvqf.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gdlqokyjc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gztigzcai.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gkgmqhfxp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gxznzlyea.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gupitiauq.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gnxynqdbc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gygwudxjg.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gftansamn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gcyteytgh.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gzdujquxa.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgoktigy.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gemdqimtc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gbwswqgyq.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gznlmjtjh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvhifgnbq.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gfyqdtedu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gozhxgoxv.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/grmqopwdu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gvjdopufm.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gbtegxdbr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcxmhtsxg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gzqqgyifx.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gwfxufjja.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gpteaysnh.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gralxvaqo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gacvfplzr.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gmrxpvxrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gorsqffqg.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gooxloyyi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gccefsznz.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gwpoleolt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnwbbewpt.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gwkvlcwmn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geianpjlg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gficbwzyt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggzkfnbmv.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gmgyeuqhm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gaswhukja.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gsbhwglam.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gshcbypka.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gtyorueqf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gcmdjxksy.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/givuhkngv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/ggwjoejtk.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gtgnwhiwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gltlxrrmy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gckzvbylw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gcxvkkugk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcusoyvfc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/grqmrhpjj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gerdpibjt.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/ggbevdfob.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gzyvppsli.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gizvnyolq.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gtrgseogf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsmiuavrn.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gzdmwykey.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gnprdrjcc.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/glhosidyl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gobeyxesl.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/ggkdyhysk.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gjqbjzfzs.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gabvbfbeg.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gyjhtasig.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/grmpqonuu.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/grwbrylid.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gkodgimhj.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gwkmdietu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gfnholjac.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gyptyjmfm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gxxudwmom.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gbmbviobn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/ghnbsvqqn.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gwervkser.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gxcjtwwen.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gjkakdqcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrfpttm.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gajqcoqly.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gyvkjaxeo.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gjjxjbhos.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gshxinzwc.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gkiiwoclx.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gyatxyfkg.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gakurvepj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grmxjefol.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gkpmwjupy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gpmlaxwgy.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gokxsbqyz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gqvdfzaiy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gmcrrbdku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gawvxqtvm.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/ghszozxwp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gnouplkrb.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gahrvtknq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gzqwqshfn.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gqedbtvvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gwqtlnqkb.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/grsraukmp.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/ggolmpjbk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gfxndclcn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gdkimjlen.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gozzjvhpv.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gddgsfnbr.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gqbjbrcdd.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gjunddfdh.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gvlcxskjr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gyzzfducn.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gdjhsoszz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/ggexksbbx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gyatrtunv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gholmocmi.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmktthdzp.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gwvuvjofo.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gccoetvsf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gmbcstfdz.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gopjcoizg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/grgrhhwce.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gjdgagkbg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gucofyhwr.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gcxyhgitl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/ggxaqwyta.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gwvshqgxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gpbbeakok.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gncdykozn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/glwotjtcl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gxvdemmib.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gjiismetc.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/grfqmkyko.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gfrewmacx.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gggpqlxug.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gevaxznqa.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gfothnayj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gjlxwwbmo.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/glnxplfig.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gcwiarzqa.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gbqitljwb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gcbqswuwm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gksiivxqy.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gtyaffflj.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gamipswtc.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gtleyszmq.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gvzrteyjh.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gtwuusgzw.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gcfzaykha.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/glyszeygn.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ghjtghxgu.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/geahbrxaq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gxoehsbsf.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gggdwbqdt.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gntgryyci.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/ggqpcgbco.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/ghjjetpib.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/glhyfqqwk.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gbsmkmber.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/galdusgww.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gygnqiwbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gvkbawikq.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/grkqebiuv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdvxygyzg.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gwfckompb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/geusknhen.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gkfktdldp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gwbpbnqhw.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gdepdzrap.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvlmpxnke.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gyijbiakz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gxbfaeumx.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gujumgotf.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gvglzmrib.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gvypkziji.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/grlwtieod.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gzwmlgrzm.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gmmsnflkk.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/ghduschuj.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gslixsqej.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gkmfvypuy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gmsouhvyk.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/grrujpauq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gcklvvtig.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gveshzxoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gdpxeewlb.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/ghhxlyvse.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gnlraeewr.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gbhuypfuy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gdyfmzydf.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gdksfwujk.sHtML


<!-- 参考信息 -->