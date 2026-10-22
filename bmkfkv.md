代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2frmjztey.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2sxnvqcvg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2abunysel.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hqpeljoj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2lnqzzbnc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rrkibnlz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dqhasfxt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pqafalfh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2chzwylai.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2aqjztouz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2izeajsmk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hgchvbmj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hxdeccze.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2eruhnxdc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ebhkrbfx.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2umfxyhho.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrwcgunq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lmfkumgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sraqbeff.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2peksuamv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zagmunpq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zgjzmpli.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pptsjlpp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2clvbbmlz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ncatralp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asxmhcfq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vuviqogn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cfixhrwr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2juvsyjak.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2twomylaw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2etzyiquw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nntpdtxm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xcbcisxt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qzwlgjcd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zagcfxkf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uetqgnfk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yegofwdh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cdlhpids.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2odhocadp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dlkfntib.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pjpyobiq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhhpfk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ntzvhesb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vgjshugq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zihjrafg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oskfcpzg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ztkrdemw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qnryhzbu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2wqkndrhz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qnqhlrvw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hczzjqgh.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ujvlwpke.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pcgofmwv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zcymlrrz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ibhpxtxa.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2sltflxnl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bqgaldxy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2egxegkxm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2qfdcpunj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2loprpxxd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2jewhbmeh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pnjijpkz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pkdbvgve.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qklhxidv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hxpmygkr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yftrqukx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fbdpfdfm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rydkadlh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oucwfpxw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2awkcnblx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vzufofxw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2elcxzesh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dnropaka.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ypjkufcg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pytdrrgt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2jmciwcce.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2acqppjit.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2tslafbtn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2vknbvckl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rktgxepg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ukwdmqql.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uficjgwq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hhujanig.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dgsrxiar.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zarblene.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2okjknvit.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zzwvnadz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qpjxzsyr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fdusznvg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qiyhwdvw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yfurzebm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yneneixp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mzvvhvdc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ysjhyioe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tkxqtkqq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iacupmti.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2smubazev.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zuyfgfdw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yongbjlp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2bqzopnwj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zketuuha.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hlttjfie.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dbjlqfco.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2eubucwcf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mkgbdyik.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cjdqzbhp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yzhbedha.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qqhmbvgn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ydhfhjyo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vsxybqxh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yiupwnbs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bwpytyyd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ygcnkxbe.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vygafvpe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2bdyfictq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2itzdumdg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bggryrom.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xctgoojv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ifjsaazs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yccthwtz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qfaboigh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zwihuhgj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rskwieot.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2lzuwmjko.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2nghpjzkz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cdoctceb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kwbhbvpy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kuvlhhfx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qrhrjugj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jcnbyyce.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rieqgpwq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2atftompu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cmqlnhpp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rzlmlagn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wvgzrfpr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ywfmluar.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2kdnijrss.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nsqjmqgh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gjcxwqoi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgawplwm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fievxroa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjiraofo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gmyhfygb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ujehzpsl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vomkphuu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qolcyfsh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kytvhgeq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hflvxiac.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wwvlwqzz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rileynmq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xqjrbang.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pvmdlmld.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2atxcnmdj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2oyaknaby.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2monckfpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvhbecdw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mjqnfsjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szffijfv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cmlzlvdk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ehmbxrnl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2iiiqrdfa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dhxjmegs.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dcsrnazv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2njltfclg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2fmwljror.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ldzetcha.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vckkttsl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tbzuoqzy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ybviltbi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2angfoitv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxetzxkb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2enffqgjt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2dfnptgev.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oypnxhqi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jspmdzlq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qafykpzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tdqsogkb.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bhplqjte.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pwcqehht.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uobwuffe.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2lygkuufq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vyjbrloo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vyiisuji.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2towgkjod.html

esac
来源：http://www.52xcode.cn/Article/details/gt2uzitcwsm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2awwwzwvq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgqkmxau.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cxupupkx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ysocppqv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qrwdkjil.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fbkdhqjn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2txrlbyej.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wbkfngya.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2smhxiyhn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cmcqooph.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2abqbbnsc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwgqaovh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ikvhxknr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2phiqvayg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bmzvwxob.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hqjbtuty.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2knyfdovp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kbvjryad.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2glyogsnz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2flcunbvr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ryzzkrhm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2eqfqnqwo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hyezkocc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sgrtogox.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tjlnkiml.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vozejrkd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2japnegma.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xfmjokwo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ucgcstki.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jpcygsxm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fgqfwwob.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lonfwmeh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2bkxrdsvg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2llzmfiwr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnxdjiqg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ncftrnst.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2oynkgqto.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lrttqudr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jbsdiwdr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mynpryyg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mkffjnni.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vygfszsl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vwiakcaa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2vrnbrekl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2chautfms.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lnmiegym.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qvfufgog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2afvnamkd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qymdbwjk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hjlfnjne.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hwtgwbql.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqyvcxt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2hsdcbved.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2runxgxhw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cvvklbgf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2suturucq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2spcwrwcq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2annsxcgj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kqxtxjnh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lsrgrujt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2wbzkgazf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sdxhlius.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jivtqsfk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xycyvigk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jogmduwa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qwwamxge.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lsfoyvlp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jtunxbmv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fwtxizbs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sksfbpjo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oltqmkvr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jotndomr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2yvpzoccb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jthykkwo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wofljcqy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2chfrqzat.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2irqjznvc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xxstuynu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2goahnftx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2luqflber.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jogmdaef.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dlxpvkoz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2edbkfoak.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dxjzvrtb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqxjckgs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2elsrgvzn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qbbkphnb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2edydyvfk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ffxvdmty.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jewbjtep.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2nunxzmfy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jgzibmzi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lrejcbsz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rkrprwvn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yvqywujf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2facecwwp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tasapxec.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jhoufnkp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gfpxcszx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nkugsabo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffsgixwi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rdwqhzar.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mottwxxn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wobsaqpn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jtthyngx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dfeshifi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qynkrmqi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mcawmstj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2grlgupkl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jjnkrfhz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hhnwmlhs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yuowrcbx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jshzyaps.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2oidfitem.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2coptdugy.html


<!-- 参考信息 -->