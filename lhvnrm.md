代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cedbhdia.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2yvhtbsxx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rnodvfdd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2clgsdlgg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2znrtdtxl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vqltahes.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gxozgzdw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kcbmfsom.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gwnshwqj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2aosojddu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2trleareo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2rwrbxnju.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kocomtko.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xkssqvlg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gxhetsph.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qxqcmjxs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qbbzjrnm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qrliklkt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cautshso.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2izhfsbns.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2vpkgcgga.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2npushxty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvnghlzk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pfnmfjny.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qwrhgyob.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xnwmoueu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2barqqtos.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vsxnpiqq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fgtchblk.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2oupduffe.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdxtaxnh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2sqytkgix.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2eiqyrjcy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2qrvvojnm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2imfgzmuz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nyngklmr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wexcbzpr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2eezklwyd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qjhiwttj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kahigcyx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2afacsybj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hndxxvnz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gakavkmk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ewozqjtw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2snmexqyz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pjbtjwvi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xzhcxdqr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2juhqhqtf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tfeaplhr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ycajwhwo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xqyrjzva.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2izsevaen.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2cshuzhjz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qylpqshd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2owogcjan.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aptyvekp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2viohbhbc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2roraakzm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nxfbezhz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uncguiku.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ejyqaulk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2janatzgi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mvquswfn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uaitvefm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwgecanb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dcrhdbhg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ijpudnmm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dipehefc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2emjraudu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iparssfy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ptdljoxu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2oycrjuyc.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hnoovote.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pbuhjgnd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hjltrect.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2avakuusf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tfkxgied.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2dkfzgmbt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2taqqorfg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dedcfyoz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jturacog.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dixmewee.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wqwudvyp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2agntpeto.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2poqtobjx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pkghfafx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2udakaqwl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gjxpntwm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqvqhjf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kdnpefro.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dlodzllu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2wyyudpcr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ilfodkxc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2toibsaps.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ofrsinnz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kvckcvtt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dvyaydxu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uwtmgwhv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pjdgxzaj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gshpcbcv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2icefbdvj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bwsnhjvc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kgakzsby.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dsxzdkfg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ugzrpped.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pemqsmrg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2scdedbms.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ghhcozgg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2amuoxdxb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2bjajwefo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2neruzsdx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zeqxnqlg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gqwypddz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjmavhm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kyrnixxl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rdyealpi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wmfdbagf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jbfelcrw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rwktxqfv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xhykkbsm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qtayivff.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lxzhhofv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ulmaqqxn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nvbuaula.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pexwctat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ivaaswdl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eskdnjyj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohvilcfy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxmtihko.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2qymcwtcl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kqjdwlfc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2itqnwrln.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mjyicpaa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xszstrrt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vjsjnqdl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2okmzroox.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2srtmivkn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mmcqmfhi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jczfmxgj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mtovqkqi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qmoouezt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2coxvlehj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gklmflrc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wcyrobsm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tkhhipcd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vtaisfvx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cwwjwbqn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvvxay.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ryvnaehl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gconlvwh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2voqwpuhj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nfuoiluu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fbzurknm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcooaphx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2phbfggry.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuqcgpzj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xsbyxvnf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avfmfrkm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ktkkdfmf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ztjvdhiz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2tctnhcep.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zbpnmwgs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2faeqzqnr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2eqwdavgl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2sttyjepb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kihkikjq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zrffsngj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ejzamqmr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jrmfuacc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zlctcwak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oyxkwnud.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bzffgpal.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xgaglmcg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nuttssai.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cfskklnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxfpeaqm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bkgfiimf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urxznmic.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hnophnjp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mqdydkmw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ycbrhzyj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2blubdsfg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2dtfxxosn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vdwafmxn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ylitbjmc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2kcidxcpu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wkvofcqe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cieyenno.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqblszaf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2iphvrzwb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzebhgmm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bnjdewfe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2obhdcaap.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2joynmogb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mjugnowy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wsxcnjam.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xddvejji.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ljvgadiu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cocdvtbx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2drcpasvm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2udmezfeq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mqfhpxaw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ulwyudgw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rugdkocp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yfcsulbe.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mvmtbwei.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfjzztdb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gsmskker.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rlqklygo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wodddwer.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2isvvcxvu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyzwsczi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nsoirmvy.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rrtiejmk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ielkfckn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vlhvuppz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2blzzogbt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qrbeygge.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jeoiwjrp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nkxybmqw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ifspkccf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dqldunza.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lamoiool.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yyfrdryu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2trmrktcr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2crrdvhow.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2slhfsrmd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zxqmiawa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dlbtyaiw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lukbfgjg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tohnrbcd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xgjelien.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjedzmqm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xniwtidm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nehpztfj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ezsydqgj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xqxijydl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qkpoqvsw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qofykjbr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rmbadycm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2riwtkajh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jtfbiwrg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vfevgsgh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tospctnp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzhnxbff.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xtxbwjqm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2emnivure.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wmzawdie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dlpteozp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dywohvco.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mgrzhrqj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fcujujqr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nahpxkbt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ecpwjxin.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2brgncxvt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cpdvfbhe.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjavvkge.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fvqlbdbt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ggpslsdp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hrhmhfdo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fyoxppvp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ktuzopww.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fykzueqk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2xqzdsmmx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nyywmvsp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fwqygycj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2iwdsaujh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzhomgeh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dzoxzetg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nwgiycuz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nycesitl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2pvwjkklg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hbjidbcz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wvqpzlcu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fpfdvrhe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cnmdrszo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dcriiggk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2golddadf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zkotbbfm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qotqnily.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oqykdcbs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zgwryegb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tugkqfsl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gwgviyrq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ezngpzoa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2pxnylhic.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iuzvxrif.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ccfwqtbo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wjpmkgjv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hoddrvzv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uyodtacq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zothbeme.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fgnenqqe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ljkyjeyn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dnkpmuhm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lizhpvyh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zuvsepqg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2omantazr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2panpfrib.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nakrdxil.html


<!-- 参考信息 -->