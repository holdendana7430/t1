代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2udnmsgck.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nqurmwjj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gvxscztz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wjipwaju.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2gwnrukll.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jdwrbnmf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqusqthl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qhkwilys.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trzdioje.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lbwcppnl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lswnvgrt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hrrurcvo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srladhai.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rxifjzlh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vrcxrnjy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yvdidtei.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ohuqdxcz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2itzgmcss.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vofkmsek.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2idffvrkf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2wbddacrc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mxewvvnm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2niiomqmr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2govongzl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ccorvipo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fthvthyc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tspqeuhn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2eimgiopl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2trbnjpka.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxylmhik.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2klnivids.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2umygaeql.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rmytghms.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xlapawvr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hesazywb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xgfltdib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cwglsydn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ojgqkqmg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wfhzxkae.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xhdfjmvu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yidbkgbr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2nomdjvno.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jetqdamr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sevknudv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zukhhnge.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bgztufut.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2iczcyaup.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jjflpjwq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qymdunjx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ksbryybc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2smgecjcj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mbjueitq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bsfgrmnx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2etyxjqvv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fkanonfx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wksejjjj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ikfahgup.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yzuvkwhk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ohcoertv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rdgjtpzk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vkyraske.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vovzwwhe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cqzyoene.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pdkopcvq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhpffwhp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kravowjq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zqtpbtnn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gwjanaiy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ufynowdq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ckphqfny.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2lvwusfgu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jpgdolit.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wobqcsvd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cjkfwxyn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xlbgzcyz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ribyfzqa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smyvtckp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqozay.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jatcqeqf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hjbnllek.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lgvfcokr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ooeviwkb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iqsnmipf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2leyasnon.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jfqzfmxc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bxlgnhek.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qsuzfljt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wlymbbcu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2qbssbzbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cltxyyzo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2whhqgmwq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kubfpoyo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wpkilnqn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ogskgodp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nyjvkpli.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kneryeyv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2njgwhqqs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xyjpszqp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qhbqxaqp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2brwhgpxh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rdwreayu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mbbwaftr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ybnzobkp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cbtbpqij.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lejisuus.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jynuwdie.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fjahbhtl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rucjqqyz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aohcfnhm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2iauqhbve.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2iveggguq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fepjbodv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gpwvtbwr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pzijsfiy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2unltuoxj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vijnsoes.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mzskefym.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fbduvxum.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gmbewoew.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ssmoyxnj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yjyofogh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jjqqbqin.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ugyxujnp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2cehuhpaf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qphoksne.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xnaljqqq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xbsmgkok.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tqihcnmz.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bvzwsghl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajdouhma.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2znrsomme.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dyottpmp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jqajqgdx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brhpngxk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zidtcvex.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hhxiovqh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rtwiqpah.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bumdbccl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xvxmjjea.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vyipmoij.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2feqpgspz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2szltbrhy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rzvafhpz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ainpxjuk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2imbaakux.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tfsoxxnr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2nbkmabae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hadvffof.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2evhpdizd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afkufary.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2uppqumlr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kbogkzrq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vjueysvh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2otwevysa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2klyhruia.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucsiyuda.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qfqqylir.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2wnhjtpvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mkryewhn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qmxxaypz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lhaxiimf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lytndegq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aayehwar.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rtkhnchs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ugyuciyw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2aiyyknqi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jziyxieq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pzcvatvo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zdqkxraa.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ailhmcpn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2voyozxuz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rghrwnin.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2opoedeao.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ldoboxwe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2abdxjokm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yntapuug.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2glmrpphk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lfmtilrf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vgkydlrx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2elsbnesu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lxvywfqc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2bdikkoin.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xivjjbto.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tpfumgkb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bzekkbnc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wxfsphmm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qetrygtt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vkudyolz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2howelhvy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2iwjfojlg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bfeyhpaf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kvtdmxcj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2vnstkjbg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ucsyhpfs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sakmyzbq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ldnflcuv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2fqgxctyj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yfckzokz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xuyplmcq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gastrzbp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2szbmnfyp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ghjypptk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bpwlacgj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2flzilzrt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2okflubtw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2yyiourzm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2efcjnzqy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2usefuuve.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tmeldcmq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2maijlqnw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hgdtgzhv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2geolqfqb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zuvtshbo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nfoiyszg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lnskuxzx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcakcjek.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mepqukso.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2yptqzmep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2khhydjkh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ankkpkmx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mufjuaby.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pgsusomj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cieplaoe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dslkfebm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ydeiwoun.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2sfmbxnto.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2iutsemdw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2nzyevysm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ufeascjn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2rjijnarg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jaqbwgxq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wcvoqege.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gfbjoqzi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cndqvtks.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pfbmelip.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2czbwqvyh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wixzaefw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fwvwgspe.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zjrugyab.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mbnkofwg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tkzkvgux.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zulhlvlv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vldtpegk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2myddrpyt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xqxtlxap.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2txmnmkal.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vojzayqr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjhlpnbu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xpbozxcy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ovuymooe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hapkeqew.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sqzdrzjz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2esmyvzzp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2hunyhpzc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fzgamien.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dhinlaip.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jfenzewc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2chjnqcyg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkoupclb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2slmyhzky.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xfmusvjk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrjffgqe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2lqicivpz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rpqhxsjd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yirqqebu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ncebjgee.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hvzpqgcy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ksttmjzs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xwygckao.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bylybggd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zcytyebn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ntrgsmwe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sxtakyfh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wcaurulx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2agzgbopl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zvhguuhc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xwvnnfsi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2czbztkay.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kwmtueoc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jtuqrese.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2opwxqena.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jgvycvhi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2obyhlsmq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2guscqrhs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2vqymcpwd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ciydslfs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gztfwmzb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xswuzhfn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2npwlkhka.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fpfqpiiv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wqbaxjkh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2oncrlqxl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2syydqjat.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rdgsbxml.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tyjbpwms.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wpwcxsrg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2suujqhsz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qpgrxoft.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uzdcisow.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xvqksjzo.html


<!-- 参考信息 -->