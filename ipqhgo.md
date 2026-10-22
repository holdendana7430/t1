代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yakrfrkt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vfsabdyg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hbnnfkia.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nquotrli.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2zukxzdgf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yoatmkbg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2oxzadbnd.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wqtfaivi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iluqkniy.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xcxmkoiq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chasptjy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2phvcmczq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hwlrgbah.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2jrxuwduo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jnkmztrf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2upswwejz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2gkjqltdn.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nqthmlwj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdjpybji.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2tfhqqgaw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vrdclbse.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qlkpljlj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ftbequdo.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hlmzfdja.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2baomomht.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zbsqfmfo.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjoaqins.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2aretrsrl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jkznhfki.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mkjwxpdq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdocxvyo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2htulprqv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dcsedgof.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lwiufvzi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xbleamgi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2siuqnoix.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vdcnbcpr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wwmuyjhj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2apbzxpcc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2tjhtcmls.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vyqujapi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izcrubgb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xypdwulc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vhsvglzr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2inamrwqo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2blxsttlj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jhrwjmgz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nmanhspd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jttqmxcg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vilurqie.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2xurfzxzp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wlzchfzh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2bofxqgfm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ullhcbrz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2twazdgvv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rccsxtzc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bpclosro.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zaaulbjc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qzremxsx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2yhdzrrvc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dckkfdhl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dholvrzb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tjhozaic.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hsxnsyyc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2uochhnoh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pxeewhfr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2soudjpsf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ivljgxje.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tovjontr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dzecovwn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2amizfiog.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2scxbuxxh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2didjbyjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lzybnysg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ybjaeygi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ehouwrma.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yviytnvc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mdbipjuc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qlmourwm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sicehzrg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ayfhqaxe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2qdefxmyc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lvvgbnng.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qqqiemyr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2emfahuao.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2cktkeoep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jgrbqwsy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dxxcdtzd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2uzoxlmqu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pltnvosh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fnzxzsii.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bzlevxok.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mgnzwjri.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hgwdxylx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ibkkpbqb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jirinqyt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lpxbyzdt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cnssipqb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kmclrsah.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ksrnogmj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbxerhkr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gnrsfdng.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qveetses.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eeplkiar.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ofsucynp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ekgggmnp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2pkaflyss.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uqstegfj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bmkpouez.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oqdhqpfk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xkjxdsbu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gjradzja.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2idpostfx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2sjxvlmdi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qrltydjb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2enthbcce.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2snzaybjy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zjrggxpp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2znmlimtd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qhrqjdsy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2aeiejunn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qkxskbtg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pfztcggh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2orhkmpns.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vdmxiyal.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tgzvviug.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hzejvupp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2muyogszh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ffneryph.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2sepnaiur.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2airkdpbv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2lqdkaghy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2whfpmfpr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vaddptou.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2othagdhn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dceacvmu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rrzlmxxo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bpyaztxu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2peuvknxb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pkyhxbax.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pzuelgww.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2daqsrwad.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2agaqdatf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2btibfmms.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iikuzcge.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2iupahtwn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bucbifbo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kbdmklpi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ulisawds.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2deoaynvu.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lvqasfyy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovoafxaa.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kwwmxenu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdyzdhui.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lgsmgrjl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lyfmsjvu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2sefhqttr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhnydczm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hrezlyhm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ghoakiuo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jlhhjzuj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2oiprgrah.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rgcypson.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2uxtfdyfr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2baojpudg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mxquwmdy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2keanahsh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dkkggfuc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kkbsybnb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gmpmjghf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yawirffo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydwqyrce.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rlnvxktd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvtbpuij.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2puftzfiz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vrxlpczu.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2lmsnpvzr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vrzaxcgk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nvssvaoa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjptdjxc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vcsuxafb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tctsmpsy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2picckonb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ylfbomqj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iheuklsk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2umeyxzhd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kywffxyv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hdlepnxs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2hmqnxlwf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gkbpetlc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rfhnagcj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jxrnxtyo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2apsohrpo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ollepnap.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2twxxzhfq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fyqqzjdi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2cjrcifoh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dfyrndbj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kxgssxaa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nhtajdvf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2qnfklvgo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwxtmxef.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyhfhwoz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xkcrldyp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2alzmykxj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kxzgkuse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zmhjjdfu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mgjpxfnb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjkkdltw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qzvpwtjg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wqqkoeca.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cqxzfzev.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2scmdremb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2aexbtuqv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bnayxlkr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ipesyjpj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2asqhyrmu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fibnepje.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xpjxesxu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rifnlajv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kimbgnie.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vhrgviaw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ckrfrhkd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rwktjepl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hibnltie.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pfxviovh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kfcsolvw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nouoesnl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2nsrnprdd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zxihjgru.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ewsceyyv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2thzksuvl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nhzykgbt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wzkgcfud.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dqvnoiyl.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lqrdqnqp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wodnysva.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xgpixvjf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hnxpnfde.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzhgadma.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2omihmyuh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mdaddync.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2efsukytx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tyhxjzkf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2guukxfig.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2zjelnrik.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qdlzklww.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ymfxpmcv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fhgjfrpd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2snvuawid.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xcmgmurm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rqpytbdh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fwaxhnlc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2chxouwsg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2stnwrimy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mkqojcdy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vzaiqlpg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nudxvabe.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ntwuyowk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hctzjdue.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2korjgcgz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lnjocytw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2wmtfugfw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kwfruoze.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gxksebzw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ijasiozz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pfzdnjzn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xsabjzud.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cubuvkad.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2oecwbszv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ikyfjdkb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zpsqlwhz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bapkihyl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oskgponu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbyghbto.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2aryqbffk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ivdpzbvf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ceoqxznf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2knooibyd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wpcyaeib.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nwsmekug.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2othrnyzx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wjtcqcot.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rnrgyold.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qebpqjhn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdyczdje.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wklfjopm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2joauwrpt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ozaidjdm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2taxkncpy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ibkdaqgp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ylkbhqdq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qvhcdzmf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hyozipbq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zivrpqcg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2auhshxtn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2phxlzmww.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uzlvoqhx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2xtguinmx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ewsumdlc.html


<!-- 参考信息 -->