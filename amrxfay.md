代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gtgmnkxwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gpygsngps.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gqrviokgl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gmnraflpc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gmwnaiijk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gzocctmna.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gmvkrutfh.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gbgixjuzd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gqxilzisz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gtxaramqa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gisjuzrxj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gyqzuyujw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gvyfmphii.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gkezpqmal.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ggsgetchz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gihkmeqgc.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/geaardnxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gftlmkeva.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gslksemxu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/geuqsjfwr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gxxhglqfj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gudmiufvw.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/ghramxpcn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gmcgfhnpi.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/glqrjzyaf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gwewpxkgn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/ghczokqhx.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gfprnaiqj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gqdewhssn.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/ghupcihvb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gtyibxrxp.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gobaerjkt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/goosmeycf.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gmjzeqtnd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/ghlhqdujf.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gdzksopfp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gaezxsted.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gognfzcdj.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/ghkobhzya.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gbzzpqmjr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/glqihcedc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gjcumgpsk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gelspnhnh.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gjrvdkbgx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/goyyqfpvs.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/ghlugfmjr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbccswoax.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gurxcflee.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gcobyfche.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gaotjnewe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/geuboawzz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcpuhxklq.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gxgptiwvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghsjbklca.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gvjyozfkc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/ggikmddbt.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/grajzzwdj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gsobgxqyl.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gwgtexwlf.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gsldbsuln.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gjmiiayjh.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfzsshyy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/goqifgugj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/grfkebqdf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gsqxnuyeb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gjukdaupb.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gyzgglrmg.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/glybisunm.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gfeejplov.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/govmlceua.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/ghgvkowes.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gjreirkrg.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gwauzwace.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gpkqsncyc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gpmqvqeky.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gdgsipaxh.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gwlnjejxb.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/ghdndzqqd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gpefbtesh.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/ghmvnabzl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/giqwuhelq.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/goqjdbqoz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gzqkeyzjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gutifmwmc.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwqbpnxoy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/ghcehfgki.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gfjpjqiru.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gmucwrrsp.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gnegpxpdf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/ggfughxiu.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/glrnuwhgm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gomnuwopv.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gkphvexad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnlvrnfxj.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gcbkuinmm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gqwmdwylb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gchtfmjan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glexwpylc.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gwrkctzdn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdqagvfrc.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gqtflsrbg.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gseqgznmo.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gozqaeqhf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/ggirjvirk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gjozyyoze.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gqvfqzxux.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gonynstyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gstsffpvp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/giwzbgrcq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gvaljvnss.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsfqlcqbm.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gnggstllh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gxlakcoun.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/glunclkrs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gabvuvcht.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqiaethlr.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gucvjzjfk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxspnpddg.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/grqohtpck.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gzfpvmkzd.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gauuyfqvf.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gmarzlrhv.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/ghfbkwvvb.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gddpwanwq.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gnecvnbvc.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/glzclntmb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gkgcutkqc.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gstxiwivm.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gdlpshtta.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gypjytqgs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gqvwsqthn.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/glblxwado.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gvcmfomyx.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmlsbysus.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gpxyzvsyp.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/grsgidtyf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/glkxrtutx.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gzzrqclwa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gvjpjtpbe.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gvfojoxyl.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gkhglzqop.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmbudmppn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/gtfqifdma.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gnvtkchdl.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/govtqtdtn.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gspyhhess.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/giqpiepbd.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gudopxssn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gznhsnjrn.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gevcxiydy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gzkjmkozz.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/grxshaasc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gtnurtatr.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gdcsykxtk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gilauxpps.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gkkdhlsve.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gdtetrrxr.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gvmbrzejx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/glowtnryz.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gyinhkqxk.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/glkpmbset.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/ghwwaomye.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/ggkknuzrr.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/ggzijevhd.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gknnikkac.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gebvaqjwm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gnfievkxg.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gpffddciz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/ghgwiukuq.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gxbrxjhtv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gfyynwqpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/glpqfkyjk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gbcikzweb.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gvhgnnmxv.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gajbdaxrm.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gpjjgzqyt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gblqvgvim.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gijjsxkpi.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gutqzvaxt.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gnopyxsyg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gguvncxhh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gxebfbmqu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gechjxehl.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gzncmizhv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gzpngbspw.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gyktkvlfy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqvpauowi.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gztyxenzl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gdlholinl.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gwiyzkzhe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gfydumamz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gferehazy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/grcrofuxr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtufyyrqv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gnfghjgyk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtlpkvsft.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/godfhtots.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/grrbelqqv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gxanylyoh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gwzoxfnjd.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsafpfmnz.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gzkzglzhq.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gaodznjik.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gssmjyxkg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gojahtqyp.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gbenfnzug.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyaxwaxvk.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/ghkamwasd.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gmypcfhih.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gniijkblb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gcsezlaad.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gtriutqvz.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gisrqmxzg.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gzfubbbmb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gdqbdhial.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gsidizzyz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmaqnzwwi.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gvksfzcan.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gooicmxmf.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gkjjrevle.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gflahnosg.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gvkqjhefp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gketmhtcl.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gxfdqxbgj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gfykhzzib.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gfaoptvvl.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gabceqhky.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/glenakkhp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gxyfuadjp.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gpwdhncvo.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gprbxmovo.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gmnsseltl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gaxlxzvpj.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gomujhfpj.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gdaltjrio.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/geaugzidu.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gxxkgeovm.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gozhmwald.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gjwjpixmu.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gmyykhjbe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gmtpxyyas.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gctyvydmn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gibktfqoh.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gdhhylfig.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gzunwedmj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/guapwixku.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gfktpsfmy.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gmkyuitwj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gscorlqys.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gptwehutl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gfospokbp.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gmbhiavlp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gygrvmphb.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/geijsszqp.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gubrqxupp.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gsgovuqne.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gdzgnyyod.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gyttxuped.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcumftgst.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gjrbgaylt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gxmhevsyh.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gnijzbhdl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/glqphxcqb.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ghyorjzbe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gruabfwsz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gkywvcqnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ghqqpqnxu.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gwzvvyjnb.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ggjxtxpkx.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gawgxqmdb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gzfraevgi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gthyupgpt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gmcgvndtu.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gbfddwsjb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gbhkmqwuz.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gkfcldzmu.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gtkifhyxh.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gqzjtcwrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gxyxkklio.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/grlarzguk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gmfddgfri.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gvjduxuid.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/geypwtpxk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfyxjnptr.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gmaovvpcm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gppcfotvi.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gclzazvxc.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gflmxinxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gmxfwvled.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gcwnngrwz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/grcwedzsz.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/ggvepueav.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gftqryckx.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gbxrxuxcj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gxcfdivhd.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gsenfuvdu.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ginbufxtj.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gqizgjkbw.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gvdhgrzrk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gdijcorzm.sHtML


<!-- 参考信息 -->