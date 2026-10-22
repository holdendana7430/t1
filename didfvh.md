代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2feemvyto.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ntdcbjsb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ezjmyzim.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jbhpwzoj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xyakdupa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nituvzim.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsgfsyhd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yqapyapp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2owykoxnu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zoqnvaat.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ixrohqpz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bniyxdek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xiwfsrnm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kypuqeph.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2enbkkiki.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2mnhwzman.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xymofcqu.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ponbodlm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bgigsglc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uxrgsnkx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cmdqdpxd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2opodmjdi.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdrcdwto.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ztaghamk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zspjztgj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gttrikct.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgneirt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2knmnpgka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axedddwv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vpxfsjet.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ohjfztcp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sewxufmx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gvtikdwb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fafmrtpy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hlumbuuq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2brasmyjv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2edbvtlqk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2loiquald.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jczbyqwn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qnfqinul.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jcrempjg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jneqafia.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qgrdouka.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2volvruan.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zfxickam.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2syymlsyk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nyilepnl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wfwuucyt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lfapwobb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2anlhyolb.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2vvnryszs.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gxfcnamx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2tqecylzz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cuexaooo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2irnnzhgv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kwuiodyg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xwmdlehq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ktqmfvqi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jjqlyujp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2htjulycn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gksfarlw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iiyittua.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hkjifcrx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2tjobxdbe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2rkvymwxv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yrgarcrq.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gxztsrqt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zozsczqf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yyprhjtq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ngvtvjfg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iqszbcxq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2udiurqvu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lxitukvv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eegxtqxg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yfujjyie.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2slnxjowv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ripymfpv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jlaldzwm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pccyqsvv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ieakkwxj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pjnzfsed.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2shnrrppm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2druinfsz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2stuupdtp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzfmvgfo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xvfndbpn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dhcmgcwk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yfzbrbfh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2eyjsliyj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tyqwishk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nvfkmrjv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dvbbkxiw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sbsctifl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jwaawiim.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lwupmasc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vprxcagl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2stqxzzin.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sqhaxqri.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rphclozq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jpkvmegv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vsazrpxl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xdbbqden.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dwbxllpz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gkkeoqmm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2lrohexav.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tappkjpu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2yhinndma.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kfdhdafj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2gzjlrjqy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nxmrgsmw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2swfmaczd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zkoeczvq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cmdtfitk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lrejgcbe.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fooazech.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2cnwprtvr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2bgkemsja.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2nhvpycuk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wipoiruy.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zwbxzprp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2djbophhx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fxxlxqrq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pbaadkif.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bidhbkhm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bhbouytx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2iqkpbcec.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2shmkvfow.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cnlgzksw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iezwtpfe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vtemxarz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vrivhlqv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2tixrjmcy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ctkpneqb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ubeqptje.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2guvypaog.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ilgezmte.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nrbatlti.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vuzsyxua.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bxsscgks.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ccpqezzx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2efznexxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2lqirnkkl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ieaujzkq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2smyucxju.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zoaxrloj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnuahxti.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zviprwcl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2prdtmygq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xajzcqye.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qezieprc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jxfhfopu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2auoxhdts.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vvavkrcq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2taullwuw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2irqerwlu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ooexbkhy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rminsmpn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uindcpxr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2lkkjcava.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ieohwfdi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2oqkpyvsf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zbiheflg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rjpdbtfk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xcmysbsw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fdlrsmbm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2uhuvpdfu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tngxinoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qoyhssig.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mqnpsmpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkmuxwdw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jcphmpnq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2llpkjtdt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oywwddor.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ecadvspn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2funnjsvl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2otcjsnmo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hjyznuxn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjbbkeom.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ulgstaot.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2smhutkgt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2waoyorqc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ubkbmuvd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cadvvtsg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdppalea.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2glzycxam.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2zlubkhwp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vtrojcnv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gucxusis.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mxxkrbgx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nalckfxs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zwacjpnw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vfuznuwd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2sfkvfink.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2slircqgv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2equiohku.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2okayanfc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qgrorgcp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2blehrcsn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dqopzimn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tivognuq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yagnncss.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qopoaevy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ddplzeby.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kazoepvm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jcsbfkkg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2barglwpm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mfcfpymd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sripgqbb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmqywmqu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nuqijixt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lsqoblsm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wpjqlvlj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsispgsj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qhwohwga.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gyjfqfmp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pjdgznmc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gmejimob.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2detmuzlw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uoycikof.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xamphwwq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2bsfuxoai.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ickkakui.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fxildwte.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tkdqfbps.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2brkuhjqn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wtkebecz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hqupmygd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fwtimxqv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2awraxght.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yxvndvpk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2nynzqzrc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dksuzhgd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jsaulhhp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bwffrbjf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bdsqphrw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kluiaiqk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2awnoazwu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzjxjd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ontdnenp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2kchjbetx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dwadzcke.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mwttlyua.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rfbrfuwa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gkenuine.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2fvozbcsl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mnhjgvph.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gzaptnco.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ztoxfimf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tyqpjoef.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vnicijnr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2mpofuzaa.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dawdkgwz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gdtpqxgk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nfxpdeqt.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xiaulbwn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2itxxowev.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rxtrhaxm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lspkmabi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkvuqyap.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvlykvqp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yzhvxekd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2znnmimna.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ntiadfxo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ibbxcvdb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zbgemkbc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vdedfjnw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qqlbyzza.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2habikvkz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjrhbbwl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qaturzxi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2usasizag.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kysyayoq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2naguplcl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hbcwdkst.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ktgidopu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fbxupttf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2eebdvqbn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gwnywyec.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2inbackge.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zkgmortl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2eptqyxov.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ylhropgb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2opvvqikd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jkwyuhca.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2cqgoqrbd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gmrbpltc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2scrpvrvy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qexcball.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hpjyztlk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bskholvb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rvzlglac.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hplimhul.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ydgwqlsn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iuhiyjkf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gcrsvajm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zopojyss.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jjahcszw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2unwhcsiu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2owzfatxo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ibjsxpdg.html


<!-- 参考信息 -->