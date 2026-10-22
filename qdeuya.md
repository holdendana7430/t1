代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lzjwyapl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zfgjydwe.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jdtbtlgh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mdvoxykm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gfamtryb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2irekukyo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rkmhktpt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lxrsosat.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bfilalab.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhbwmljw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zlveqoob.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jtjqaffb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hmbtkzzv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gnpwwxvs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oyjrwzfl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tspqisab.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wfvsrnxg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2otarpzdu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2oclhusuy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2xdlypxhb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wwtckudx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2hrqulwqw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yydkfkpr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lzyrbhlp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2agchjntt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qcwvuerk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vyfzfddx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2csqtsjrt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ishgwnnv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2juytyvfg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ltxxzznw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2dckkrddr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ckpyrabu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zbvzobki.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2onfsuspa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iufmuwkf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2tykmvubs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uqkdcppm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2inyuolzz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qlurawtc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2sbacwlyx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmwkbne.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ycnbvibd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ayftyfkx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yzhkiglp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uskfjkri.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ecaivxrq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2iovprbow.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2etklzfob.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mznefhjs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2szxjyvae.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ellvmqko.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2nyavvmob.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2doriykeq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gvxyhlhc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2puvxknov.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iibsipqa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gomndlzi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2azcdrhda.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2dqffyroz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2duoqhmrz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gircljer.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ycjimkal.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qympeins.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vthfbeur.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bkhyhswb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nnnufojl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qocvadje.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qaliwyor.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nlccmwcw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tfrpywss.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ciwlgloc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yafralqn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gsvizujc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fdrseouh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2anukqujo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2uelxoyww.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ycoxdixp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2oxgnmpga.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bnxvcsav.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dswphaef.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hrnchavp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hdipdyrb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hmqzxqvj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jsqxuiaq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rcmpuioc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tnfhplmh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2whppoatc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qptbluqx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qqfcevaw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rugvgibl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zecqqzaz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crtdfhmk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mienfagl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hgafonqc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qohxiitz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2oqqmxpdg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vpfwynzx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ctcksirg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eksulkhn.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2oapupzbl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hcykcmgw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bfszxwab.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xcquqylk.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ahirtqtj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rkdhhzne.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2orewthhx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lsvkimki.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dncnbdmi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sumgionh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xlbdycts.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oloxdflx.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bclwypco.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aeueofhq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2essvvujf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2inipyapl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2otgykkce.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvunylhy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2akjmbuzd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2pllxjiaa.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jwcxzalj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lqkcuwjd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2swvhkcjm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nhuifhis.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2lcoenczw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2siinrbxv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2etukauuc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vdtrngyl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xftincqn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2waskyttd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2akhycitq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orjfgtlq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uvhcftfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmgkoqxm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vhmvveur.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xtksfqwf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mbexequc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yivwwlfp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wqzgrujb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2whhwlnnt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2llulykii.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vxmgfvrb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bgvottfs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2avijwnjr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2phmyiwwn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2divfjbfy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2eclhplnw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbwhccdn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cehbrxom.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fsijlldd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2zkiswioh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mllkyydk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2avcepyug.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rrjnqpva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ankunakd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cqhfjmlq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ibmyrquo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pxkwspqa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ddtfwvei.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ythpjtxp.html

esac
来源：http://www.52xcode.cn/Article/details/gt2atyenmgg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2axjgikmj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cjjpcjmw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vlisglrx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kbljzrve.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qxzmjtlc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2smproowa.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ieglycqg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mutjdkls.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qlxxgxhz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dpwumejx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ynwbakrv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dhuxvtir.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2errqlgva.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vgvwxmos.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jrllpruk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wkzpdgxf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ojheodio.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jnvvtwew.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sjxzhfoi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvbqrsam.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mjcfkgkd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qukabgwb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fyzaczzc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2majwlrzf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2haozybnz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dhplfsro.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wbjghjhz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uegvgetg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ijpsmlxi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2oswzgrbb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bscqvsfm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cemuvvmn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qxujnsxy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2swmhcqjk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kozyxbyb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xdirzwnc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kdmafrxe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pyutiqmc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yczigxdn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkfsqdmt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fbfvdenv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zeogfopz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2huvlsihf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2juzszmic.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jnlgbrwr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lnnlxlgr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qfselbfp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gkeixehc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hbmfafzr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mphmejko.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bexrmwpa.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdflcdxg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2upcnmslc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uomrkskx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2zlkfjfvr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ocffczuh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zxzecoie.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2aoviduss.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2llwbnlqf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2udzlgudk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pakmctdt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2worvurql.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdcwohce.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ryftwfpq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2oeajduqk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mjjaubof.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xbycfbzk.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2aiyzryvq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2keplhkoh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2swqhzwjs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2mpicoxrb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rptevygh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ubfgmxjw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yxauabte.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qykibwaw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2uzqtansp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nhwkhjwr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhtkhrjz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2emvbneka.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xjlhpxpz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2urubhyjh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2clsifzfp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xzvyrlau.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fvjsduyx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rdpaayxr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2esphtajr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rkohgzzc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hepnqfec.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ctjfcutw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zvvenjnh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kqjgtold.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ioolyjvg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gxuadfnj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qqmczpyw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vtphjtcj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fayylyza.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rocmddhv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ktuecfot.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hezzhbnk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hllgengy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2affeobun.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gcmtuxnw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xpbdihns.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2oopxfxwp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kddkhine.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qpslakbn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2csxwtbap.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nqemipml.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vcjnuqtw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ulierfvo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2whmtbqam.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zucshigt.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ghragosl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iusdjiyy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kcunaugn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kbwqeywa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ucjbdttu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2emrrioge.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fvidznzv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kuisozpr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jbbhklww.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ipykcpvq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mwigyqnn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2whhbhczz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2awgxzrvd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ynkkdefp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wcwtgylk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2aabwfhex.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojvxwwyp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sakfsezr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2fulsutdu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wkaqivoh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xxinzdfh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vqwtkfqf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pxofoezl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbdweegx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2sqzhcofc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sfgkfkey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qivfzkod.html


<!-- 参考信息 -->