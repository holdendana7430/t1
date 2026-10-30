代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gbhoxwizr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/glodhwels.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gcryhpdnu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gkxcpinzd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gxbimjokc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gsurmdeoa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gwigjcccq.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/goxekfrds.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gmadwljti.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gxbalzjkz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/goajphzfi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gfqgpdchh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/glftiydsi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gqzkbvpyp.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gfuygpjjs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/guoyboehy.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gmswynsus.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/glrbffgek.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gpyqcupzz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gpsggldjz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gayqveujf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gwubairuk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gvedtctkx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gktqzephg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/giklpwwsa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gunybjmed.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gjayijysa.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gqdvennrv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gfgexorwt.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnhhnkafv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gbviicvvt.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gkzyrclch.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/ghyrsamwm.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gyfgnaqqw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gzjgsfzhx.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gfcjaocvt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqtmaszyr.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gpwqledvz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/ghctlqgwy.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gdxdokkfk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gnpihgarh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gytmbwthw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gyttytthe.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gamoozuhs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfnmkeung.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gbfwwoqze.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gceotkavc.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gfrwephlv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gfzwvurhb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/glzamiyhc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gwdaddivp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/goyipnphf.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gyclywple.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmjiyvnnf.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/ghcshclqj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gywiynoyx.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhoiqzg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gnmuqbwit.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gtyebpppx.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/ghlgzsfoz.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gzdjhrong.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/guqxjjphx.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gxiphrwns.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/ggaevywjh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/goeixgkfw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gbheyyhju.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gsxknrvmr.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gmnnszoyf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gxqfpascv.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/ghrtsnfik.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqkided.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gbregevcc.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gjizuayre.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gapduefsm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gvopvlooc.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gbuoofvmn.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gjrxyttks.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gttmyslpg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gvzdmsftp.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gehufbync.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gozklovvp.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gjpucuuag.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gunfvyzbg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gkgydrtjq.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gfmszuoox.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gwkijycyd.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/guhasinai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gyjudueop.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/grgpswkma.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/ghahsnany.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gbvnsfgly.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gixvzssdv.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gitcjzxpb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gktudntjp.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gyuwhsugd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gubssvubf.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/glwianmcb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gahffydkt.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glqlmserc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gnsxczggt.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/glzmxuvzn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guspraood.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gxppjrxkv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/generujee.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gpijnbsni.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gehygnlfz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/ggntbubbi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gpiyqjcdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gsdttvuyz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gvgyutevo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtebqgpts.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/goosylxlm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gsrprxzgm.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gpqpfriaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvbxghfgr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbxgiihcu.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gemwxzavz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzavrmhhr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/ganwcegba.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gudawdsnz.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gjwcxhqrf.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gpybxoigm.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gdajhzmkp.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/grjqxvnwj.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gglqlaoou.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gtgyvxlro.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gvyyhdgiy.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/guofuhoig.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gmkerqvdp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gtwejjudu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/guozjsrut.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gckhejesv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/geuvxaksq.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gfuevoobn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gbazaimxr.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gqylhozrf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/giutuloko.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gsivsxhcj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gqpmctuuj.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gcqkpxodf.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gpsmwvray.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/graognrcj.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gjuibhszg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/goxsjyiio.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gdtwxkhxd.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gcropbzbw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gxomnixvj.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gcfxczqxu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gknibfzfm.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gfpjmowof.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gtjsluoup.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfshidapw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gnexfsvgf.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gromacjrh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gpnwvlqrf.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gpicrsguo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gobbxyinb.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gnqucomsr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gizboimcr.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gdzybhdfu.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gifdgnjak.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gptexbkdr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gjtptnljy.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gtttvrdnv.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gwcpmnphs.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gyebsskrq.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gnwnaspbq.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gcewhbnhz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gvtlqclnn.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gqncpkfwx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gpkoptiml.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gufmcmlav.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gnmoixsox.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gerukcazp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gvkvybfki.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gguxtqhis.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gsnzkloro.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gmpilhxlb.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gqsfvpyfv.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/giwleiiqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gcksybfej.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gzohqidip.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gobzfycsk.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gqyiavzkr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gpgjdhpia.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gslnbhwyi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gtotqazcg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gwonexzil.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gfwenimqi.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gbrnckwep.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ggknwnegv.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gpvvhjzeg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gedvjcqbo.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gekyfcrzp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gjgvfxehn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gjpjpljew.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gkkdqhjrm.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gxxhxpvzp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/ghlbfjqyy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gxszrberu.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsywtnnbr.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gmlbwhyqc.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gjvndyvrb.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gnjiiwerx.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gilpxptun.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gpgrrthgf.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjgjytmlh.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gatybblmd.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gjgeporlj.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/ghkekecpr.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gzjqlbsvx.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gjnwauhcq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gnylazjpk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gsyptxegi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gwzevhniu.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gkudugizq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gstvtzlpz.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gombgwsjt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gbxiuzoeu.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gvwkgblrx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/guhipsgtd.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/giytiutur.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtyoshfdk.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gbbthbszn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/geduxdopq.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gkognzsff.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjmxwjbvn.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gyfltgagx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ghmijcpfo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwjgprraf.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gtefycqmt.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gnykmqqxw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gcoakunqi.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gemqkeuoi.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gmrxgodyy.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/ggbsaktdw.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gjffowjig.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqdobwfhs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gauhfpcnb.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gdrljknro.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gauefazvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gzabcpmut.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gaylnaznt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqpugwj.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gkexcbsvc.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gqnmmkvbf.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gtyrreltv.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gyrexesbl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/glommcdqm.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/guymffbkp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gditfaigd.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gfjixmxzk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gkdphulhn.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gmrzyijge.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gytatidmn.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/geqknvlon.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gzomgfpis.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gmgoxoarz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnhivyqcv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gykcpqppo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gmdzithes.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gdtrcongl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gpoaexqjk.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjooxccja.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gyuofdsjr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gfxvxgfba.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ghgzgrilq.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gvbnmhbge.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gplypidph.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gczijzbxa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gyhuztapf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gigflbcrg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gipidcybw.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gamzepjiw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gnhxzdboj.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ggfslssuo.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gepdkhpsg.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/geahlmdxe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gsqucuffh.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/ghnlzoyiy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gumpwdgkh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gawttwrwp.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gdzcvtzuf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxeawipye.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gjjgznhea.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geuyinqjf.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcaxxlcwj.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gwzqzayff.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gnfwzysll.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gyiieiatp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gfqbztzus.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gmswcglaw.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/grdpsfkzu.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gvbklakxc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gjtpfhawj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/glrbrdnbj.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gtrorwxem.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gvwsnuomi.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ggatiehuy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gphofieau.sHtML


<!-- 参考信息 -->