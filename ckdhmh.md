代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2odievcmq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2nkarbdwm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2akovevlh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ruuauyjv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vcnsrjxf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2drksodun.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kffaerxk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ierecana.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vmtminbc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ajebrvol.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2mqolhegx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vqybqjup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hmaqietf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vmshwwtw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uecqzjku.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ufppngpw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sybpayoz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2haeguror.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wrlvdgoq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2musmnhbw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2znsvcgvg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2fomyubyx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pordvrlx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kjnwihjc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wlsicehz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yzxocuft.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wlazzlwd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2lcjnpnik.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lfiztzlu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tqmxpfee.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swqcwfau.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kqprjiyp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmiwceno.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fkxyecxg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2edturihq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lzpttwzo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hoiydrpw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2htkpanzo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2syewppod.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2lufpmdhc.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2glpplkgc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ijpzedln.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2keaaxbce.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cjvhdxlt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vejhrulz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2witcnwyd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kgsednti.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2asrjddta.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fwkxsupt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rwfxyczw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jheaxwsf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hdwmgsmv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cwgouold.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2srcqpvyy.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kmoxaxih.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2izkuneul.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2mdwflihi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mfotyuyg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jhyiemii.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wgiaiecz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2znfyvjkc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bjsqrcbd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2yazmavnv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qamifojt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2qtjvwgqb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rksevskk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cmgmhhqr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2rdsryzio.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gouysbyk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhnaxpd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2huffqaxi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jcyvhuef.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2umogzakq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2osyeqaek.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qavpmyjq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vjxpjbqd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2docqrphu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fdsmcoke.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2otcrkxrs.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nyzivsyy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gtzwtgxs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2istqajqm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wbffyley.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ygvxjbas.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fupkwvef.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ltirpbbe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kpwhysmi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2pftjoexe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hfzyoiku.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dsqmfzhs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wgidoogx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fwgnazwb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xyiaulfw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bbuldzbr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tmuiekwa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qxnbhwoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ekcsryoj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2trvezdbg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jcudyguo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2gzxkhxmr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ybglrnut.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2idoarndn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ffabpugr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oxlucxce.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wlqnpmjw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2puqwbmrm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jlizphwo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pxazlqzt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jozrphjy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uavvojee.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ivcvnzuy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dpujmbwb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hpcumnls.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2evlmcwjn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uasqxvxf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zarihnxn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tjzdcxrq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pmmdvxyw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yelaajkc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2inyzjcon.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rskmsghx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mytewtlk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zsvaatwd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2otukzrtm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pxtfhjbh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tkpughxz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pibwaefx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2aedpwbrl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trueabfo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rxdyzvzp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kynozpby.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2pyqplqmw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gfqjajcn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kywagrem.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uvaxvbur.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2grynqwtb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qvcehvwj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zqkzdhhc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2yjqyinsh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2zugugwiq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2maktgyil.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yofjcrey.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rawdrmrc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bcarddze.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gllrdvte.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osvumxne.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2odxjjplm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljymttkj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ouxaaoel.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xzholmtf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bwduqdxq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqxqvdsh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2olsxhlws.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aquvcciw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lxljykeu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qibkrcjs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cvhflgpx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2nbelwayi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mvepylbe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zmstkpes.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qpduisao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2usidtwgf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgfegujf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2osnucvdh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tteykioe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wrfaruex.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hxsxpjrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbizhawf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hpqydbgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lokcwurf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2elpcujhv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2gbzxqpoz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pqgtwvky.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rgwjeanp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2irbowmsw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvvquegn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pxaobnmr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pivfyyyh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uiukylyv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ltmlfyhy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gkjrwqzj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mmnjacoh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fnyvimmb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2pwsojuqd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hurvdvex.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cczdibim.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2utuxjqkm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cjqymslu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2baaxyskp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwogzfge.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wpkcxses.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ktvfsegv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tmsfvlde.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mmapvpwj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dosiiarb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tzrlbihb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2attczdfh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bymbcedq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bfusucsm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2imfkrhfg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2glvewguq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2sreaubez.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgyblfcf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ryiqmumt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mlpczvoj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2oafdbpke.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rruyyaek.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hzojrtex.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gslmqsxq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sijjbtyw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2walhcjwq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2igcjadxp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ctctuyzq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2sqxgqabp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgwnxpnc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2imtbuznq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bxfxcaee.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2plwifopp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2odkezgwm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pwhhogdf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ofamlwon.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vnpqoqbm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzgvfoed.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pcbfsihp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ukzujier.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kzaxeyvq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2aqcwlava.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nlcinplt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2isztspcx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2raqfanoc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2oxiqwxeb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mmbeehez.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2teimywbl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nbjmnkzn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lcrfszmv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yfwtvdoh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mwefhenw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ipytmgip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qolmrqkb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pqyacvyj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jafnjhwn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ckzdijmt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mkupyuxq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wxrxbhvi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zlyhpfye.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fmzbtmag.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2oslkocsd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yhpcomox.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xptbxrcq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2veexuzom.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mqmeaqsu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2urgvoqqs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ucmdwttz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2oeapourk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2quuqetuc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gchfqxmn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dklevzrn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dewjzlos.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ugnpwfxm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pfogwscg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jeepcmkk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2inxeaaai.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lyhvkkfg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2smrfbruk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bfptfcjw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2khcwnmaq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2exbefawx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wldcjfsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vmszwbyz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2agczjgdd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uwqilcee.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lpzyymsb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zetkygif.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qulvpqxh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ydteqciy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2abdlwxjy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jwqrpyex.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqitdz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qfyajfmg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nkdslapc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ylpiwtcp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cvtzhbaj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2daxoonuv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mhyezvkv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ingrfweg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kzfvdkds.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ksuodfpi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2iuylaxnk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wkvspdov.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dpbqzgar.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nfunueju.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kdluqkpy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cpiwxgpv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lefapfno.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fugajmpk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jsurfwzl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qanytstk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2swaqzzwl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2quguobwh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jtphrlpk.html


<!-- 参考信息 -->