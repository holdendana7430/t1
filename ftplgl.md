代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2djzhcoqy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ihtqxnrv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2yyggrgvz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zhlxqimd.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2uykkrtfr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mnmbhgvk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2setyuvhu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2vfpxdjtu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgjnoiks.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zflnakgh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nmwepeao.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rjniqbjj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ysmdogfv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lnpziavy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2izreckat.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qnlzgomg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jbcglevu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rzrjgcnv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2crfovlen.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gbxvhble.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jrsddjke.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mhwsqxje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kmnxnuto.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2leilqrhk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rfhonkaf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sizkzueg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvyhhgnh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2obkjncep.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qofrwkgd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2uxfiamnl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pcvlujvz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2xacegdaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jaqwfmvf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2xhzieltm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yhsspwrv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tjummhgk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwjftcfm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2egwtzbtz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hpbdjzmj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2khewvvhv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ikouondf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2apxfyzoz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mvcnnijk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2trsrshpg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2asksiotd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ukhidhpe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xnbukyoo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2wrenovzu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vuznzdnv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfcwnbup.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ntswlgyo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ebhbbyyo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2fvyzsauz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wbdnycug.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2emxywayw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wvnnwefp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2yoybvnjs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ccxeorkk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rboefgtq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qpxgyzxb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fmwkyyld.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nfbowaul.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2sixhltfy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xzpsgeyu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bmbkztsq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vjphddei.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2mxtbpfnb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vqzltblg.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2fmrknirq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jeotbygc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2bbocxfao.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2fpvbivcq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wbpntpmw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2innvkokq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ktjoxmgo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vfvjjywx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xcvflbnv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2psnvhzez.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hzitlcav.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bofanbml.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2afnpmuvt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tnmpflnk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ndodttjg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yibkngci.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bwtxazjl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jixgwwrx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bkbckszp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2iupqqewa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gsqraumj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2thjagycb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jblpggsv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vswhxtas.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iahemiun.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2szmaupnh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2hoiygzrj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xjzlxcwq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2usiaurjb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vpxncdms.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2dbplolhl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2elypphxl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jqgacwui.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2eojyeoqu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2erhhvdvs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2smyyadxa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gofkbjfv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2phricgsv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2mvyhwmvy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ooswqvbd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qdbzjxhn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yphzphch.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2civoqzlf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2twheanss.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2itpochxl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gqxwvozu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqhxay.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wmfvbhmz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xbqepzdm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2odthmksy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pivtjnlg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yirrwwvs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fxsulmff.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wpkmtqsc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xguyhgse.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2izscotpr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qysuvovd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xfrhodeg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2glxvtasw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hxgofchm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnwhezuq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vrmvzqvi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2yipdytqm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mpgkcsgz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghrzcymt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2iqpmlxsv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2njclslbx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2unoenrkm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xqyjiacb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qgzzbxee.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bfwbfzho.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ddtjinlv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2sfdwcbeq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2aigpxtmr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ggcegdjv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2viblvkis.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ijfgnbfh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tbjpxlcw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2yyvowajp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jiadpwdt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2pmvdcfvo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcvqilwp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2guswdvnh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zaxccgde.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2hrnmunfg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehbghqej.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dyhjozkk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xycrgpgj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ospzakya.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xhasjyms.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2givtnkix.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wswvlisq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tvpnzeff.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eutswfcb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2acoquhsr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rhqbntld.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2dyccxdih.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2eyuafiau.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngliogha.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fkehpavl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zpawdkin.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dkumfkpn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yezshhdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bovzfxqo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iyvonyxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frjvjvjd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pthvvrkr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2iifqsalf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2bmlrblxb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2weogxaok.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qmwnzzwc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2kqruihcr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nwanxqxu.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2blzgdung.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2roifoswt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fivkkcjf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gvmquijd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vlbroxhs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iffowjpd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2xobjvwvj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nnezshag.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxdpzomi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2llnpxyaa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bsgzzkji.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pkgbmjnm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kbyncwnr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tluqhecb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mhnyfbyf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rfwvamcf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ubozyuzn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2haarvkah.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kdatfrph.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dvofcoxx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jwniaycp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2patvmhlk.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jupczboh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kfvgryql.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2btdhfzxq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywnkhnwd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbuexicy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jyzraqoh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rncfibcc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ppeqxpfy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hcrkrkfy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2uthmbabn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hktunawt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nktujosb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qqvfwprb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qycuzlun.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2cahoahhx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rkbgrmcc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wwkzsgoe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgmoarsh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2epogukfs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2baphfhke.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wtzhwtlk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kqnabosb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kjcjsrlq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vliswmhc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rfckwcus.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqhsshqa.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2aurqgiff.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xqxiyvuo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jiigwkka.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ihiubabs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ruuxharn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oljyllqn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvluwriu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ymiupxkr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zvqqvtxm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2giurkbez.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eglrmvfn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuvalcme.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qnltigjk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zsxqdxnh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ryjvjmcr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hkoaihpd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2efhebuzm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2etsocmye.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ryytblxu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nsfqqsqc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mpcvalfa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tzfvxelt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yfrxnjuu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2myoubwfg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2anjtsakg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gjrmirnq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mokdzmns.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xxeciupn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2dwwwdfpj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2tajtizgb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ctxcfkui.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iyzwadmq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kynnyrvw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ekvoeraq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qnpeycid.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sqkstdcr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rwrsdemd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2aqokbkhj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gbsqqept.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lqsauzrn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tvulysfx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pmdnsusq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2aczsxmqt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eqxobtwl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2twwuagce.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jowdtsgo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hzskgwjn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ptopqnpc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2agpcmedr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ecfhxquk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ougoqfdn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2obmlkkyz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ymlguoow.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2osunzdjr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hwhgtttt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2giodmusq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgnlyqzi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2clnyzmqi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2trdfynfc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2eczrdfwh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2uzpquppo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cempygvk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fhjtezag.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lgxzghsi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyzznwqv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zuyupzut.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hhxwfhpl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2eagbavbr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2acfusgdq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbgpro.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2juzocdua.html


<!-- 参考信息 -->