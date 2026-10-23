代发 wailian999

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jihlcnim.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aboeidci.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqpxtosn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jwrgefmx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wonqzeei.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3mpujgjmy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bcwejqnw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3cjdvxzai.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3clgmlozr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dacdvhhp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bnbzpmme.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lebwbkhg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fjbvtmih.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3semqifmm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gfqxavhp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zsxnpajj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3sgspzkge.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vqmwutbw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asiwlhqf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3oajnafly.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vmefzrcb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3xbtdkpug.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttcpncpf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3xvetbqeh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gwifaaey.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ugcjjkcw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uykegqha.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xmrglnvj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xogncbta.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3wxzzmlqb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sdthqabg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cavnscqy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ijjmrtom.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sxbrrcev.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pifcmkep.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3efxkjgkd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3npixgtiy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vwetumrv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3mqjaqavg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3wlhwqoka.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ymfzupyk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3olfnigpt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lqzaaltn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qccxalqy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxucaayo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vgthlmqd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jcpzpqez.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mnqptsbq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3eefcclrv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3duesgwwu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nrndeebo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rhfkncnq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rnmdafhz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ykrnucau.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3laurlqff.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3qtorjvfn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wymefiev.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vgzmmzlw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dzjltysd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ebgqobmp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hpgtbsep.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vuyxwnds.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hfpmhmbv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wnrgboak.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zdoqqmzj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3oihibrzv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qfjjqwbv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jcplkpkm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3cvkwwnbp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3edlibrhd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvqglkfl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nikefvij.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lqcjdvkk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vyewibxh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xtiacaal.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fmgrvmgh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3egforzij.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qfebxniz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3glsbzspn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3svtooxmb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kvkdipmv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vfbetqqk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qyryocqw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3qsytkrpv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3smqdoukc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rqyfithc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3viauzjrw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3tjzcqomt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3podoiani.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cqumudvj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3klluzxgo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ainrukow.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zsggpplm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3psofdabn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jotfuivx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3oltuqdsp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iquzjodv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3skvmilxv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ytffqroe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lynxpqub.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sakolizr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijognnkz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rqvvsfcz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jxlahllf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3caqplwyu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lhefmume.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3okfmgzvp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3uprdvhws.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wymnwdwa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3unmmicdn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dcawsnwq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3uyempian.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zajsjthy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3cpmkthwm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fryianae.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ugkqedxg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nfwefyne.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3bnfrxixt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3stvfmyel.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ciwutvkz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nugtgsja.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lnhdbloh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3lnucnxwu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dhsawnee.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3behfkmzm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cwnzvgjq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fqmpkwnd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3qrqjakdp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3clojchqm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tzusooep.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qqmgbwbd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3oozdnjnh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nqkfwgrl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3gxgghsde.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tskhbxno.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ikophrfr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gqhgpqcj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tzyelkbe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gdqxxijv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nudqbwwu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pkhiivqj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jovkcqgx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vlnegnyz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqmsqhsd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dnvfwnlb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwlegpde.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3angsyhqg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovvyzvza.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3omumavlv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xagjqmou.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hnydxybr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hysvrkbr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3njkotijp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qkrwtuqd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3woyrmwfy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3alivrlkp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjefwx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nruqdefp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kypwmnmy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ezhdutlp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nvuqtorf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dybltrqw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3yirwwdos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjxabxxw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rkhcimlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjwdnces.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bydvtdxu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hpepewop.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xukepslc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jbqkwkae.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bueimfai.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3riedfpue.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tminkypa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qpodezmb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tdzsbkjv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lfkjeupt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3svqhulli.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fuwhxbvc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3guoobote.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uhxpetav.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zvmmwomt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lhqundqf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3earxdvhw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sorxgqoq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mtoaisje.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rswpgswq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uqtobdgd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3amqxwqfy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xtbvszxn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3njhqcyzi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rfkjpqee.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ilurqvdk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fzaksvhg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3paadmmay.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xvdjdzqf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3awfkzqyi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bohviacj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kcrpdygm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3inxhrawt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wsgjeqkt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ldiulrvb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hkilgtya.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ladbxinf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ygwwctrh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rlvicfwb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dbojpizi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wqtvonfc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ebuhejcc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rofkbgww.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hunzkwvz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3whecotqd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fmysziyu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ixrsbixf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3edbtuded.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lulwsfre.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lncmvzjx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bgaxnmpz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3badudlnq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fqtjmnvq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3otjcudyx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lnxezbeu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3itnzrsbj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nyguhqhu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3voqqvnwd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3zbognuxv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bqpbcyfk.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tvohsiwg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cymppsag.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wnxwkxhq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yxsjjdtd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3aotjncja.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qealthqt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3enorosto.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yeprdjve.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qqmryhur.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mluzltch.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3aqcfwyiw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fvirlpcm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rlwzmoxw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3icefolfk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3smcavczt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vtvtblso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ytovmiwd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojchmeqa.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3azhgybjf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3msihetgh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vaziecya.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3dciaaohn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vtmfshvi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qtpkoljl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3tspwsptw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lornmscm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tlckzwiv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3wiuloceg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lresxbxo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwvfderi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3swvzwpgg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ffniatao.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vtzlwudc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gvgnzicl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ovtvgpta.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jnfylsbp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pdophevo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lgwdvith.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ofsaacyq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kabdutxi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3olfmgpkh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hchaydwf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qjxkveup.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gwsqyspa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wdzxhlos.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kxggwavi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tgpzfajg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3efgrkusb.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3aasdzdbb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uindazbe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wzuybnyl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbsvlerl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3quwlszhb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ndjgvzao.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3eegrparx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ahcgzbud.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uhibhkid.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ponkrqgq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bpxzwyfh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ictzxisk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3yjaettjd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jkmydriq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wzbngtha.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3guxqmvax.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ntdidpvv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rapcsbjr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ikbmtail.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vfbsyteh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vlqeltyx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3govlhxgt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tymeghoz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qrdbbabw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3yoouqxis.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ppzxtqic.html


<!-- 参考信息 -->