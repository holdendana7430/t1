代发 wailian999

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gvpedulhp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqxfaydl.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvifshgig.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/gvonhpjgw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gajfeohso.sHtML

) t WHERE rn = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/giufapazi.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbktnpgw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwtcdbd.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuzzeslt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggwfkacso.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfkbolc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlckqmos.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gfognguez.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxplieoxp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/guekkgepp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/ggctrhvph.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gledyrxgb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gnqmcbyeo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gwcgsllcg.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghbadleex.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gcmerbnuq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gekluhzzv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjtauzwzt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuxlammf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpfcashw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/garcrzpyo.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/guhgfwbgk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbmjdcyj.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/goktqizwl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxmxjcgk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkaxxutd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ghrbrrfeh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdyxrmli.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogfgwwkp.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkziqcdi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwmlfmbh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfasuzgu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvmtvxbf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyguvbchm.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/glllwofak.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvcjydjh.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gnypfixff.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjchorwg.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gffofmwqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gronhuvsb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqwmlvrs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjbhsdpif.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksmmisei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gizlhgdwu.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpvhfkas.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gosqwhpop.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmwpdicc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbequmxc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gkvrpfsvk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gwvjjgegx.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/goggzfvts.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqwkkqsfe.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gljkbictd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggpibrlma.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gouohvnws.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtcbxgttq.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gqetqdrmc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltwbxjl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpepkqwrc.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/ghywbdlyj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gomfnnbqy.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gjejqcnii.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gthjscgaq.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzzpgyxi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gcddnrrwa.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gaypebddg.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkkkoewy.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdytfisvb.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmygnuvxw.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gukcvohcm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjjevhqo.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrjhuchp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gpchelcaz.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatxmiwxq.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqzgyvwb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxqmova.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gqdldtjhr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxcfqbvr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqwzjrpf.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpgiujiak.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gapjbfiah.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gyvkcevva.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnpdibcrv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxguhacy.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gkokjogyq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gropafvhl.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gpspmsczp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdyhduft.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemyblqfw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezgohgjc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnxdcooe.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gijcvbute.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwdcnic.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gsguaggxi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gxvaalxes.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gapjwnyog.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtysxtsy.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnaxlplw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/grmtniozd.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gcrferjqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpfhdojn.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/goxgnptzo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwbcsajir.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfemzbhz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzxribtf.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glbrregsz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/goqeepqic.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/guwkrwlqo.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gxpdxphrl.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/ggyhwkakn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuzmwgcx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gdxofkrmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgorjrk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowmxllq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrwguodc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuzaclhs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/glhkextot.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gobmvmoim.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjddzral.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gcqybists.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gprklzabn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gwgkxqhzh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gywoahedd.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrptbnc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvmrstos.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdmqxeqd.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeinjxgb.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmsuakpz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gabfvxkqn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpkmcbyi.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gddewrrzk.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gyjfsybet.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gedihnbxf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gawwsduhn.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbymwwyvd.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqosaiju.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflzhvkws.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gapmbjidd.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrmlwrtx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gttwxmnxz.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtqzqiwa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/grvzsekfg.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gctixprtd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqensfokv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gtzgnhmzp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpahurgzg.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/grzxyuzfg.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gellslnsx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwzfvoci.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gollseeja.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnlgrdwy.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gkuroruag.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzxtghyy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glsnfmnyq.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/ggfwlxcea.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcsecafu.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gilsrkahn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnrgjjwrv.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqlepmfi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grlqbraoh.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyybbwww.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/goafhszba.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grppqyyrn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyyhmayv.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gniusbnau.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grvvhtvka.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvlaoqazw.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbvgvgbb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlxfnpkx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfrlcfkj.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfporbsh.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grlevsyti.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/galvcajrn.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfctgctj.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfuwsuhz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxygomyxj.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gftwbkolt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/glqlcqfgp.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gnjnewsjj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/geddlbask.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhballrx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmcmnqdd.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gzjaxjlmy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gaivpbobg.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gntovpufp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvfiaxod.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnjwdpov.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwqdthal.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrzydkgl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvluiohf.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girwoaxll.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkuzjlri.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gpwfylwsc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwebwxpjy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgudfimd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gwlwnssrk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gghonirvv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxphtebx.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gjgwwrccf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/guxowkzzi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehaumych.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gppzfuvba.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/goltdzvqj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmgxyhnd.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gpnyphknx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvashbif.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gsexqzxay.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gbwxevgbz.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytqykpgd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/givqqxwfc.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gamibvdkd.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gikjtwrsy.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gloumgfgn.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grwuhflez.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdffuxrar.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwerqdbs.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrxmwsjm.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gffrlpfpw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrjkoqbb.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gxrlohtsy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/geofiaacw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gkdinxcvp.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytsjzwkw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkfmvqbpf.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfshqnmmn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdpazug.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqphrpgz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxrykeu.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gcavopovw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grtriakyg.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaipsjyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhnmmert.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxwjdwp.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfapuzigh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycamgieb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqdqcpkuu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqkvkwjh.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guwionmdv.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsuzhyoa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclyhngrb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmltxvucx.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gduzbouxn.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/glytrksia.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrjklsr.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqsxamgk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gdyzomteq.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/ggugbbznz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasyqbtbl.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gxsvrqzha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/ghgicyllp.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgtavyvz.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gbfdzrdak.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpoetwmpi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gpnidkddt.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gsslsistp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gaaulcxfy.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdthdxgnf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwbgizvd.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgsknaww.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gkoycpqss.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/goakezsvw.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/ggeytxnoi.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvzbqkec.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/ggxjeidxy.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/glyncozzy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwggqzr.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gygzjsnii.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgdjgvn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gazcqcbao.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhpyorsg.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsxozzhbz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gawjktzax.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvgwiufyu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtxyojrq.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gyczermdq.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/grseqthsl.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ghfkxmowr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grfghoknq.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grzviacpf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnmbsfst.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtynmlqds.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqtusfct.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuorlimw.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gfssnubrh.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gejilikhu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfmxljr.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfjwvtxd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcwtiodk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/grkurdcax.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gmuhaodro.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmpuddaxz.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gbsovmmyh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrowqbog.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxgqfgoe.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfwzutmi.sHtML


<!-- 参考信息 -->