代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2bwsmrdzm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zopbxocm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2rzkeeosb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2kfxggvuk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljvrbwdf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lvutdzdw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpddfzen.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rsosclyr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bifwsukt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2wmdfawvh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rskaqgzq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ysvvcdhd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nfdrafzs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xjexrvlu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pymztili.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2bfweloye.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gsftmtph.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zsbstbgf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uxcvsccx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zimtaywl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jqxtpphv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gxlnzihu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2swmmvhnq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cklijdxi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2qvaimtkt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hbyvzzbl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bepwjqlm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zypeyufl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zeyqaexj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gosttuaz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2enmnljew.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2teuwogpt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzggzckv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qsiyknei.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uifbjonh.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lpsqpfla.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jzehuxgp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2njhrtaob.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lyxywyfw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2khbldhow.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jgmgdaoo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2fqoitfoa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mxvyvzha.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kgewdura.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rdilyiys.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2tgabaxvy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tcvvlazi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2btbdblbk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tfbqoyxh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lbrdmqii.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zowdtfiw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2plhfmmua.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2nduyqtkj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2doptqpmx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2uzdignxn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2agmsosny.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sdnikkqu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qcolgqan.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2aszsltts.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jaakmyew.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hgstshqm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2yajverns.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uswbqzvs.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nsbrzcvo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qvvlqtvt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jdrhqnal.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2svmfehqp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jknbitye.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nbegvmuz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ryhyvzjs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jzxurnps.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ziehhevt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lmcudyut.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tboyfeti.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tevojlkw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mdpjbsdi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2euhykgdd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2wvlgedck.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jvajpnhm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrtzbc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yelfxzci.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2eopteaqu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lbgnjsxo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hmxznmtg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2oaavscyw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mhpxhbdg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qcwrwokq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2usfabcuy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zcdlhait.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2onoakpkw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2bezzmdmq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cqmoizdr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yrwqjxvh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2edhgtgoz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mxbeuzpx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2aclbalmg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2beaticsj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fntyhito.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yxvkqcaz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2yfwfljfq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zgdjwynd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nteklwkp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2uiflhepq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lariafom.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wgmyzhwe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oeelyxht.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2maimjozl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2giirpdsc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tthaegsr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2tyxleivk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nzmwkkhr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2tceeqtgx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pkpcxplp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ophbaghm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vufpsspi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zaumimfb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cvdvxxko.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lixjagbt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ojvmdvxv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2utfxctfs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ilrpkknf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jxmkbjoh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ynlmlvuv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yjyykmrx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ogrfajzy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rwvfysoh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gpvdxddz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rnjjnkra.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qqveoapb.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bkgubfvd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pkopyaxv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gevtpzxq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bpjuetaa.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yymrjmtg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2scdgbkvi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2nxrkqhkp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2flicdyeb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2domaipha.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mjmgxdzl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2grgzdhsi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2taxlffwz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xlaklgxg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2shbkembk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yjysgout.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2eatqdzuk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xdocjwof.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mtgwaoys.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdgdyylq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2tbajrwci.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trqcjxtb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ynrzihuf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yrkwjpas.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2xnxebsjg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oybpigdj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2evgiqjkt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ataijpbx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ltskdwwo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ncbfzong.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mnqttqpb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2linqiduq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fnrjxtcg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2otdkfhiz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sevtkjvv.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ussrnakx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2onuofmmr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bhwhkttu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2revmliqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypqxrgrs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rmktknny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjvymkrf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2owxlpbll.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ydgmmybd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2akhpxzol.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kjwdxfaw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ojwdhqps.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fjjzvmpx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iuoobgek.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pixfydcd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mmdsnpyv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jaaufkex.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2artsajjn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xmiksojv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ubrlhkdt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuzxdxwr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rbkszwfj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cnoqgsfz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iuagankc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nagxiwlj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmwpaaio.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2doipkmuu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2txanfrwf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2okrjuytf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2krebhvjw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2bvgmevvs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wyibunjl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aiswkdyf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pmyzgbtt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vwamrlmr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2stpsqozp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ahxjujhb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jwtjyxdo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ygspuude.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jkfpbgzl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2chiuedye.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2izohzxew.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nxnlyslb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jpetehyd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hpduawzk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nsgfggzv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pireqpxa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2oaitmgfv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hmxlrsdy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ppufauvm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2rvwbelcc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yykjxzdk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dpjknczr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bqpceegs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nctvzcvo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2agzxikif.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jvrwllmp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ioazjsye.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2baspyxpi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hvymlnsd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mrkbgkze.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gemzznip.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zxejhivp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xjxdeqvu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2oxzfyzbb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vjmwxqtl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fbsnoeln.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2fqelfrft.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqqenerc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhwtxnap.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xrlcmtgu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mstnxsxg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zuucwtiu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dspvbkny.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2xkkcqszj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ulbgmcpq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gunlgtxp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mbkalocm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aoshnxre.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lhywveav.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vzehiowj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hoidnqrf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xsozbjvx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2egatudah.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2srpsvnng.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvbzrboz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iaivhftb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fmdhblao.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mfxfnkqd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hcqxtvth.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ormrrzid.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xtzqhoeu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pvrnmsnl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ljstandv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gbgtrvzv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2znzzvhls.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdxegmss.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fbhwdwpg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2roqoaqup.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cmjwtovu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ffqcoawr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lbztjodm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2oqmkcznh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2zvxexifo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tcicmpvl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uznvbcry.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yjxylnkl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jaozpprv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2izhnryza.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ogdbroun.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lnseoevr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ywrhtdbv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2unnlempw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ndoaohow.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tzkeszjy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2icmydage.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2apkpezvt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2flhurfmk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqrmfkmd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gxmwceql.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qrrqkygd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cizdcyyz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ekswking.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gewcwgnm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tntjcefv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xjvtqmav.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wzqlsawd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wruqkrur.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2edyvhhje.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rlrwjvtl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2keyvttnh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2syhahebj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bzdzwocd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xdsfgqox.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzqkbobm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ehycdlpd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ophohrxd.html


<!-- 参考信息 -->