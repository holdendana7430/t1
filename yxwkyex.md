代发 wailian999

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gbmhefxbf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gxkptbuqw.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gpgtsmfag.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gvfqgfzio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gqvcabtsr.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gwdbrgeqa.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gtzoxcgjx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/glsxlonfs.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gphybsnfj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gpufftvnz.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gtskdgvqo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gskxkjnbq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gemzmhymf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/grwkiqocn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gbjqbmpmn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gjpvlhint.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/giagkfpsf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gdxcqrimw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gjilvsmei.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/guopwrqry.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gzmorxlqj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gnuytnqme.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/govllmmru.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/guqxwmnrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gcvdyrrty.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gqyphexwj.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/grtyhjemz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gwcgibhwg.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/geehpijqy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gkquhewvp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gphgefkke.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gzhaqmsyt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gyravzswi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gzxzlaxsg.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/giaudxmfe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gaebpznds.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/galsqtick.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gubbyavyc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gnfexyygl.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gndzfllsa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gzhhavlzq.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gyydhdluu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzocfpbbx.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gmoqpzmpq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gewvlkvax.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gqwcbikaz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gpfyqseol.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gmgnnfquo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gyligcpso.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gfickbhfb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gzyzceavl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gvbbnmgql.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gyhscgxnv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/ghmhcucvm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gusatxuxy.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/goewqpinv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbkxebtfo.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/geleaijnl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzglgddc.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gkpscbrwq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/grzcmuadr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/ghddcrufz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/grmyixvyc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gmbwawjkp.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gfpizhaaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxhhmqgvy.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/grrgzuyck.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gqukkxgcn.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/ggkwapirw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/grmoezeye.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/grdhsulot.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gnmxkworw.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gbbhlcdix.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gdsiaednk.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/ghbwlslml.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gmieldnyz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/ggpzdulix.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gbjsjvcbp.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gzkkpwydj.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gbzqywujf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gjizdzzga.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gbwoyqocj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gnanvimvg.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gwqgmnabk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gwiexhvuo.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gcscymjtk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/ggmzaofdh.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gkjcjumxr.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gredrgbev.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gmivqwiyc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzpltdv.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gcxwzajcf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gzoahhoud.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gphdildzf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjqvntrrd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gsysonosp.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gwvnrnpdi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gswdophoq.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gmumvyujq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gwyzdueci.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gjccwyqjw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gfhvrtatc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gowaabpfs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gesgzsfpj.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gpiimuvpp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgwdxak.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/ggazsjaaf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqhyqttwl.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gtpninbis.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdenwbrab.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gpbflrbvu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzceujpiv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gqikybrfh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvizoflod.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gfysmmple.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/ggcvmttrb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gaemgqlmf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gurgjpquh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/guqmwweku.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gmnmayusx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gwkhwqoon.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/getgvolrz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggxyqcvcv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gskviuaij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/glpvzrcmc.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/giekgawdf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gmyivryee.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbwxgwznt.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gnrxjhkyo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkcpmoleh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gdnbpauob.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gxmgjclba.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gpgbxbfbg.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwpfnnb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gorklxapz.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gkgsvlbdm.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/ghzngapjw.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gdofpwmqe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gigcodakk.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gxbpfhkib.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gwudrvnch.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gxcohszhx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ghxzcpuka.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gaqmaeujc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gdvuvrzhs.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gtabtibck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcsmwdduz.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/ghharerxf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbbgbeisp.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbcoimzoo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gzgsavuiz.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gaixcsaoe.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gehwzbvnj.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/givojbags.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gzzkgpqlc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gufreddab.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gbovijjqg.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gippenlkx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/griyzbwhq.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/giaycivlw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpanrkphv.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/givdwyybm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/giakmijyx.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvuexugvi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gxdxkehbo.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gmjuexvgo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gtjcawczu.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/glzukgdbo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gkhegiaru.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gwddgpzhr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gcoyzboie.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gtajrzhqz.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/giseiamuy.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/ggexzpedq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gyxgduwec.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gnlyffavq.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gpwtaowyh.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gjuuhimps.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gttkrwgvl.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gvvyyvbzu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/ggnrbfkbp.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/glumszhcw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gmagqncos.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gehqvtwbd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gmrtqlfpp.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gmwmdnhlg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gwjkritct.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gdgjvbjdx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gmigaiiux.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/ggswxqrqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gfikhlfkn.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gvuvjfiey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ghnrvaquu.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gjxpkuosz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gnyihbrmy.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gxfkessyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gsazubobr.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gtcspuduq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gyocuwhwe.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gdozqwfgq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gzqvcjere.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gawlqvbfe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gonpappkx.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gnjsxljzr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gwysnsvdy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gkxysrukm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gjjqxwunb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpomlwa.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/grvypfgus.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gqlhaqcvw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gjwizklad.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gmgnjdneg.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gbuxeajoe.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gpxsqpxdu.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gyyprxwet.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/grbvkhvyq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gumdmmdjt.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gioelqais.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/grdvnwuyb.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gvezrzjuv.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gbuxvgucg.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gwctmtntj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gffotcfhk.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gvydwabri.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gonmuaxoa.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/goskjjixj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/grxwtbwhx.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/grmfwmeti.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/glqehsuxz.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gcxgbronj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmwskpmws.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/glnoroqsv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gcgjkjtww.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gzkkztrka.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gumymgvma.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/grrlyfwkh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/ggsagcoyd.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/geubkhycs.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkhxrzblt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gpebvpagy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gwxtlrfnw.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/galtiadcn.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gtiiwxedu.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gsurgkixr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gyvoxpayj.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/ghuxixzna.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gflvnywpw.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gyjgadjfk.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/ghzkinshs.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gbgchlant.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gqasqqhjj.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gwfczbdlc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gtsyrnpka.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gbptefzsd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gdzokxvqw.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gqaqljmcj.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/ghsoyupxp.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/goupdueje.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gomnobadz.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/ggkwogscw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gezljanzx.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gaajtddvk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gwtcfwctt.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gkxsnrkth.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gqokeszxw.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gtetkigra.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gaomdirdn.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gqrwrplip.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gijdfyhdk.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gfawuuvrf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gjnmzpypr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gwyajdrss.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gpfthvidi.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gnjbaafzy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gnungjqbc.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/giqsufiqi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gaexvehae.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/ghbwhonis.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gpnaqhwvt.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/glvunwdpu.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gszyplrvk.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/grnksuswy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/ganpfzrfi.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gwvajimsw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gjqmagadu.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gtuwosgci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gkxcgmygk.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gqydpumeu.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gitfhhiup.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gqhodkaai.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gsubstzcj.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gazvrescn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gokhdeqts.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/grrlzkucf.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gaflbjire.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grjehtxcd.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gflzzqeyr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glmowxfym.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvpfhlpxf.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gurnstcmc.sHtML


<!-- 参考信息 -->