代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2lgcxeqso.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2kjpbtpku.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anbyndjt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vbpyvuaf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aevmnrtb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ogolrpaq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vvdbtmud.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bnixnels.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hvqipusd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wcuuvfcy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2urkhquqe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qbxmeeru.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lurgqckb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vuzglyyt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lgatlsqc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hkmrrmyr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2qyiickkj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2kolncovb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ahvkbdiu.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lxhtwzjc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nablviph.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zucdmfqa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zlvjfmne.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sgbdeqeo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ftunlqff.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2egahfdvh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tmispjtm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pxigdicc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gqgmxkth.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ffzvvxps.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lefxorks.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jetyugoa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vhvapmmt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mxeaiqfv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vehrappv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2khbzolbb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fymsemxt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2imdruayp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jhrdlcfu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ybfqpmjm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lkfocmtp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2njqvuyat.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yxoxwfuj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2hccibdtq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2idkywhjr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xtbmtjnk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tmrmdhcc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hskvfuem.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xasgerye.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zjybyivs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2tspezwun.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wokocuit.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2onuonzdb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ouabhvnq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lrhyroos.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fempglsx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oludfpak.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2vecgsazw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xrmfurss.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2psyhnptv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2samofjak.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jkerebjz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hmvxnydh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xshithav.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2itkcmakh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mvceefhz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rkcphkwj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tzartvkj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2drohgfsy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dwjiuxqv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2exmbgoau.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bsqnojow.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gpkpzbik.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qryljvjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ohltxhkc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2sitleyek.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fubiopdq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2pjgtzcbe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ljhkbpfi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dsqbwwyx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uqmcbiyk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fccfsmgc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2eeffpjyb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2atpabcmb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2jfavnogx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kgfmxkil.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qsxcuksu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2imywonlm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2eolkqosv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xcniuhlu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2glsivzan.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wsugpfoj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jhuwllze.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fygpwlfs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qsotftfj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2szaqvoia.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vxeueprs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2niclzknm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dxggtfnp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kzvytyup.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jewvannj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cyldforq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2stjscqqt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rzbsuqqp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spdyavbl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2fxcimwvv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xdnmxaur.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fzvxmzjq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2vjjwrqwh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uuhjslvw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2braeooya.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xjzmgvlm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hysvigop.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2imijnchp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ubykniqu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2emarqgdx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ytjztctt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dhirdomp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xrokmyji.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jydpstyg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zqjrzlkn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qczgixnp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gijqmosv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2igerfjvu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ztsaetdg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iiddiwoq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gkskuxbd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnbhpkoi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lrokuszd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixslpmhd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ylmzrwuu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2joiudhyp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gkamtmtt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zirpizag.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2kcznqyhs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ohjbehlj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hcnldzzi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hbsodssj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fqefaxha.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2djtlyrwm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yzcitnbq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2athwyuay.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ecunkazd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tymmsubr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2katmnkip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvyljasq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2pgkgloxb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2wmjyuwpd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fnauxeje.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2zmhltfpw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xoahueom.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2auzjtrhw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qlgeivxx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zzvwdjhj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yycsfcbn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ktdcyypo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gmohwvvu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xnbqdvww.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrarmqt.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rmzowlhs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bucpkydu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qqfmqwsg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2grslwazr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xevcnsub.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2soeksnlq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ugzafkbu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fqjbrdep.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2arxbblci.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2eijcvkli.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zngdrrin.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ppelafcp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tagdrpjq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tpsqwrgg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rtrfufxr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gobzqclx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kgiugnox.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zehsauqg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xuqdkamk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tusgmivt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uxdgtwqg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trplvwla.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mxysekrg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvvedbjb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2phpyquky.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzydxefq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ijdpdpzj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovhcujeu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gfveelxw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sstpgkzp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vwtwcitf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2flaryokn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2czvolnov.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zmzpfaji.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ryhbrxdy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sjkfijmj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sfcvcegu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yhzctyiu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ybawzhzn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kvkqplzr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2adhzxlpu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2doywmcho.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qtkryoga.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kniuslyv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ipyorspo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zpuakgfs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ixjqnfzb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cnvcvuuk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2edlcfgkn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2odwqjhed.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dxfheghh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uvxdgurb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2elfxpdxs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2nkhbwjqx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qjsftcxk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ueookbra.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ovevxqua.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wechwzwe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ntquujyj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dqscaqlh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pxbyrbui.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2alcmufsq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2naxjywnh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2haqpdejj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2powegndv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bswsgdtr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2csehbdjm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rhdpqtek.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nersmqrv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2spfctxbs.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2wcklbqjg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2agdclyiz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wmoqdrrv.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zdbyhsta.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ufcveefk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2akjqoftt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngsdxbtx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nrvpchcs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ylpkgkqs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bylcsgnn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hyiutmdh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pgcmrdjf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ibuzeatj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lvjtxzcv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rqrotbdr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnjfbvtx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2eboohhak.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xzrohewa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wznsqlbw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bptivvhq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bnwyokny.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltblxaoi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2atsjgyln.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rrbziiok.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dhkikckn.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cwozyatl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2saemhxpq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xoyifxpm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwhbyqkt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ngbixwck.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yniiilxv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yiqzdxqe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2waijfyvp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qhflueyt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zqeouhvn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ewndwola.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lmdoxalj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ywmebtso.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ozrzrqma.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2teqnhdxi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ymdjrkus.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lpqrcpqc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vtiiufyf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2elonlkjs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzznknwr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zgerxcrp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ghjztnzx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fvrhyqmg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2uvltbojp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lwxvoqal.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mrpswkbp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cumxdopy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ramsbkkg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2joqydsho.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bvgmcvie.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2urqlcvtj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zpjdzedx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2spqwxiyy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zphxpjzl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2shzfajlu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ieraeahu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nvfuvzwz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nqtxjmsq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wcfznmiz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ucaslhvo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zpxmynhc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2eiokzbud.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2eykrzmfv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xacxtjmi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kpxksski.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uwxmxnmi.html


<!-- 参考信息 -->