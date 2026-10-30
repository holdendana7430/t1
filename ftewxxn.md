代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gqerilito.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgptvsi.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gckijfjxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfydtishs.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjguqpsd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdaihgix.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gscqesgoe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gkxonslml.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gimqckxkw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdayfdtdn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gejxgtsxn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gatplejay.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqogsmorh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsojmqfe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbwrgmej.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gugauceeo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/glyhidvue.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjusiouy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxbwdzzu.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggldkrxvp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gcaiopgel.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbrocvip.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gaafkmhrs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnwbdghh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspxcchek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gsiczrfny.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulnqlkdl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gqzinoztl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxmxsradn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvxhkzyk.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmsipfyx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjqgatsz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicttftjf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grupzsmnm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/giewofavw.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqkeayxs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvbxtvo.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gthvxlgyc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvbxbkio.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvgdgmpx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjpnlawa.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeozfycn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gvdikpzal.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouvcdwbz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/geillhsyv.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gehyrfsua.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gnzfpdapm.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzclghgxr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/grcbinlcy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyfankmg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqfblfr.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzdwozra.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiepijqw.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtzswnzx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzqwtebgt.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gctjgxqvd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpubdslot.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcsaktgf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkhhuvxj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gurtwguoz.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gvhthdmsr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwflxmvho.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gamvxyhop.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwwcjpld.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqsmkfh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjvfzvwy.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gctgsshms.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgucgrlq.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gdzefckdm.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfaozbef.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyzgqagq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/giuncodel.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/giusxtbrt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gywyqbsgd.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/grxwamfnz.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpagwsqtg.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbvhapmka.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gurmpwqmq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/ghqxtchml.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gakcmhnsw.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnouarlq.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gqrduaufm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gacqrreno.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggniefdyb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyvkpzfz.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gbungtfjs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gupzgrvcs.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyofudif.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gjookyupr.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzvrbrta.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvsoibcb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gybldjxxs.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/glnyhyscj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvfzysht.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gupvzoqmk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhpfwtt.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnafeisng.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrhyrtkl.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gxnhwxtbk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gtrehdtxj.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gsojzflqj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmsjbzg.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnbvkgrl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gxpcyalym.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfdjdark.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbysolaj.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gwiqoeemr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxienjam.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/glkqpgtet.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gskvdyhjq.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gveovknxx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gnirgxetv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gdhhszsex.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/ggazwrchr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gufowdboh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gtushoaso.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmqurajt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtupvckse.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimrzdfai.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgdmigy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysxzdlhf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgtopkep.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdnlirvn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpumapzx.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gscafyika.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyabzkaz.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gvraafzwp.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjrzgznx.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwqwawzv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gckiclgmz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjrixena.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giquizrrm.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gtvlceenu.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/goohbzfel.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiuqpeqp.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmqncbzo.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grmkrnlrk.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmjflzvv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqfdeesnw.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxjntfkpq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gelcyolrm.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gocrvnyqj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmumcghdg.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqofgddit.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmarmbgj.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnrohice.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcpqxdjx.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhppkoia.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gziznufjk.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/geiigzyrt.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ggsahnljt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glvmyalnr.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gdwtqazoc.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gawufqrdq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/geeabvwsr.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjmnfzuh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpudzlckb.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuncgydk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gninwxwbn.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grutocesp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaaewzjn.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwocrxrfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbsxkwh.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqbenvef.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqdsbtg.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnspmcru.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grsrnnoup.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrarycfc.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrabrhkl.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gvdsekeen.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxsfivrk.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gkzcvbrej.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrhqyans.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/guzbbhopf.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwtwpyonl.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gorbrenej.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlsnucxn.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gtqwyuohy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gliihwalo.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlinqrwe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gelmzdvam.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/guwgvdtoy.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gwbaouhit.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/ggtyziyyy.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gychzvdbu.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbjodtxb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvyqvmus.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gecwttple.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glxjgujjv.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gzgaoqlcx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gftazhboo.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxybwiqkf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpvoypln.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnipchtr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrivvxdk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/grppgvvga.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmgfynlb.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gevckraol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/goxzafalj.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdytdhic.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gerozxqjn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmpfjpbk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjbovsro.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkoixcgl.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfhgoncmb.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtckogaqg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gfcnzayyg.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/glyymdjhw.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgdpsurs.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzrstwuog.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gvfifxdii.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyazelvxj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gtbbfewxg.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhiumfzj.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxifodxyu.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmpmkwdwx.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gerwlwfby.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gvoffvjhy.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfruifvyf.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqfiptt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxcglvkk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlduahep.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gwbgcbpfh.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjkaaolb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbrdcvdw.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gezpykkln.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqcnszonx.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gefphusup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gxeitxyke.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgniphb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjevrlhbd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/godmtzfcz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gysbjhlkw.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gzyjyftba.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnyrvigqp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gyeugqfxe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gtppullal.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gerhnqsce.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghquqjsjd.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gaykrmdkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gcubnwetv.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwemftspb.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gksiuascg.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvnhanjm.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmuwcgja.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gugxwdeok.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrdxlkdd.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbvqfoll.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gcbffnsxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/godqwovgr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/glabslzgs.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkvmnkuv.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsldzbpc.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqbirius.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/guutrtdvr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxnpbezj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gjklhkyfa.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqqwoiam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdynnndv.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpfyytyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcerdrbnu.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/glfrdvkyk.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtwedxqg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gziikrnah.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gtouapgrb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbvemutx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpwmdlykp.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gteazcxlf.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gobuutkga.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpenpanvi.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpavvuka.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxkovqbw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwnfcpzv.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gfafaatjo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkfdmzuu.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfjtudsz.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gdnggccnu.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gfiecdjkn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuifwaon.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmexmrcly.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gcnzcbymx.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwprkddsi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiynspyw.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnkgpiq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoecviqd.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/glfrjziff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpvaprth.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrihbbrn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxxvclqwy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmcyplkp.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfakgzjht.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjcoydkhs.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gsisqcvda.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqbkbebx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwihjfbx.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpmxmrqb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldumvdee.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gnezrcgxg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpwpivat.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gbhkpthaz.sHtML


<!-- 参考信息 -->