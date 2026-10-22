代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2grueeqyl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bfvnindz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bxxvxliq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2slpwhcpk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2tqbhdvbs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2svsmizid.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tmmmyjnh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2oqqxpjmi.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mukwevng.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ssyyfvsz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwqpklrv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hzptgvve.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwscdigi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ycqvkdrh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2udvopmxq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2rmmerhhk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2egakdpzk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mriloiqe.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kqrxtvrb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2xihortji.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qwpoymso.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bxbmoqaf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2praeiqvx.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cakkhzde.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2irfululf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2luugdmjb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxghddti.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2wiyucbcw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2rjnxrbcl.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2erxigham.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgnafyky.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cwaczixo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxlngzan.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kfvbioql.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sdhuloyr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mawemehr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ekhoubxn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2grwrtvlx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kaexyamq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tohmfexm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwdazbd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmpuaomo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mzoakukp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2edouzlnp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hloolpcd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lcfsrhpt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qkxyozhq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qgnpsxbu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dajptnso.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ebirufle.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2plodrydb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2icrrqdjb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2chhotrjb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rpjbekms.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ooakhmxi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aezjrbux.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2oearyckk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wetgwhyv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wxsgyxvk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fxirlbhy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2coucpfuq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ciwzxsth.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2lzdlmguj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uinzsefv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wqhpqgdp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wjddmxic.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yqlbykoi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2thhuimwc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pelwsori.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2juyiusjf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qrwmvoxw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2skgvfmwf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ybyzcgzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2votylzza.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kjyxdzvc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kasufmns.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vxbkomzs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yjrofoso.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ujydouly.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wvgkwdho.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hyqugcyf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qhssydah.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2angfoqpp.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2eornehow.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qvgpypof.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kdfbhbwi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tzgpgqpp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yagrouee.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2reyvbhql.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2nzfhaqmj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qxlnikgi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yyqlnpnj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cqgfzopr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nlalyscq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cqlmllnj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rlmpbjat.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ymtdhzvh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iqdptxsc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2iowpekqe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xcioludm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvekevcf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2igewyfyl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fxrmfitb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nzmkwhbw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mihwlcxx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fjchzayj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ilyocxbs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pmkslzxb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kgpynsgc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2txugevcl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2niirfglh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2prbxjqqk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qgzppvnm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jerygdyq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mtlwlmqc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2yonrftjj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2skirnrgm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2nhesqsei.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uuvwfghf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2sakhhnxh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lrkcnwpu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ngvpyfzz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2lgdryxyl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2stewyszr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnodoyqk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kcnskclo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2byxxwtmy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jcsabdzb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwsgwvtt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2lncttyrg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oyktfylt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2kmcsnjri.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spipocvs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hlwhltrx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jhzymlbt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qvpxwept.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dnhfcqwf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2slotswol.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wcrqntgm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ohvybitl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2plimsbpv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2qbnjuqdc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2copegbqe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mtqfciad.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xxpihvyq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bxokjppe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ejkzmodu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cgonhpjs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cveixyrz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvgodilj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pkqkziom.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hpqtjlpy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cvvdeyjj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pcbnuxfx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2peydmxtt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikngszvj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vxbmiohi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gommefsc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bqffwvtg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dnizluec.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hcvistxn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2hgofexil.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mfrapyrj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bvqcunnf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2psrkbfvo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2effcpwyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2joqneeme.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oeojmtzy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2suaatjag.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2shfxclbq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kwbellge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjludkrl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yhvjlors.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwtiqyvt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fohrrqey.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2whibtttz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ygfljgzo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2olubfxmk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2yknovlkn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jibbpzmv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yovztgll.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2cwjabtsh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2opdbxyzh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rswjkbba.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqvsapmb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bxonbhsf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwtbbsru.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2scqlghzl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jfzhehyh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydixlbvx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rdpczvpz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2acrbkjrr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ujvubqnf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2sarvzvxn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2haasdtkx.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2hxzdjpza.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2puetyaiv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2owefgrvm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2crdsomrm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ehzcumle.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kwmorvnd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzvkdbna.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2knfsocoi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hehmvwwo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2evuvasjd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nfaqawpu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ubpakdbr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yuvpklro.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ogpbuwik.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nfxhdyfv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jfefllkp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ikehpvdr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yuxfnwqg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gbrevoqb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zdbbpndg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftudlmjo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ijeeqgzh.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ixrpzgib.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bcaexixt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qebqbtjv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzjxtiez.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2awevpjtb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2vxtjxbxh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2twoyabqg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tsnxionn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2krmwxdko.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wnugcppv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2coitcbez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nhlismmr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cfvzxszr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zbxcsnio.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2rpiuydtt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tbixjqgd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zlcqsafx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2whrnviqr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqgbnqpq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vwfkpknt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kdzkhovx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mbsyvlla.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwcpqngi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isfvcpii.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vcjlnczw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fwwistvw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ezjjjzxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2puptpxum.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2abtrcdlr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vmnpcqqm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hrijgdoz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fzioirhg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tcavdief.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2esurlapp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fgdvgmht.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2erwxtdqy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qtueaveg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ejagtfwh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ljneeeet.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gxrovpar.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zaagwmqr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nmhxlakl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rzwpbihn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qkjpdefx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qixscyoi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2swcgdjwv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2umrwuprj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2adoxkmfj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ayaolvso.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2acrapaxu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xfbzfpgo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2iutndqkt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xnpnkyvu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2eavfsyhy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vsycyykv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jxskbeck.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2lgvzwnzb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oydveqnj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xlecddqs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mcyudnet.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qdhyaorn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lvuaeinp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rerguags.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ebidkfrx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ylkrlcpg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yccbqnfs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2glwivnid.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dchawcyu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2emsjbkbn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2stlfnbfm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2vawqzpjh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vfxfqcij.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ftbjkmyr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lzgnbjkk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gusshenv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rubrocnz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hltlvzte.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ctvbavrw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ubvgxyzf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zbaiztuf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kvdubagk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2zxwimsbh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2pnqjnsla.html


<!-- 参考信息 -->