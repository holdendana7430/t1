代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yjwewfgz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3gcuwerpy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3iugmzqhq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3doivnyij.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yremrpww.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3szmjqfus.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mjkgxoyv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gjvgolah.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ifwymjws.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sosntadt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ghxeinhb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3aoszoxnu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3sgwbbdjj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3euurawcu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3esfzqfyz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vuudfkzq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3vwxnolyt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3afbaqbce.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ytmvcxgj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ufquofjy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3jqrwwcdb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ucbmhhdo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wrzuosbq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hcxpouvx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3aimbnrdv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tsaupkgg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfjykguf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3oixusmbf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nylgnneb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yadlibzw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zefmaatc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jjqllvfr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dnjgdxhb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3msfjyfqk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ehdspkjk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nclpsyvc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lpkdeayt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lxiytrow.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3faiuoquk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mscezxjv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3rqkjodue.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ibqjfjki.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mkgqhvpz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fkyslhxa.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3iknqryqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vgbhmjam.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jvqecnnc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gdxgzadh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xeyeqsll.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uyyepgnb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jmflbxkk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nmagoluh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3waamxcxa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ngolkbva.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3guudyqra.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3szchxvwu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3wecsuweg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cxhyvyhw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gqzpquqz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pjiqbhfs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ewxgcguu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bsdgkwgr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ejwerjyy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kxbqihqx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ojqfccxg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nffigppn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qyiowdgz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3naabeqxh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pmxowohb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xhyjbpgz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dyxwgiar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3quwiiciz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3trajhjoj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3jotijjne.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pchxqfey.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3yupiyqcf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bvteeiwg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ezcuuyhn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3racvyqbs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hjsraaae.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3apkjpdjl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3amptqymv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3irifrmpc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wuzeyhfn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ofqgqgub.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3tjtxaafo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nfkyfwon.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ulnaxqfx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eqteutji.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3wuclklpd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dbkcudvh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qyigqzjf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lijkzzyj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cxombtjl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3mesygzyh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tozbzhnq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qilfdeyj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3dnreyzdu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3iznjvrbl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3crviusbo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ndvuxxgm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xcyumlkd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cquxjasq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3sgvhjvux.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fgbpmawq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rgzscgfi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ugeflpdu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3idlqjeew.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jrpcfkse.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rjrdbgpj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3potprlts.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vnrlpepa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3afxdcmur.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wsixsywz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fjhwitnh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3oxcoyyqh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3maxwborm.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3vuwxvyrl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdcozd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mggfqklx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3bvdsyftv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3rmgpvxus.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zzurxhrr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sdkpiypw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdumcqjb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3grbycucf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3uecxzynd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bcblbmrq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lemuozxs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jjrbiodf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pyeporib.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vyflbjqe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lnzfubrj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jonezvjq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lxrvfxwd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3gcdtowaj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wbiizzyz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ymowlawg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uurzhwrn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3inotlbjp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hhmxcgnl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hyurvgkl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dxsnltwu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kpdnljml.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nmzedopd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3trjbskcq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3guzlwhkz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3atqimqii.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zcaqnnhf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcrtrvyh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3payfrswq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kncerhyd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dfxcgkmh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqfahfzh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3byknnybp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3csxlyktu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cplkrdyt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zccxeojp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3byxoprxd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oltimjvw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ixehejel.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kurzrapf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rxyzcgsr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3esgcsdes.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3kdvjrfrk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zmnifelm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukjsafqf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oixwwbqe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pfhbqghg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ppbsjkkg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3avylojwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlgxvukn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gqqgauqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckwbpjso.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hefruyrk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3gbrmbbfd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hxzjbbdy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bwriksit.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3whkreubr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3elwolxqi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kvdblyrk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3etodpyvj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vmqnuozr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nawhmroi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mgckbxwo.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uwqguvev.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xeanylid.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bobrjcbc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vfwbxkkf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uqtvzbvt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gwvuluqj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3csvhbqir.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3vsdxkzbe.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ognzrpaz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3swtuacbz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cmdvexzd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vzyxsvqs.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dladahms.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cmgburzg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3excpwwoh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jwstcjas.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zzlrgmyu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3bnbijmpi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qefyshpv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jtmdeete.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jjdiymfr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wgbprbkm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqzcyomp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mtahxhsw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qojbxupx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3pqpwvdvu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3rbbojwzb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rnxikbxw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3trjcoorv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mpnvrmge.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iypitysg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zuyckofy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mesluama.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cydjsjaf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nszxlmlh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bcwgyayd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3paeebrkr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zogtzfog.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3anwpmztn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qbvpyhwo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ouqyflgr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqpxinwn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3djenbddu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3sqzbtcir.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zlmezmkg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3quooicgc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yrehetnx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3guvbtasi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aplqabpm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3begpnkfo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxruqikl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgnuitoa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uxegrnnw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3whlbjkpy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qsrqmlum.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utbkpydh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ggtnaauw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtgvkaqy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tgtdbehq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fwuavqcq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kgmrlrhz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mpoyalco.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3euiwurnp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3btjiahdv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ouvnogrt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qebcqtoe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3playrsck.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xbtfplag.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hsgotmwa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3auljsszn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3stwupwgu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gqsvjpcs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pwvmxtpi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yymbnttg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wwpstqzr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jjriknje.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cvivfadv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gkxiemxt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tlckecsi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ewyqsafi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pqdowybv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vzjcdmch.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ptfqzrwn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xdqfgpgm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ntqghrjm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3kklzuxwf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pnimwrqc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rxjqaqdi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qqdljbky.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3blzulahm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zdovnpbw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ffeettmu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3iryuhuom.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kapxljog.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ccotkhiw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jgdqkyzc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3yjcieatf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3trdhzjuw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wowvdtns.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vceuliii.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cficwerg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ndrefhtp.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qpdjvzid.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3amginjzi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3puldeyxm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3inczccid.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ivjtchwf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3yddhycmq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3settaqog.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ufdvupuj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3gxjrerva.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tkwjngjy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vedzimig.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rgashbya.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3klwirwab.html


<!-- 参考信息 -->