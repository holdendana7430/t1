代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2llvuiyko.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kqxhfrtk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vpxmkcfp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2gwbpikxc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spoklowb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oycvejck.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rhislzst.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pjxwzozj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aeuaxvkx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lmpagpbi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eovuvwtg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fatjpyns.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yhdfrxnq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gxbrcajh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lqjbcoja.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2eojgleds.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2azkxauzq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jnczzxni.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ertozgmc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2uwavcdlt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ckkqyrgf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2jeswlgog.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yoviatpq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2olwjffgg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mkosrcmm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pqgvqimj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fbyfvtuz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2vtabimwk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xxpiykes.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kadvwyig.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2apnolxua.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2njescsbk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vfqltqhg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hfzboyrf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2nftarthl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2emroqsep.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mwnscgxz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2uutfzudc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xerrebor.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2klmjbzfv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zsajpzvl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2usevisgc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2thxsrsdo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zqovrbow.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jyfkdqcw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2myyhxobi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2rpgzhijf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2iexmglat.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wuagxfrc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ddqgrsrl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kmfhlybi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kfybygrt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hqfgbfam.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2zcuhoyex.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ghqptyad.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fploelpl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2impoztdn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2kmzusiit.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kbkpinly.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2eperukzi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2hvxopuwo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dhdjzgcc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2acjvrthn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2idbtvcpa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2awsbpnmg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hgpyhrbw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2yurfcatt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zweqfdgu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2acdavlgq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2stqwlbqj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uvjmpkmq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2scmsqgmq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dltbnuxs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2puqndxft.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bhsshkod.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qhpabymm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rhszxyxm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2efjqiken.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2gesgtoxx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pzeljmwp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ebosxkde.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ebfehmjd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cyamqokc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2piwimypw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nzsoyykr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nzncvroh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2isefdwiv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2eypoemic.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2igtgimcn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2alszqzkx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2topypmhs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gdoxpryw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pbbzxzod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lkhzepje.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zvlwifah.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qlkaunnp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2plokkrzl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fcmjfejs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2crcxepnv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2snaqmzfg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2umpyvmbu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2codussoq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ruhmajun.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2twpnknxf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrqxyodm.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mxsderzk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2stnpsbbv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zlqxlipw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2onzlfdzb.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wjioriuo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ouibezio.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xuyvicwl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rmlfkqjk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2approxhn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ylberqoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lynhyhmc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2opnxnhwf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mbuoazjh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mnaoavfp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2awcrbdme.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oomvkjxg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rizrqtac.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfyuzeap.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vawdghrd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2orixczkf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bhsbjsul.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2csflkdqu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qktjusse.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2podhyxen.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kdpquouk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mhlhjlvo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhkzfya.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yatojqtp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jccmaxhm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2lwxynqcc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ryfrfcqh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wtwsrszi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tqqjqpns.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pojpzlnp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bpcajoji.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tgjuyxls.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2krgforbv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2uwaxasbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwipahwg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fkoazeft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgdasmrk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ctqlrtyp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2amjllwlj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2obttfvee.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2oxrtupxw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jnyxahot.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2phctcdel.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cafzsmiy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2opekytdw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ubimawce.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tcuuqdmm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2etxtjzsg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ymzwanlt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vguytogo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2scqmdohg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rksdfgqr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2flyhmfue.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nzeuyscr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lfljyyon.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ptyysmef.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tsgloaes.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vzhxvzxz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zlnwhgga.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2nontnofu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lysxkwaf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hkazankn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mdcvuoye.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xukavmhh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zoyysejb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kvntrhpa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vbxaeiqf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2skfqqkne.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2sjvzvbnq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ygmlvgfb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfikmnkq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nqiueysy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2vgouyvlf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mbporawi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2unujmoyr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jwcozumu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yxclplpd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ancyozws.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wixdolmo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jyinkomj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tskoedll.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wbvhjcma.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ujsfsctw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwecbgas.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2quznaddx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbpgwdtr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2haevakob.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qqmsbiyy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qvcwmcil.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bprrueku.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qummpunq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tkgtprvv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2dzmfauab.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ucvhasnu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bmcmfhzz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kggerhbt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2texhrbem.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uecsqldk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fiwvqapg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2npvyqwbi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lwmqjmdl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2btmowuld.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2iwvnwvld.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmntsxqk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vsxttweg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kxnjczdn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2indfamtf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zwmoofpp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rmwfzpru.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jhdcngiv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zemiezve.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lrmtdkpw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2edltpytv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fnzmzcvh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ncglkzem.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eenlyywu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tiltykaa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dhjlvice.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ernriokv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pzzgxqcu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2malycqal.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lgpnvgcd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ouucpwyu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ugxpdnkn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hjmnqjbm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2txzbakml.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xeknuorb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ivwvxipp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bkpjewlm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fuctdvih.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2olpyvtop.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gocymebr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pczofcuq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hzaglqpz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2agfydnnq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydbsvkzr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mqdfwwcn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmcoofni.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lfdgqnwn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2kytvytmb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2meewkucs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2drmltuar.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2oerhvxhl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pvnzoafb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vceudxzq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2odnpmnpt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sqizrpdh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vfnhdhcs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2yvkyqepx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgqixdpv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wmplgmib.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yubbrggr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2edjevkxm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pmmotxeu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hgnwunqk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sauslyfk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lcrjiggr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hkkyojul.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qrdjpsls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2awfzfrjj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fcwmkaom.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gnwbzjza.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2alnqleuv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lpejmhpf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2mddphstp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qdfxokim.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2wlxamlsa.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hhiufpgk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mcbtejmm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2awmamudk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wmetrhyn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ehukbwez.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ktiagixl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sexrztko.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cqicbbeq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ppkjooaw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ujhtyobv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hrmpfxoa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lwhowpqx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ymphvmug.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2moorwatt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ztzpkyrx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wcfdezmb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gtedlill.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ugdpxjfw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ymwncifu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nwzadhvi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mxuepjca.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ljrxyhls.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kndweuls.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gsbmjaon.html


<!-- 参考信息 -->