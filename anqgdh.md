代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tuhakcwi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fwycbdhs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gdmmtglm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wkcdwyse.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fiofhutv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rsxuekkf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aephppxx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3qgvghohz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ycruwqyf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3laeyfgtp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vbkxhjyt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mapdnqrc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3buyjclqi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lyoffxus.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rahouyvt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3inuyxbxb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bjremlwm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dipiemuf.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3wxnidrqk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rxzyrtmo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uqpxufmh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dwcblodg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tieapxzr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3oqjcyxrv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3npohyfkl.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3gigzxphu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3syjyorrf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3mkhoniex.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3atcfglcc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fomgadrh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3nejvfpyu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3kmulcqoy.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ivekryak.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3somcolgf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zuvysxyh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xdgdqcam.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cvaytbpz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rvykbjlf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wnxplvxi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zdsjowou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qthfntuw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3leuichrb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vbmvieea.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3mwioosne.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3myhfckdk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcahayc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3egqfqufn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3auzjepzs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3luklpbio.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3skoczypp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3whqlbpcb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sddgeudm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mgwsxgzt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yludqcgf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rykewodp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3anvbmcxb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bcvknhyq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rrjyaylc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3aeomclkc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3joekiipt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3letghoid.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zkbakbnw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3uxmwwlte.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bcdpspyr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sxgqjxfs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rtvuazpo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gddzbhxh.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3dptxgofj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3llgxsczf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3legegrum.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3baaowbct.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ofcdrlbd.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sgrfewue.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3blimswcb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rzjnwikw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nhkihelp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3lxatqrnz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vchuqwhl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fnvzjvoa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3urbmlvgi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ilznhmsb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hpqmbaze.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3trgmhuqv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fbieyxuy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xaipraho.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jpryrosg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wnqwdqby.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xugttdhz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zuxgvedt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iznklypq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dysaowgx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3eodgwsyt.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dfaeznin.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3mkyrwoin.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lusxznlp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kickmblm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lsmwzjvm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jqpsxyhv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xxsmbtpw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3eabpdcri.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ooorifgh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oxchslsw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3afoxkxcj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3jsglcqeb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hcbuqhaf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3jmsxmpcu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lgiqcfvr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jnywyclz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rcqmrbkk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bqtjsyzp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zcafbrqj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hdasnfnh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dzpeewwq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xzsazasz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jbdwohdv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ylmucwzh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lhcjfyio.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urazntce.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mesryzzn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qvwaijjc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pwttstls.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufmjytos.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fecdbysd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qyxjzboi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jxvvgqvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vfllbadf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3sgujmcjh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rbhiebua.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bwdsvgoe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3lalyivkr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imtgfbqm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mooanevp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lwchsjla.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jvhpgetx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3vrdufive.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlzhwkgj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qvcqgonj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovemqmxw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tdudyjmf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nirukhjl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3jajmphzw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrsuii.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3lleflmph.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3enudawpf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3sjowunqh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3eevnrznn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hicfmseh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3iaafqrxk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3heykjpwf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qntvhisa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3udelcznu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfihccsu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dmctwitl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qtpowxnk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gfinrhqn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3suoxrhom.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mkvziukp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3igrxqvco.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3czukwkse.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3mcahqcvr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ggsbeifo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3etwvsfxr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3iilifgib.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qhwxdodo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rftjkfjt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfilyisi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vnlfuzsm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cfnloxrv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3svybxzaz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lrqloqdq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zhkbdntg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vlpsjmjh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3fcudzmxz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bekthqsx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hjuizhfc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jzdqqxju.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3emntxfwh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hvskgmmd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ucbrfaah.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3emccwijv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwbyxlab.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3povlnooc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qhflwxdy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hntazvkw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oftzjfcd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bspkxmia.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wzrrksgz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dihbaufa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ijqzmjkd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pwksvvbx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3glnyjqup.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vezqnsnk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pyfxvfld.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbmfbcph.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3aepdgfhp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3naahdlyt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cwiurwme.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cjupctyh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gwvbbgch.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3snmpcrbk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3gboeennb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zqsslist.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jduaulmt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rsoebihb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ykwbwhhv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3slfwzvic.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3musuickx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3upuqmkwr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3nfvmaril.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kwptzpqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tklvrtuu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nizwwigk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rswzazdg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3aqclklql.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cwbvcdrv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bsplupsk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwcndxrz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3kvmiwyea.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fdpltafw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3wzkfarhd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bfhkowvd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jtwjdpsm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3cbgzdnop.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3agnmeqha.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oxmiphun.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nrhcfank.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myfmmrpz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3yfiajtof.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3srsvrjcq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gpwkqkca.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hopzrzgk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3stvxvzsc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kfhqwntj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3mdzzjnfq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3khuklguj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vobyodbs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qcsvqmai.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3huiohhqt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ptreblzj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zhhtjwnm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kiwvhmrc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3zryrvdja.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wuqwgsnz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hgkuoydn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3woxsfpmd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vuzuqdkh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ewoksezq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zlscrkdl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3otvsbtpa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3frmmslek.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ilivgezu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bvjapcpp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dbqvpgni.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bxubisgj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pwjemurl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lqwonajs.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cnbvkynv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hclzvjnw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hrjmjnqn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ycbhyyxl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kxvxkvhx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rofktcui.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kmhpycsm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yaixdsqh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3souarhtt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lwmestba.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nmdjbqcb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gssxqwpq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3roylzpcu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3sgehsqkc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3spjthzov.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vetujhfu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3pneezldq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yefunoik.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3iaytavaf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3aqmfxlej.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nhrfmttb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bpwuewmb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3stjgkzgk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3eenvmtdg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3carghpdc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xjdgnion.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ypqdrczq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvbsdfcu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3chvavhzv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tzdarswa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwjxkdix.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nnjrsrmd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jzgjaqom.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dphlkswm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3esgmdxfy.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3vnexxdop.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mdsamyce.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ifsnmaxg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cnwjypml.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3trpvqqqj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ctlrdgrg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3toroakmh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zumlmeoj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3uqdnrjfx.html


<!-- 参考信息 -->