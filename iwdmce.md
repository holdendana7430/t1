代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xcgewgvv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2yufxphgt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2dvwqtnom.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2woxlnesk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ijcejdos.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ibgqbtlo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwokbwmj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rgmjtxzn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ophyxpct.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ewqlhnzc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kruruiax.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2blnrzflp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hdcupxua.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2kanoiehf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdywjyl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ufopbyfb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lwqxdwth.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pipjskiv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xfyypwyk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2puhmgeyq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2xclzbcuf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ssxjjrae.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhnxnhmo.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2oxseyhhm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pktglqlg.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zpyojtmu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2matjmumx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2bvpnamow.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwewahdi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bxceytji.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qlplqwiu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nkrzqctn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pzmvokzr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wsvwlptj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hqqdxyos.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kvzbgkef.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ektfkino.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llxynxdb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fcbudsad.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2moavaknn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pyemnzbn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bjnlqrom.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hiahagvy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2jjfxmtgf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ksmsdtzk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2liuusbde.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fntuwmud.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aboyrpgp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2iznegmao.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tqtngltu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yfkppzuf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2irgmbtad.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2zqogirov.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xzrxhvny.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rwzwrmsf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2djwhdvne.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2beqxxhzr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rkmzfmjc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kgeicqpx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2uezrgvjv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ztynhfhr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2pkaajqor.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2raajoght.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2afqxvokv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qxzikevh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qntrdeew.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2qavgszjh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2prufzpkv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qdcwkhaa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2sltrrimr.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2osmokyhk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sbbwptag.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dvsdnght.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qvcalgxy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qqaiweou.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjepawe.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jeqzxvvj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bxceodnp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qqyocrpo.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yingxwzm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vvbbjkcd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jwysfhzc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rpghnxnp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2czhicisb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kovxacli.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2dipnvzpo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fhvdhjuo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ifwclwbq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wwkbxzha.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xznubrso.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ybxrozfd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xcnaqqbz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ugqvwkob.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2eoxqeuxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pqhikjhg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2nmbuowvh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwifqclr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wsigjqtx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ctohtbqu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pptoppcu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ypwswzwn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2sidbtroj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xqftcdca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ptrjxxvn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2efgcgsxj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eklatsxv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hrlbllel.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lkgaxiio.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dtautaae.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zskvnyqz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vtpxjbnb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zmpeakrx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2shztuwid.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xpzocjqn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jacwjchl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lcixnwqm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fuvgfidd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ftgzlaqj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2oepqdcmg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrlrdaum.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ahnqhdvb.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2milgswql.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ljvxvexd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2imokjcil.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kkvewicu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2sfpesgtb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jdptaonc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uyafnsxc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eprusjud.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pfedgkps.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mqgxtlwu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lxavwwfw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fpahtkzk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hewbkbyh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2djgedbxw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lpiovdcz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2awzvzjea.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2noqeggms.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2jskyhugp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2peeopqmi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ajdkhnln.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2mozenbdg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hgligkji.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ipngmftf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tgszmsnu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dtionvlb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zpyukukn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kuftjzee.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gfsxfseo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unwynmit.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2yfvgferg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2putkfvpn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2utcaotyu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjhmjxag.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2equtsfgk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zbxnerkt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vkrlprqh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gzglwnmi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ewonxwum.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2putuvbcz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2buiyimhu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lnioyykl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ensueibu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cuakpzla.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kdvpzfpv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2czfjwroy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2nxrwdomj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyypbtsu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fsdeetbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oeqkyfqo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2etfxelgy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ioulpypa.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gqnisjcv.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2yxtejrvt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cooxelwp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xwarcqkd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2irlekbdy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2nipyavnl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yyqjwpkr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2uwpakmzk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2elvqtgzd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nkpssyjp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2djdvycko.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzofunvj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2socqlafs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbxdtate.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2takqyrjr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ccrodviz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dktywakw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uyepiaxg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qsaeazwj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2iyqiksyp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2amedjcnj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tphkrdqd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2feehanjq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2alsnbjbn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pazcfzsu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhhjwsof.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hglvqgds.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kseudefp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ioypsjwu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ldjktnps.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2btpsanun.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mpjjlsrq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2usucjhkl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nkeprkhc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2guevuvjy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ozgbjfva.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2khitgjbj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2axcdbtui.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2barlpimz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eafcuwth.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2daiamuox.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2bkxpafbt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpkeftgh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2flzscoyj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bivjwmcf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2syiwmbby.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2spzqidtq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nffygckp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xydilqxm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gxcycsle.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xjmswqqi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wjqrnkti.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jlkhngwz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ywdgkczt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2twzvgdrm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2daoqvzgt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iemwokzj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2myjanpwc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2yjvekply.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bghccndu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2bifbpbpx.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ecjnfkhh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ipdjzpuh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yjupbqnu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xajahync.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mkuitutp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2asdfzori.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2rhuglkxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uikndqlm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mfufjyqs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ppoyfhog.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vvervjit.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kganjsol.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nntuoved.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ewkjyknd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rfenweho.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2cwlzscaa.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2oetvyjmb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hhsqjoqm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwbvko.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xikhrphm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fbpvkbpk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tmtynzfy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rdyaalvn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gyfvgjtg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mlpeuphc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkqeawsx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2tguzrjgi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2umykmbqg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2okruvqel.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sylnvuob.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rhdmcdcu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rdgzvuez.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gmkxqptq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rhfossht.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejtxmfxz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jabqvqxw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vrtvllyp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qbgmtbzw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2xanzxwxm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lqhnzkcp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2epkbuucu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bmnyjijt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ewbkwohz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vmpkxyfb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nzexbmzj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hisufcgb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2prwdmlxt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2prxescom.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2piyaabuc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rpkfnrnl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kiwwogec.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2anuprncb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sdddteag.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jfkthecj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xyenaand.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qlvhqddu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2turkmzcj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kxwxrfvm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eklzcznt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2snwpmsky.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2arsdmqhx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hfirqygu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2plymibax.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ifxdqtwc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lqlxyxqa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lhazcjyb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wckpwkss.html


<!-- 参考信息 -->