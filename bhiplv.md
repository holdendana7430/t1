代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2egflzzml.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2uvronjcu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rnungfxm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pxayszsm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xvcjagiq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fdnuwste.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwwfsknl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mgnuchzt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hehvrmvx.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2yjppdgyu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2kfxztkvw.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2whldvqws.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2piiouocf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fxhvowwb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmsfbtpk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2vzleqsnb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ulrblxti.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xdoxxgpf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qozspowm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ebqmgsak.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mwqblfmp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vujetrmv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cjlxamgb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tptmgbqr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kmjilqjj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2czrwfrgg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nfsyofka.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xtnsxffk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xrxjreic.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywziknly.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tiwlaqge.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rusgobwy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zwewfirp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ekivixdm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2boxolyen.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2azqyawib.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2kdgvscmf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xebymzwy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zwxxrnmq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2glgeshbk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wbguphef.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uzllxvin.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fcltnkjp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fkuzqzyv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2dkenbwnr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fjoalrum.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rkldiqls.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zklybbbu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2oayeteub.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uzbxkbvn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fzeqhhlo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2qgvlsgtj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ndcvnxbt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ceryjufc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iyevcobm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jssopuip.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hixmiidn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ovxabtdr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2azigwtjb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tzcykaru.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lqfojpza.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xnlxrmqv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ixoqxpvw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uektjpma.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2dxtumqdd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zqkmyubv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cfbwtdjn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jfzootrm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gzeyiqtq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2euujgmpj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2owhhxfvq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2oavtpwab.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ubesnnoi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tomxgjex.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rgchteta.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rospojyu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jibagoaa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2droekehh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vpnviqhv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wrqlhlqn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xxncedkd.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2vwbhxmdf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lryxubhm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gmzuasef.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vyaodtys.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jvjjoqqk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qtlopmyj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ujfevfle.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hqlkgigw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mjyszpzm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sxxlbbgl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ugiqkrse.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ibwkadiz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2fmiuibsx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ifwupxje.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2izcpuyud.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2smgqeazo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wfddxebj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2iejhsynz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rcgsmuih.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wsiaswqt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qpogrorr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hjpspdpi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2pbkvkpgh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2tnusxntw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2urpettcl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jeerbgkv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2sqeckjvp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yvrqhgjn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mwpwkjmt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wopeneqg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zurlfnhd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2baiwbuli.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qgkhiezo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kbriogum.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ngnqlhdj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uczxwmwx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2edzpndgz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2derfmkzx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2zrcyskmm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esrruolv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2qtgmqcmq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jqwuhjzq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cyhcibpj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zwyxrbci.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jxihzxck.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dtxjprrs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jenblszi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jzccyrdb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jcxpmwdw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2okpsbzru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lnaprdcu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rpwlpxal.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2iyzzhllg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wyfgwboh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xxlzojlg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2knpslzst.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxjzvwoo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2szddwqxy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qendbumj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2sutdejtp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tarqvzmk.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qewfccev.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sebsuntm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uhhnpxff.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvnwrnpr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ktpzityq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ndjqzejk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ynspwqac.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2loqbtkba.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tcaqoisn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qcndnteq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tryimplm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2aeyccikg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cdebdldl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bsqtdsit.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2szfmhrvv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2rbbmujlc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wdcmllos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thnslqbv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lemnaszz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucwaajoo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2edpvtcwa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vnggpkkp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hprslkdn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2pnqupftl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rslqmzpz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oklrfaah.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2advlcehj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nvehtrog.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tpnnzdzf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xhudfwmw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jccxluoa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ahzjfpjs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2srsvsfpq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2kegayysm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2llelvvpk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vudmblof.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zaqqjvwc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2izrliaxh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sphvrgiq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nyzrlpmw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2altkwwjf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wtbillpm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dxdzpcdb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wksgspmy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2idxklgch.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uflkbadh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xphukexp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovqeiexw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rwtwrplo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kvhiztaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eyobupbm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2mrvmywvl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tupcgvpw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqeazinw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oilfkpkf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2famdcuyj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2agnpgxtf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nsneqatx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2iaozymue.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lkxesory.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vqbqdxjn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dpwwmkrh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2oszsiuqv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mohmejno.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2qiuvhfpn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oxvcjvml.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2hlvrursm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bjmstgju.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uaiqwujw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tccvkpil.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ygblpxwm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fwrthuea.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gprbejni.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hrznacku.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gvnlltao.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wknolttt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2mmlffhtr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2huycrywm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ectqxdvg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2zllcxdak.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hfkymnbc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nrcggmfa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2joxsqvkp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kadkohbv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lmswotvw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jcjlzxwc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hdequxvo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cbcxochk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jgdzcibw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yzyzjlah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qwufibct.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cipgitte.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kafgoabc.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2htjczvtn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mhdwizld.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2djicjels.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2udnuwxnv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ndnglyir.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2obbdlcon.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ssazbniw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rtcnhpmc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pwgcgjbj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tbkinlsa.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ffzaawih.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ptsiuwzs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aaamzdis.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qtgrsirf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bsssdife.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ozusxvjn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ctconcrm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2prkydowc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ejlcsgab.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2imawxyus.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2jdgjafnb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dphnuxcz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2obyaxbpb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mskakbzy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2rtsbkbch.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mbwyrsxf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cezwnbmt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kjuzcnwh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2otsoaoyk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2iosvqcyl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2uhxxauci.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zsmbzmik.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fosbnddy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2twwlabpv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mealopso.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ezcnzfqg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2aggazibv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fmbxzage.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpzrreuu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2piliodzr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ocztqidn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ldjvrimk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2whqxnrfq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lttqnibw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ixtyblut.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2icigabqg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2sefckwog.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ldhuarts.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fqlelhli.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2duuosexo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xkwnjiyo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cdcorxom.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ihxnioct.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ooixuodu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lqlsarrb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2unjxvfji.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2frjhktpg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rnumsxwt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kvrqyikm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tdrxdxpr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ynydaeig.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gvomyhth.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wzjlfyge.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lvjxovuw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2aemlylrz.html


<!-- 参考信息 -->