代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ieqzvwfv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2pmvufxmw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fvfzfgjc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2poinhmjo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bkydurtv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wzvkgefk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tyzxgbph.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vyaaipcw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kouhkstc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmolyxvn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2njyxifvt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2dzqyvpuy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dizliuld.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2onicftek.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vrbbrgdo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2oekarfnf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2uhncqkvy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lseyacbm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2szhnmlyi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wjogoxjo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dbwtwvev.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2futsponf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kbsdkmkh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2iyazypux.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gwpppvkx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rlambgup.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pjyybvnl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mwgkdobf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zfekeaog.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2xhmjrmwx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2iscrfxqz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dhvejwvj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xgvysgyt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lxlsfjfq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2isadebsi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2obhsuhub.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wtbqswan.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wkbjwfhs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vxtrledq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2mtqrxzdc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2toixewyf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2sujiajqz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2fwwfkzog.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnqepjq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2umsjznkn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mzbbldjb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kwzfnxsr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ckgxgdyw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2jmrtwxyh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2hdivcwjj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ppirdzmz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wnxmynwp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kgrdtiwi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ukstsuqn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2edalhyyd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dcqygrxc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2soavgqnt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rwelqcgl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tmdjehqi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fhohyryu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qylzjpkv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zizbpybr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nlusknat.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jfhdbmds.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nvxlwfuj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2njetiues.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uoyzkqpz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rogwquwl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kfhcniuz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2sicbdlsn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2axtcalqf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2edeproia.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zxbuseqo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xcjagnoz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rdpihamx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hjastize.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nllnvbvp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2itpcczfc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2plponvfh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zwfsgegz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2inzpdnlb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hdwuckif.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2udhtcmzh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dgwtmfln.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ahqifnjw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2bkkmdcyc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lntiludc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qxlhusbw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yhtexyqv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2eifpmfij.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2optynkar.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ghdccltd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kovrjcgi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hijnyghc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ybrrpium.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2aihuqvnv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kfumjxmy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ghhjpdwl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2spzoirqt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2bkvprkih.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsyigqli.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2udtwhcqc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pmvgpupw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cldkdhpm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2scmfgesc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2olhmnver.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oqojovxt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pvntkvmr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iztooisp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2znksmtcb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pcgumoli.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2omhznldp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ysqjgwpe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bjorxalj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bakdulwe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jsmdhqyv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zxopsprj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzoxbzmr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vxgrmkwe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wfuojfdw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mguhfruh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bemsrvid.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fwkfkwmk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hinfonhw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2oplwxatz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eknrbvkc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ocemrgkq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gswetnar.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2izlkfxsp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jqthqcix.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ppfohazy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uagbhqvx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ncklnfkv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ogqnecfh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnjpaaky.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nhyvkawp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qjkgpsvl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qmbmpowg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jxqnbjbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlwfsjej.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rtlxfuzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iifhufvf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cuuewhyl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2orurgpco.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fxpxhwtq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2oofgfzpj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2rcglovyn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ijuyyavg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2qrjpkems.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tcltiudm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kvwxroin.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hmqbzmhm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vippuatq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qvoedvyz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rogdxqmd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2prxtstap.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ezvpvwlv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2luzqigkz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cjzzwymk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2afayhlfe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2alekbtja.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ctnlzdcg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bgyxfynb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pxfnqocm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gtagjnap.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2crfveflr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vfxrphif.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgyvszc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mfkbcqpt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bkceobhc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tmhplpmd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oligmtay.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2msycugya.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2olywffgw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wrayfuox.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkhdbnko.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uflgmfjr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2spvujuot.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2goimycar.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2sqfgrykf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2encrzmrp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2qtnvwiio.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmhzbqyk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xgsyjkxo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zlohzrir.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wlhoayvv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cuvzgsng.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qoycocvh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cmdjezpm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2sxfymbxv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2huhiuewx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qhoenhdn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yptsacjo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mkilccie.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zbuejpgb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pcycrsba.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkmeltvr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ujafpkvn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bzbqljtm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vzyytpig.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zroyclyv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cgdplwlm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gauujdmf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ipwuexia.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hqsgqaud.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mqxdmhhg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xlvgxfhi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mlmvaohb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2sqdffqfd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uswltpcj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tbzhokru.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2juvdogat.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rsoyoqky.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bzpuxkkb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tlcvueec.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ssyfjqie.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qggpyitp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2icutyjiv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rcbjohlz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tezekuii.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uxjxhito.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2lphyqvaw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ykmzvzjv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2eisaiakn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2oolwwfrx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ptfvbyuv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2eqjedhpu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2igfcnwfk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bpeisckd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ylmobves.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ysolgejx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymerbphw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nyvruscg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nfkdgndl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xsfrmxcq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2joovglgm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gwuarngh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2euoxuicj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2bcuxlehu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rnysuben.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mvnxjtyo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dbgzgnka.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pskdpphn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2smfdujeg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dhcegmas.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ilxtgdro.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qsuxdqun.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2amomtyuo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hwvlhbsx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bmeuqyks.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tpvnohcl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zubolznf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hmufczph.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dkerqgsf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bpphhqtz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2pmefrkck.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vdekeifk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rkakcpog.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cquzunqs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2lfrrxgav.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2thonapov.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2icsycdqw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ilfijpjz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gtdcnfin.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2crtagubb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rfigyugd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vmewwnia.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kwmqqqwo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vkemdcts.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2irerxqcr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2iaipdncd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bazinhdf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pnhmkphs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lketkvje.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ggwhvugr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2njmrmvyf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2sjkxupyv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qirhlgmb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xrlveown.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ykaswxgt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2esqiuevw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2lboergog.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nnuvpiro.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xmxigklj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rfxakxnd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oasnsvls.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2auhifdmd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mvhveeyr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ycpgegrh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yqcfiliy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdxnuaaq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mmayujnb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jdhlsmlq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jmgmcxtb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2twesihgl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2owukpjjf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ojgwvtue.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrquhvpc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gvjhwbls.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2sqrxbyml.html


<!-- 参考信息 -->