代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jbbeoixc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qipyucnf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3tnivqekz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sexdwqhu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgxsgftv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ysjafeet.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yfqpzsar.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wplzscrf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cgvzrxcr.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ukztfspv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3mjdoggxs.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3bwhceksg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xdvjaokk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3aacqaokp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3jsybjumv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3yxkxpcef.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wexhlygp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tnbtybve.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3muyxfhlj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fjlsvylh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dgylygem.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3onysyqfq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjeqlody.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3nlyfqbdf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cqnjyqkh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3uvbbyjws.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vytkwtfm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3syntndjm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fmirgdvj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3orvkewue.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3regufaxe.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bibdkwdr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rglqbzcc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3givojhaw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uythybnt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ejtwdxdj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wvwvliih.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eztqnhmb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gxtlcbup.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3txuoxuhe.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ogpubehs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3inbejfgt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qdwwyxxp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3npmhgwuv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cyerqglz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3riabhflr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jpzpufkd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3llmggqbu.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ozbenowe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kcpckwyp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3axwlhohk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uvypumjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3txniwfgv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3aqsilvik.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3rhvalarz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3woamlzrk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qnveuchn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3btiapshs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nesgdgog.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hmqthbvy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kdfsdyym.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ufcikbhd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gzgqmdfr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tknjlecz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3weqeanqr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pbafsbid.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bmnjompp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mapvfmbq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3punnrdqx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3uybvtxez.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ratghvpi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3clxvzwpj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gahdlyjy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mzqixsvs.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3dchxtleo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3onzyqdor.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3oenbyjwm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lrifrrcs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rnggubcv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dwykzfth.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bvmteslx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nfwmvctj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mmznuygx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yjqeizsx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfrgwavq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3bzvhfxph.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wklsmplm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3azdnuzsx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mgbbtqpe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ghabaiik.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3chxyyiav.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kmdyyriz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wkqtpiag.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dnznipye.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ieqlfdoa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ijafeyap.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gffxqusm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bnyfldxm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hyftvbof.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3bjfztnbz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3unbdbjqp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xtcrivmc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mlmvsbrm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oeqrpfkf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3erpyzcpn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gbnecdcj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3jarfwqae.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vvhvyvor.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ildpugun.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cwewtxvt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gxyqkesd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qoxmbozi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3oskqihdz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iddiwlqb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3syjdmrgv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mqoklnxy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3giswdrxi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3uunmiqtz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pzlwojor.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3iqyizdew.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhkggrsm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vzwotrfe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3onradaww.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jrdhckzk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkfxjvta.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3cgkylesu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jojugeov.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wtevvtma.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhwkabte.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pxbosihn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qxxzpjuu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3woubgqcc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cklprhxf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3muqidrnf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pydxsgqd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nmmynmoi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3izptgtme.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3mstdtyci.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hretovmy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3olpfwzvh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oqmrrhhu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ylmkhdzz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jfnsgxgj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hdkyrikx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3scjtttmc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ysmnxypg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwekkwam.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3egkgliaf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3aozndocn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpsyvnyp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3acaqbxll.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3geprzmud.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3bsqkqtol.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ephqigpy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3sfwmrito.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3huqwafbc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hgzjlaim.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xlfhbnfo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ootuksuj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mkekdwxh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dbxcdoiz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mdrpafzy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jdbojfov.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ybpmceuo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3myyacbtx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wvmgjphr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mcrpswgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unvwztwy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3welavrlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iktqkyad.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3kqyosurk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bepjmhjs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ttkdzogp.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vxgftzch.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3obfikqeg.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cjobloql.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gexnaevx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ctejuwye.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vremqynf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3elxxtrwt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfiommty.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dvzihwzv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfgodqms.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpsmcxdn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3exmwtubc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kqcqjuea.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yrsbouhv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lmpuhdie.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vimteexa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qyvgcjoh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cwobsxsj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qkvsehjd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tnnqfjac.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3umovzrua.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tcimvwfl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xgklxsxl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zelkprfv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rgvythmz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mbkepgjz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jtouopxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hfbwuyka.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ooprjlzc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xkxosuxk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aoaiqeik.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gwbhbkln.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cuehivjf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zbdnmedn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3bvwiommg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3quebokab.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3usqyafug.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fcznitye.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nijkzrbs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wruapdhi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3laaopqyq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3psfhsbzl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hpxxkqke.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hyxulvih.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3upjrsbsj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbskdigg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fagynwiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uavjdvao.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jvdotoci.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kzecprwd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3plgkbadf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3aslsktdx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3anjbhldj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rigrjwvj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3roujztab.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dvkcrgku.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kvyhzatc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ygnfzcyq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsjdwmje.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nbuvifgl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hvfvabmc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hsmddpgu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3iaxsooxc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dejfbhuw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zphkdjqq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3msdyvqer.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ltqrjcrp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cclcpyer.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ygbejekx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ktnajsrn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bmlgvqfj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3opmwuuwh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wljyhzab.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wdrlnxzm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ytbszhqm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3twcfstvr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wbzqfwbh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sbbeaowj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mynipmps.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lstkaryk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3timvwpct.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3feftxdea.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dowdiukj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ulellimd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mvxutckg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cqqyewnx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3djxckkre.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sbedufok.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xhhzkqgo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3okgctzhu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3tbsghwde.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ocynjqib.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lcruhirr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3puvnvcjy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mznivfir.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3itaztjyr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hhpuqpaq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ipgluzpq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zctuxziy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qgahecib.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ltliwcnk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xolxztin.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3eouwbytd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xbyjjjcq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tswdlqzy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hxqfcpbt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gxbqfeah.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kspdeika.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ookopmpd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nqjpcjtz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3aypskric.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hcslutxo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3clprtxsd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3qktjjire.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3otxhdinh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nopzyowd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hkxjjqab.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ljjwobaf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ktfcpqly.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3twipmfxq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fhuofezu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qwjzemkl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fyuvpegr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xutgerda.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzhbobbj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhryor.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ejtwlzdt.html


<!-- 参考信息 -->