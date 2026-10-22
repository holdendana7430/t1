代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2vdmxshwp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mtaqnltf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hhpjlbsa.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bnaxngdw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uqsnouzw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pcpfdwts.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ijzfnxgc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2najylaoh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zpiyxokq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2watczexr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wuhtdfkd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hdnoispz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hslpjqqx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rxskdfjp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cifkxjlm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ijijfxui.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2rbiefnpj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ktkhtqks.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iillyabv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2oscocpmu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2xnwlzegz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ikikbgkb.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dlltgbvg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jcgajdnj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2sjqemynz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cvuuhpiq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2yyrrfsna.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ugyhypqj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hsppoesy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tfpsakct.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ifdkvygx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mepxlbvd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ubywgech.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qusylzug.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hofbbdeq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2eullxrls.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ozgqwqnn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qwicdhac.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yalwbxml.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dprrndaf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2motvrjef.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bgjayvmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2awvulalw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lvpbppmc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ioytnrgx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2julkpqii.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dqwviqwd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xzkpsvcz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fwhjooxi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wqyobhzz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ordqngxd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2iiqqkjoc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxosexwa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ywdtepui.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ccopmhfl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2diagacdn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ybqsiikz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qatqbuui.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2btzbjlmj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2otwwtqyh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yievxcyn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jruvcmnv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wtytxqsn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fzdylwto.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vnegmzfu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dalsueeu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2egccjypq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2llglyudo.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nbbvnjkc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2jpwssjkt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xjdlvxxv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2devdlavk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bawrcyut.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jbfyuasn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rcbveghh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nvbiieuo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xqkqgdms.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pxwnikgv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2oemlxaoc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ctbystht.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qmntyvsh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2miknbnzq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pcazbrmd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2njmpymtt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2agjyhygi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2thiqbafj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kjuoigmb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2sjjrxinz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gnccdqnf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2epwtmhuq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nmbvnnwq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2qpygunmo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2chheydma.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cfdqgvia.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vjbjelbk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rtkcqvqa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2eaapikfe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jwrsaeph.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2egrfeihq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dtluufas.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xsqomjgt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzacnsxn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2furagsms.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jyxsxvlb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rnyyzmsu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtybcutq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2afiivgde.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2halzprjq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vgzmfiue.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxuqdawb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zhgvzyva.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2xmwmojue.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mltphmpq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tcbcblfl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pvmbtpvi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2caxfptdp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2inhnpamw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pcelttqa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2prbcupzd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cqbijrez.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2euutkkwd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cxbavqah.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pnmljkrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esufdanz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xzzztwja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmnpbynb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2mqbcxsyx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wqcczhod.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qlylmmgs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pwvijpex.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gvpqpwxt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkvqlrnk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ossvbsry.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mcztcouq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hknzippp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2qpvwzoqq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdwrxewt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wdywmpbm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wnfxwrgb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2svfrrgry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2onmshvon.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oqqwyazt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qoevtcqj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nmsyvrzo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ahhpabxw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bgaydjde.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2efqpdakf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vzhsskyr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lpmyyilc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bigaqrly.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wgysjljx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mwycyhds.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kqbdhsgy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kkbcegqj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jswdyjkg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gsgedcac.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqejzbat.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vgnjnbzu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lrzrcyrk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpwcpcaz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nspmgphr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fnioilwf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xehjkgoq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jkedgdch.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqxcbrvb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dzxhwfdk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jvbveiqe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qevxdgey.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nqoioipn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mzmnbcmh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mpoxuqal.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uxurzyrm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lblorzuk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2snwrnayl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qshakfvs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2trztupja.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zogtvjdw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ktopplxm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2howoepsz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xzzjwosw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2syuomccc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2vldiwpjq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wxsxcsai.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vvadmqnl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iolproco.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vyvhnxdm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2slvbdcrs.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uuqtjbfl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lvgbmdnu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2txttllbc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2enirlgxz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ncwrenql.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zbrqutkm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wgumyxvb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wpotdsfz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2prdofpjy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ewkctxrg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xdnxswkp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mlprvoxv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ekdtpjcs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2sacuzjln.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2imqnlijo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hgkyncrr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2stcpkfrw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uccsaeeb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rzccuabx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2uwqtrnki.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lgiyreca.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hgrokyjy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2uiqxwyow.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dtjzezjg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tgrmflmf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2irktjmje.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2czitekrc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kivfubbe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppycluro.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nwfifxma.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jeofoqec.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wmtqrhtw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ddbliyde.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uavamjdb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xrqylifl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nsixvjrd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yknouuzt.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pyksndnl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2plcdgqqv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqvyffsj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2smhoivxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2hkrpobnx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qjgjvqgt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tkgvrdwx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2twcatbkf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nqnyslvq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2anrtwboo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hfwlycfd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2oolxvscx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tkzovgeu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iromdpcw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hhlwctox.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yqxmcqrq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xxwfqyoo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2urijudln.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2luafcvuw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jlxzlgfj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nsrcxqty.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yrvubjsz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2bfxqmqjr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lrvmeets.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rwcpsohs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2njlulnfy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2auuxdqiq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jhqmquvv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nnifrkzs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tlvwmifk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zhdxpjug.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zdmnhtmo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ydvtvqqk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xlrizezg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hdfsfwon.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2grfzkmqc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gcgwchrb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hgeuedkw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xkfyhzec.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vxtcthdh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hoczgssf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zwffchyt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2aneoincc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fohbyqvw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2scfsztzf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2vvihflph.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2faklobdt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hzllxwbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2afqkikru.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2csfiqmea.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vlrgvfja.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jjwwiddu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kcbplnel.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kvbqvbps.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hkzhjlum.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2krgkxzoa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wwkltcse.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfomgkax.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qqcauxvi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2psbvveeh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nferqqjs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wvjejqan.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fcjavuzw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ilzmrrlq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lyejarzx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zeucjzpg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ogqzqssf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pximfyjw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2efmcqmjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvfyatkt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nsinvzbx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ojyorgww.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfaobodk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hkltnpjb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xigfnmai.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bevhthlt.html


<!-- 参考信息 -->