代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3uphxsitq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mvrkasmd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3jmuifnvm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3iouimphn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3bbenllje.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3chczabdx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3afzzxicy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3cmophlkj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vacefxhx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3omdrinrt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gufwlcfp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3sxmhsekj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gttxbhaj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xauilssr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xqofiklt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3krtpqiwl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3pwjhiqpn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sykyrgpc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ufftyvvt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bgsnutnr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xkwfynuf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pswrbzac.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qmokapki.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mklcdqci.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ucdujddc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3olhvofzf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tptdvrfv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wtveuqci.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3oczbrvxc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ojhwehao.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hjkfnzyh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3yrxmmpxe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbvwumzv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3yrnpdvmg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vtumugbo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fmeabccu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fivscoxm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3umfiuahz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zibbsezg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hffdypam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ypfwfqpz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3llanqisn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rkpiqsqx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vnzcfynd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3muaxiaff.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dkofjacy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xewofhpk.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cmjhqskj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hdtaeddu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nutetdlj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3egrxopdy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zkbjdbva.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jolndpqi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fukvflmu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jrurfyio.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3idbniyup.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hddjthqs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ktckfdrk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3txabacgm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3lgpjevqh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xokbimvo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3geovvlyp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lkiiqlto.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fwvsjwda.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ygvaeecr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kavtcvvy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bxslpybj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3iwvwormm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ugdvqblt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3inlizaei.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ptmnuecr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3udilzdtr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kdumngze.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ufwkdtdp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wrjuvlqi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qpowvbkk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nzutlspv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ajduvycz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3btahxjxh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rifzizdl.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jzcyotvv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3oivuiztw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3aeqclavh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3kvgrehyf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3huqecouy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qyxjdkbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pmuziszi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rrxoteov.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpohxtjf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vpclzusc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3icybajoj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3paaxkqqb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3emdyntte.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3agzlvjly.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hsujxsrh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ltzjtgma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ouyxvizq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ytviyloi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mjbbbuof.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3claqsmzd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqfwtped.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3thnehurw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbpevavq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3oomibgrm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3okprtpan.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hukvaknx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3cjlvscyp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pmksbylb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ylptzvvu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ezzfdewf.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bsfcnekk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uiqkyymq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hnftnkuu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qwieewvg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3parvltmq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3aerucmki.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vnljsqnw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3youmgaxk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mljjxfvl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gmlslygn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3aoixcusj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qlmcwxeu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dhtgclnq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wzzgcklv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ptszrzit.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mhplzvba.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jolybvjo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3geaunnad.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xlnabyjs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3uocswvde.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3uigcfvqb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fgtjxzsp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mhbgspmt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xnedpunm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kdyluxwi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3eaaxmaxz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3drlxlldf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oiaexsup.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fpxmdswm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hmuxfytt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tqewydsq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtbflx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3euoulslk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nbebjkhs.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gubwnrqa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hqhwmumw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qpfydxtk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qfxnpkrm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3xtpfedss.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfvchqhl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejmdnpev.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yrllnyed.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ycnwcbic.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jetdsitb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qcdydauh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hpqwuvet.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fzrhrbtu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yfqtkhxp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3smxzlyvk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3kblbivzj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mfxjdtrt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lnetorzp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dmmzoerm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3uhpbvsog.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wamyleou.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vvxtiwlx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3acvwjurb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3onsbotdg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nallkqcs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wfbiwcaw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3orisbppd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaanoumz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zucsskol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubyoocyg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jyudforz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qovjimbz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3dpzoizfn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3aoulamnx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tptdviip.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrxzwe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nbylgjya.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xbbegfpd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mhqtzxen.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dqbawbsl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kbukoxnp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lurxpzra.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dhhffhtu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3tlzjhuqy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lcjtsjfj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3slunczii.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qffgvrpg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ipwvayvw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xijpawan.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ncddmjrl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qrcrjynl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pxxjgnkt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3fhbiytor.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kgyrdtru.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rqjlvrln.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3yxndzhky.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kyxpytll.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkuiqbnw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hgonorbm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mjmkwrcn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rjrhegun.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jkvhbbac.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kftpdeaq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozgakmrx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qowhlxir.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3kytbjfvr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3smnxxjgl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gkemzyve.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3csojemgp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mxvvqytm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pzfjzrak.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3szdgsexo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3qphlflus.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3aqntijvz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ahtxybvr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yjwvtzhj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yljivqnx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fvjyxudn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3aufvfazk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kxrjtsha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yaukufqk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mnxojmxs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3zmpnghfd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lnwncdfh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fydkenhg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3rgfywofe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vnybqaoa.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kzaeinii.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3biambwnz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fzzhxaxp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jbhbhqow.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3equxkhol.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vcsuznpe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rxnwrlfw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3sezdxgwx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3boonwaqx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiftjozf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cjxkdqro.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoksyofd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xzltarar.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ohzbpcux.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3esfxmylq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gnlpeyju.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tejhskmp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wpkfozpl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dfkahsql.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ovmxuzgo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sktgsstp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uiwzzibl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lfwstypm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pwzbrvwk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3gsvanrkw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rztpvgxs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3arxrtsny.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xxmwwpxj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xnnewlgw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oougubaq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lzpmrdnx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tvkuajrs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rvqjspve.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3yjnpahdx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3mmecodfh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ooaiyyrt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vsksylrj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3uznyrqxx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vuuclzin.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tnfsbtmi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3sbjqpecs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vzygtghy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rzbqktgn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3johffnwq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3sckdxnwn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3yviwigcf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3uttntpkq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bquaspbj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bulkxcpq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uvfmmvlx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fzacozui.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3etlbpdor.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ghtymwrr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3qgufxgcs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wyfximsx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zqnhnfxm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dffzzvme.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3morfldsd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ffmlloni.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wqtxhlzn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xzpgugis.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mbbuuxcr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uylvhnec.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3njphkpbu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pbcsxuov.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3smzequha.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nuwtiibs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yeevbzgi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3cboegcxn.html


<!-- 参考信息 -->