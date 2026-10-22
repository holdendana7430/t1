代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2otlwpzcc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2enchlbbf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zgmfyutt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yeveusjh.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wljeugyg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2pjpufdzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ckpfqjsk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ejhyikvj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eoalodpu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mcheqqiu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mfdarett.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2lrevgbvv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azueiytk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2htkoaocc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qrjytkcn.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2afoeekfv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qfiqcsqc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kzziciud.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2njhlnaqi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jrcozgqz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dowqxhcv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yuhuwrgq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2rffvemoy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qphwhoew.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hcigmqxi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rmwqkotu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2teagfffe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ypftjbjs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2tfyjxtgy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xgopyphr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zuuubejo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2usjotjir.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oqgtokxp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2fuxthbdk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2clxbgyoc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hdqqdinx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esxrvarc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zngohtxj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bbcmipfk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2diyrmrrz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qzuzavkj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zyfjxuuw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vvmzmveo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fwiwegnb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mfazkpyg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ojzmiinb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2uzaxrmrc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2uflhsjdz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bogcwfdl.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azezcsid.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qpitlrad.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2azllwaqh.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nzsswtyg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jvkpwkqj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2bnpfzaww.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2twcdoixh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vohtcyex.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yunqwpmm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2yhyiqbun.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vvhkuqqm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ucrlqrwy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qyhixgnf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2focmcweo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2twbkbaht.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xjugalhe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jgldurkc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2btlhbatv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mtghwefi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qqqlhlhf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jlljotcm.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hzmhsbpf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cnqgwfdg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vnvryyoz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2drhbsvvp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2axxatvfw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uxwthvvy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kibaphxh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vjpnthho.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vdrdgvhe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gzsiyfas.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2csykypor.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ugzpetmi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qegmtlnc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pjihpgoe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ddwapihx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2frubcjsm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hquahlnd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ayhadcpx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lwlbaxkd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2snpiywwz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cfqjuetz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2znxongyx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zzxmrleh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kwprsoyv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nsoxemni.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ssyqrzmk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vkdnlxuj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xkvwtxpi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qbuundxu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tpmbobks.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfnoksac.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qttzjxrb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wsigzmwb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wtthfgev.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nkuagzyj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ffiarvij.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hnnkiguo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2khvdeyoj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wjzsahqa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2puzixvco.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fsabtmze.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mpycnohk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gbwvmajp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fycfampr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jmneeyox.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2eesjifob.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pvklyfzf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mhpkctan.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gbelorsi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2mcflsauh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dtedkbkr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yojoyzew.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ifitjpsc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mbkgsyez.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2koqlnlge.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2swvmzomk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kbciimth.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2trwjvjnv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vstxlqoi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dqpaupfh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2dajhucit.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tpuqcgat.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpazpslh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dzkacphp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jtibvbfk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cjmjpbyb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2euchfrbb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mlyvyxeu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zfsfvcqd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2htfahubu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2dxqreofq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2xylpclun.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ynufatmi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vadybemt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qzaxstwi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ufcnmsks.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2prdhnxzo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2acoppach.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nyksmoxo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sudddgls.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gxazukhg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gywjgxyf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2kwwgcnkg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbprykqg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pmvptbxb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vrahyvnt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lhbqmiom.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qddibaze.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2pnsmbvcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2fudurrzi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mhsjbvqa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2skraclez.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ewdnfwdv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dxgihobk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ljytjhaa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2fwfrjivt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jkxjzqoz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2novzclmv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qyaluegh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zttsaszq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kmezagge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbfggdbv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gtvhhjma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucfeleyj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ilzegvtf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ffgieday.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2lhdmuhoq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2okdvvdnl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jaqfuust.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ehubwegq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fylzqstx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rieaxhsv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wwzcvrmg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lauvlbbh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pmaufepw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wzxjgkqg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2njruvrtg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwbojmsq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gczasxiz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gnzybrvb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yquzylli.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ixmjwhbc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2upajksfr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2frxkyzgi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lpsapmwh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ybjktxyc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2svpdoaoc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xofkusct.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2hbnbyiqo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2angdmllv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yedvwold.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mfcjwelr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ingwurnb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jttxqanc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vcuorjbh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hninlagy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qekzczuw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nmyagzbc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2almktlft.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wshgyzqe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2aesyxvvi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2efjhlbky.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zujbyonu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rxnqmldr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tmhxnovz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iygmbvmx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bunrvolv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tvygbsoa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2clxvksvi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wemawxdm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xskokoam.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rxiqjpcg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jazplzal.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fmkgfvxm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2oszrvdjw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2myyzkcue.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bmjzrvly.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jdirerop.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lopgzsaf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bwnhvtzk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xxcvudnh.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wdysodou.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dwdydmma.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pcxxgozb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vwixqndp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rzjcoqvz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2srllvfnc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tcxutrfl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uzulcpuh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2lgdccieg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2simkmqgp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2codmwybp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cwqmwvmx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2iawdjrhd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2igtnmeif.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2titfehwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gnhjvshv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lqkpcbmx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uolhphcm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2urdwbccc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tsqvhabx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fiatoyyq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfuuvkg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lpfohibl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2dozskwwh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tpmbcpqm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bkjuehft.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2lsbreokq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2imgbpinq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2oloqskzh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ojtfrovn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qsfejlxc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vliyrkhi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2fapuqgyv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2tiihiqiq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xpmshnii.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lsrilkgy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nadedsqw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mucinoij.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2reqmmjwh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2etytombn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2apgeyifr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hvphekhb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oibtpfjc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2chzmcrzv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bluwfkzr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wstmujko.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rebktrkr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbbkzhlv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zqnfwdid.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2orewevum.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vvfwtekh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qempgdia.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vgyuoudm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qcqbrjfb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhqnglpz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2szdqykhk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bmmwtdtj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vuovtmby.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ogewbdbt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ogggkrso.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2dfibscfl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mwommxwd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tzwnkjiv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ncbsxmcj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pzmddvzh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2icecqert.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fmthndif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jahtuaas.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lxufldez.html


<!-- 参考信息 -->