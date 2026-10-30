代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/ggtgqgmcn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvizqwvov.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gsoctkcxb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhjgqpbj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqldtoal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/goqmmbwcf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gvgudsmyz.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxofqmner.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gplvpweds.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gtiuzfzvq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gfokhyqsn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwyvsoad.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpkprhos.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gjbvadzwi.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwlazcce.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwsfuntv.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqsbdlat.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvggkbpm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grxmeqnev.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gatvclcsf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guzstwmec.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqfpdaas.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gicxagssn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gndwqkodq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdbqlyeq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gxzzafiud.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvsikaob.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoqpjgdx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxedtsog.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoxaifsp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpryfffr.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwpbmpum.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gindvwcso.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwudofid.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gresbuntx.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrgyfbyl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gpuwshjqx.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/galufgbyt.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamrnixmn.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gprhwbnqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhnxxehj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhygmzzq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwjhwhdd.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfxnrlwp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcggrqirs.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/guodqzjsg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ganvvxsmd.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvcqdxgs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwojhija.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gviduzten.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gyndkxpmk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/giwntxano.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gfddkxrih.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbwvxigkr.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gvqvnzpgf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gjsyavjsd.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdmjracm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/glsfxiqsv.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuspdjis.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgnvlhat.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gleqsbdny.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/galwklqvs.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gesezlrkl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gebrxhbtn.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gvowwwlkn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhbnhncv.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gcjjlqubh.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzexqgkt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnglolkm.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gamrirehx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxhqzpun.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gifahetbf.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjcgwirmy.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gxgapsrue.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaozqbvr.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gapixkifs.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqczmizcj.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmquoqkf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmtfqkvo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagcislfu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidpuxrph.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gqzxaafwm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkkvcbja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjvuxtui.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeelhrzb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gemlblevv.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcctiubd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsodnsue.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gguvyyvpz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhqfkkdl.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gemzgdmgc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gawebycym.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbangtfw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gntflzkkq.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gplskdftf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpepbhge.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjeipegb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtzwqmjz.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gqdnjdkqe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmowvcma.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gfuuinuqu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacibcypd.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwwfivzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gosgyeowh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/glvzyyivx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxefpik.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaqauyeh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzohqlcj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/guarpdiyc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrmrwajv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleloayud.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gruwegdup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/glvtbmkik.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/ggbrujkrj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gedpzbkfp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjryvqkf.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrtgdet.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkwskuqy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwusxovu.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gezydmhca.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gaiyagejn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfumdaco.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvhmoqu.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grcfngelj.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gzxevzwav.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsdhcetqf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gwpkbswne.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvwhzxwy.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfncivnkv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjjvpqpn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gguyjpwfa.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gceolkdmc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/govzafwew.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjcvjahh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfxzwvtz.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghznpxaks.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gamrzgdcx.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gnbvexqpg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmurwlttp.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/grsjthrvz.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gifvlhgdo.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gannboveb.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gossquwct.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gvmfibmiu.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiffwjcq.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwgxtipi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtqeoimp.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gorbraxos.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfoytfamg.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gyivjwxsm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtbnhoqo.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkubtccj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkvcuwexk.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnlgbwzly.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuxprnok.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/glhwmugnl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjanlxwwt.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyovemua.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzbnsvxlm.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgpxyvkc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubgearml.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkappaenn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqsvrzzjn.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwgijrlrl.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbglibiir.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gahjxwzrf.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdhtelljk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllglwxpg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/glckqalym.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwamvovjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtngwucc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwhawrvf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/giffexznx.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtiyskvau.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshymvuiy.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gflrsvasg.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gsjfyewwu.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjejyegpf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjwlpvuw.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyqzrydu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwulobrty.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gnjzgmrzt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gcvrxeuwz.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdehykkx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzgnbow.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwgyghcg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gizdmnrwv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoduspez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gufqdqhgt.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnuvaqbi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfywvjtd.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gykoqvcmx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gihhxkjjv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggptggzqe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gcrqnzrop.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxdichehl.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydqhhccm.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gilztbgkk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtnuuscy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gswrarolv.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gvsoyfhui.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gycuvyvyp.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaeujpfd.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggfefntkl.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwhcbjat.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gcmifldil.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvtejydnd.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnrcwnfs.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghajmzlax.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gunfekjum.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmargkef.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmejvxnee.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gtqautwww.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gezuncgyd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjruxdmwv.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxbvshhug.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpzjefoj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiajudvf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gecsghlwl.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjectcdxc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gqjagklfq.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyldgzes.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gueyjqifk.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfoclapu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqpaypmo.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpfmfpay.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtjkcaewd.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gujaixafo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gqocqatul.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gosetspro.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsstgkqec.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ghzvgaggn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gpusujvid.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gawzyaxpe.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrcwbivo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdbynifo.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/glvmoyjxv.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrbplpvt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtgfmelb.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/ghsvqaqqb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrjllqmu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmckxzbac.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlvzntor.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/guijalyfj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/grukjscmu.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpdhsmczw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gtexakcfn.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gslbilmyi.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbtnhcyz.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gsxykibos.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gamtnxzib.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqcbtdo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/godsuijgp.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcfvxojtn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwpmmbj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gyuvgjmwf.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykjimza.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gsriyvfmm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gggoqdewy.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhluuwgm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmvmsiqp.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gveflderb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnpaavel.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gyausqreu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gjarvuhrq.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gawllfabu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/guzcozvwd.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gvoxybjsw.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gporzgnax.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gxrkatzqc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmwjvnuni.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzitzjueh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gnunaopks.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghidkhdgq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gtacunzhf.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuoqqnsm.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gdvceiqid.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grilwhnfi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmfcbisr.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/giymoxgrq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonrwybmd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gmkoqqanj.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqtebubt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmborfosq.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfqhrdms.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvaobbnk.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gpyvognny.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gsnoxpeen.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxanwhmqj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwhskmptc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsribptky.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gktijicsu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdlngjih.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhnxflld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gopmsswkz.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gutppwoam.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcaipbgyj.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glosgsfkq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gosmjvoyy.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gscdfxjxg.sHtML


<!-- 参考信息 -->