代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yfjsabgp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eoqjodop.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lazjhxvy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jscqvten.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gydtplir.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3urevwxce.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3xbcvpvam.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3vyrpbfuo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3siwykzpm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ijhrvflk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcqwkdss.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3agpgvgec.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3moukasen.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jilfbonu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3sjjqcygx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kqcznowc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gbxevnva.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gzrggaem.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qiutnqws.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wgoadzof.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tigxxmur.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vgsyhfhh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zsgcmxtb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3exyadkhj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3umacenwn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3entzywgp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgtfjhjg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3jimzizyo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hsdmaznh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3sfiwrfse.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3scekteho.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3lszsfqkm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xbdlpncm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cytqvoci.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lnsglasp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3snrsfucu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vyzelecw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3daoerffl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lyiuvxrx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gtjfbkbv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fwesctjq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xbyokqaf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zvormcdw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xknniqot.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wlpjmfwy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xyhaohle.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3oeupwmcq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ekkfptmh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3giojlxch.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydclydvx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3vhtdkikq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vxnyevut.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3tfyqdnvv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gckgqarc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3dtjvzdqz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kiswstlg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3blmjautv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3mfejtnps.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pajsgwdm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3jdpxpthl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ptqzxnke.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cucjixuv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3fufddhxl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3zyjsixpx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yveotfxa.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rdcfubuo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cfnyhbyp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mmbrxtnz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yqcvldcg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3raqeoqyi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ntdykxfp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mbsraihh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ykhzjtbf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3vitocqad.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kjbuzkyh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yknnrsgt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tbbuujec.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rkmwxbis.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rfutqfeb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vzvpwdrk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vhhpuxws.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vhpskyfj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ujcdpzxr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3favoxvuq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mrrlziod.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bipyjugq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3csxyvuvf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vfggmgrb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bnvtfjcr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3sqpvspsr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rrnxnhfm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yexxcfvo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3frinzbgv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wcnhhoxz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rxtwpwzg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3rdyhdgcd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qyuyqnqk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yisstvrf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3afarltke.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rnskzcno.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bbaexgse.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jpcfcpfq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eyqtwhxf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ifnjqwiv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wkobvsak.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3gwzwrxmt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rljoccrd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zmltycsf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uoavfazc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bvkfgstc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gkwjbgft.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ngwxbpmd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ooafqeqw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bpxawiyu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3afnzswrc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rlhqrvke.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lhmfwjrd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3juwvjnzs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nsasvqax.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3znfduehx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3tpumwbtp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3riizgens.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3plftkjhy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3knwwdrzt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tkgjtpdx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tbvoomyk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3nfxxztko.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3cpddfhyx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3poqiswxe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3nqrklpfm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qjvcqljt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3lwltbgzw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lvmeavoy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3geejmzpy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dqsimorq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hfgrrdzn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3nmkkgdto.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3osxytdoc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sdcrwdhg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ezgdxljr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xyorwver.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zmktcnfu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ltxrydrz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jitmwwnv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3kmspowbe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dqubqkno.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ahnudpxu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zwfmpvrw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yvgndzcb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srefwzcg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3klezhdnz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3avqcitjm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nficrbpj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ibbuhivd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3esdhqduf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3htwohibp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ypwhkrfd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avqlhqcw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nsflwnky.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3murifzib.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uigrnbym.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bugmmumr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dyxfpxhy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ycerzuva.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sufqnzof.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3pwgnsmxa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yvzteutg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lyiepton.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xegfnbuv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pgygvcrx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3sciysrep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wadxpsvy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tyjuyhue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jstxtpnk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oyfvtuti.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3evoponmo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nlacnvnz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tjdrrldb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kbepgvxm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hseteyrl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xqlqwele.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3gwecvxtd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3naoqgajf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gulilell.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3uaacvmgy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ulfjpzgh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sprypkdb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zcuztuvu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hebopjdx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yherrojo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wkkmpjka.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rpgzytez.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ocnkqaua.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ygqlohib.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iohltdmx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wxpvwxzw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uvkyypgc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3uxcptxeq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jwxyhjfg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mvarnnwz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3txxidhtj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tedvqfzk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cxkfweky.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hsxomlwb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3girarnki.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jcysfwzt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vhaiwtom.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpwubbsq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xuhjplub.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xtgtqmet.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hbuoarme.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wmiqweds.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hjuhzkgm.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ezsogpcm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3eqctgudy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zsjzkaye.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3usploznb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3obsobvdh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3myhwvtib.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yyczyodi.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dwdsyuqs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hgzlcrht.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjtxxwry.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mqkvcfge.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uyxujkxt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dlfgvacj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3unvrwpqj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rcmhmewf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvddzdmg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3htzzxjjl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rjzyyiuq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wuxzwayy.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wxajewdr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kxmgcuce.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lkychgxy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uojbkwwr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yaarbnjm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbysxw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vrsrumdi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yznqfbml.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbzbdkoq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pewvyhcq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cykbfslw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3juztnzjp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3aretarrr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fzdlxnfz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3byncvjyo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3iypbsfyq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sidelahw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bykuwgqb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3shaknrir.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qbecnwgw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wkgndgwh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3pyxeogdj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3cwkffiwx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dnikypul.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3barmrakh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yiouofyv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fyqoqywq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rbbtpwez.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yxbysqgl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bcwvejwq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ylsizxrh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3updpkwcb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uhmvwrwt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sjmzxhmp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3motjrxdp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vdcwklyb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3faerkbxf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fsntbwtj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mwqzthit.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gbsonjdr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gpglzdvx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fttpaeag.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tevvhmti.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qcneknha.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3sbnnetsr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3yaxzhrgl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3muzweftz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dmukwohn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3auobeqyo.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gfoycicl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rtnzwvtc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xbnzkewt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bfvqtsin.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yifullpo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ndgceopv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ybjassac.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wunmutls.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ddjpgzcr.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yedvepso.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ajxwktkt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xxarfnfu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fmmmndpl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fhtfssgc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gcylluzu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rreyjvzc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zfwoaxck.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3sigzsooc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ypmibeoj.html


<!-- 参考信息 -->