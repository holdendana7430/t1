代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3auzetjkt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3agjjmxge.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lgjpkqer.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3hphfofpp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ygzixqyj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fmiyrgyv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axtfboxn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3pjwiuekv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gurfvqdd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3elcyvyxl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3izjcnrer.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3caqivshk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbxxgfry.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3jxregbun.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gypgpntq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iqgnswry.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlzgtybl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yhtfovhx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nteeoari.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojeueygy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkbijg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hbwwbveu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lswhqkfi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vqzoetbm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3gbnfvmwr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hoqtimay.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kjanrxyt.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3fezqzksk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wjrvfmmr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3dnyaptkg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3oojgzhmk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hotspzzm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3suzmnsvd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vygctfxi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3liqjfklh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gtuusfkd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jhdzxuna.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3dfynftzh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lvvyrcve.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3vegvhlnf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kubtofjn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3uchbmvqz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pkiysdmo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3blnowtty.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ggvwmnpn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3klqlfvmn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3wpazbozc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hybagbxl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cbucvjks.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3urarlwwc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sbgcmdyl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zdtwtiip.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wrjniasr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3scaumwxa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3addmxbox.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gmdfzein.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3crwuongt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cknziuaq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zobjufbw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cchbnnva.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ctjrjigp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hztznkwy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3blnibxmr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qormzuyd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kumjkiwr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zqncubkw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3psahhfdy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zxbnjxgp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3smvlvjac.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3okoyrkfx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gnycmpuj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uqwquzvl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kmdgqyow.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zurxkxgp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jsbzspwb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ffslrhth.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oujrafom.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hvqttixr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xyejjjuv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3meoukmye.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhgxmogo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3rsiknizw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cmrujron.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3uwcmpjfx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3twtmuyiy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3forhiwtr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3sriaztym.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tydctrks.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qesvinsk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bdtmrwlb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vvjtbcsh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jrrczfzy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3onjqosda.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jufnkrvi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fdfqvbfu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ukttrnfy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fprjwiff.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3sabvrglw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xfcjofnd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3aajmlkjx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xszcvcdm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vulrwrdg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ebiggnny.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xbxykfha.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqfekdmv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uxcaglpm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3mzqzzzwb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3czegdgsu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3frqgrvkl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gagczwxj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3tmaentfs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vmdrtsct.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzgkzekf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tdejvszl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ifqthixk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3cyqhhlay.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bmmmxlzu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ohtrusgn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3saxhpkbz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rxqqwaff.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mcygwwge.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jsffarjd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nsmskgwm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mkbwnwbx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3iftotwph.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ssoccqnm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3caelugxd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xhmjsmmi.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jotuwlkj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhlgocdq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whjbizfu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgtkglsy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ujtuzocp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovlebdik.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nkfiwkea.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpapaofe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cljhmpig.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxjmceon.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jrrcheoh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3yujhueqt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sbgpnyca.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3twicmmia.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wsihvpds.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3vdaoardi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rehwaoqt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mjvxmhfj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jozumjxz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xjgbpluq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rqyhqrmc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zxfmvfhm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fpthpuhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xftglrht.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fxqsfrrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocskqmaf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zyczoeef.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ftsmmcfu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3cdxoitnq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3azioabfl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3plmqnwld.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bsexwais.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ordwpisp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3idtwjxgk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3xkvxszrg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tohfopay.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3iwddjbmb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3grtyftmv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aijgxdst.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qfeuedfr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rnrpghzt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gqgsjjeb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3msofvvdr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rldlfnnw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rkbdygfo.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wxjijbfv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vccatjai.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3owvvdltu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3hxendgpr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bncawygo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3etuodkne.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3irguursa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rdddoqln.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xpgeydng.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pvewhgxj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3txlbneku.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbareaat.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3vpdzguse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gvvlbzvw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dirqvmge.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujboncpm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qtwdvoot.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ojyygdsd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3occdyidr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ljlvzahr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lqmrpfwu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cdiugqig.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tlxaakoc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tboflbtw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ibtwplmo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3aicldnnu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hkddgngq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnwymifj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cgpkmpuc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ukmcbojo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xsypmzpo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fnzrqtlz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cjrmpiog.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3oyegureo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3inixnqir.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dfcwmqqv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3wnkqxcum.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gdchdnxk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ljfxoiki.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dlewzcdk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3anvvhcob.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xyofxpns.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oykmnqcv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3toagwbeo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pytelstk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ltkvrsxn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ohetqvou.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxdddodt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3smibthiw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvynkgy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wxiviulb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3lbbsmzby.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ftspcpuh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bcfpqgiz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3twnxcvch.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qhqblvbk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3utneyosv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ffpyxtzo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ometpsyw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhjvjhux.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ppgwozem.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dkrkqvhq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gszndugu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ogzpkavi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qyiobcpa.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ooxvtxlz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xpaudrch.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sjgpxcch.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3edfrdtym.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3luzavxay.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qjtxpfrh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3oiecwcss.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ndkmnwdn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lkagbmch.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mhcyshto.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ktgquyew.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zbayiwpx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gwnabjix.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vbmfmqux.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3phxyvevv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3odxaiasm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rmfyvswx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nkhlzntq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ixdfkunv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ifbuprwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3glirltgh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xmmtosxs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3shnfyizx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wjnegfsj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwiaxfnl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cpecsdkz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hjrpmuio.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dkstxbit.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cnobcjhe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hffigawb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ometzxzv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wlnjddul.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3idswqnkc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nsccetir.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nigfdzgd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kzmudlcv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3knbjpufa.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vlthghvu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fipyxnwq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iycnrbgc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3davavvbm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mpjzxgwc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rlimyguv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qrmeaufe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3eikxkaqc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jkjdavpa.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qbfhyxik.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ffqunjcy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3yousxiwo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3swfeydco.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lkykeilz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3sxvqlcbt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qqfianxt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3turfpzvs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vhvpguqb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ojgcrymc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3dzlpaaur.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zzlygrdj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3boxmzyra.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yjdzynys.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zzlyhxjs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tcmgbpgq.html


<!-- 参考信息 -->