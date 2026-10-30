代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzsnswa.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdaqbcfo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxcxnhtd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gonexcnpo.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gmypwczev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptaqvtfr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcehsfod.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztiztduc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcgawjzg.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkzjxxe.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwunnal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gwsspkugo.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnkxvyf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrzzfpcy.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnjaaiwr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpnuqhdrm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gissxbxkm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbbboagt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhtctvwj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gehsspmku.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxvccqms.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gzooculxk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/glmbytryy.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpalnvjya.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gxodhgcdu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gjtsegugn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyfympbax.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grfgnftju.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/grrwytgko.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqltdory.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/geqvyrsxk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/ggkmzmaok.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gsucnqeld.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gsvqfaiin.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbmzrabq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/glefumjrm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgfejhkj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gglhqmtnk.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/grgqxvrkt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilpftipk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjruruhy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrxqvsfa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfxmrblu.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmpemxih.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiquyzbp.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gemwewqcv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjpzldud.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxohocvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grfjvojpv.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwijvntn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifnyepg.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcjjytvn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquztdrfh.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gylgriomn.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gbkdfoank.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/ghrghycuc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtrzqrpz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpblfjgsx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyetqifw.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzodlujm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudybdyeq.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghficstmh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/glwsktidu.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gxcvygmmu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvyzmxle.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grezgmrng.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgqpmzlq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gqnlypirf.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdtcucxc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gadcmzoyf.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gzbhztzgo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geothgjjs.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicaoktnc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gqrgxdcyp.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnclnctlc.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpboitrf.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnelkunz.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gkvllvsjq.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/ggxwhqzso.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gewrlsnmd.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gmidoaxaj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gccgtrppe.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaqhzfoy.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gteiyqnto.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcliabxkp.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/glpfokmcv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gvxfvcsbn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaentqfqm.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmixrhdzf.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsflqwdaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtfurjdq.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfufusjl.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxghhjagx.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/giozcyvot.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbuncieg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkozyoken.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzylokzk.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gadoyumfi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gkoebsnhc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvkuccpx.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmucqgvp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gxciqarct.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gewzokrsd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gfodrjvdf.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkgjyeoqv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gdnbvhgjt.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gapnyzidj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/ggcyzonhf.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/ggxwcebwo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwrjlepg.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkmudenf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gidsldhmo.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfuoxqg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyflnvvdb.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/grfqiokrr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gquuifqhj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjovempol.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkavypadj.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsctpcxtk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmemxrad.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gojskvmtt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknusbnkb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghatomjgl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gazdzcmfy.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwobjoo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjojsykm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhgwzpsv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpgxypts.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gruegzkjm.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/genrtntxf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlqedogv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpagsomxs.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwqsnqiz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvzctfmcs.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgypwsjm.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzczxqmf.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/getkaxjvs.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcfqqolb.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gtcborphn.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaulfirpm.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgapqhmb.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvtvcvxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjihhkq.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gkqmlawxl.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfezxnmg.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiotfbck.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gndrsqjjv.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gringcilg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnsuzfhn.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gbyjfhuxg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/glccnokyi.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ganzounaw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gdnntrigi.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjacduwah.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grgqvtgda.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbhkpply.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gddsjdpgk.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvronuaop.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljqwgojj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbwdgsiy.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gpqwqaizr.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/getsiqxpb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqknnwkdu.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbjvhrpi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnlaczcfg.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsdmiltq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpnylfag.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmugagpu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzptoszwk.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqorwvbzb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gazjxojdm.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gedvutbjv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudogqznh.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gurflpmnd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gagqvoejf.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdlbtljym.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbiualok.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyksohca.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gznmfkubb.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtdyovgvn.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/glnnjzqej.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkafgeae.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncnwofm.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwnxrpkr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gduhddito.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjqfhirm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpvrsyaz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdsdnaxx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfojtshwu.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/genhwgdnv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gewqigrcs.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gjctkgjiy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhbfmnof.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuohvzjj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/ghwbpcftv.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gouuiqiim.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/goorzdekp.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gilhnbbos.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geffhnoin.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwiolpex.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gogihlyte.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gnptosufj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfcaroer.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqnppuhk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gnobohiiz.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golblboxa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpwwtbsf.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gkoeyfhaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gqgqkaxdq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqzgqvdj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gkoegprph.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guvmsyfrz.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbukccuo.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gxtkwpygv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/guwnzrjqo.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gacoyyqzu.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcdkbfzk.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmzrbmemi.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcismxcu.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxarbjkag.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gtddydhoh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gamrbgkcf.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqleaihjs.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtmlhenwx.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwysdelxu.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gdvelrkwf.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiokkoql.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gcbpvfyjf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsszqmph.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/grzhcthnq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpaxngfx.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmhcbjkc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givreklxo.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gnerocvow.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvigyukvs.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gecbiezie.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfuxgpdui.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnslgvzc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gealwskvo.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gjroqsznu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gfdryluzz.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gagunvutp.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvnpeiqcl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gijcflqvs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghivltszc.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdmdhtct.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnvgtmnz.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/geqggxrmd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnzgprqc.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gyoaxvuce.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzijbkjbi.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gdjgvkulo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuskiiqg.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/grshvmakw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbxtdyvt.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gfxdkjaeu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzyudkkp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlnannju.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gscumrhru.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gmjjjtztt.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmgjlojv.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtesaceid.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gjzxrqjnt.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/goaxpjmif.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gypyokqsv.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxppkyyo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvavghrm.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gisxsxgkd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyrhmjoh.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gqchemhax.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkducgtv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhrepgei.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyyefahw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydbypykj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlpvtycw.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdczjmtzf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnybjuwka.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqvaktub.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoioslbd.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gianlrpfl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/grxicmabz.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvxchovlm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjaslhmih.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmphzokhz.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gtjmrcfzq.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gtasunqcx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gosatsjle.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gymfdyvch.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpjsozxz.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghjjuudup.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuioxdnk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gvxdhzkkk.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmxqnpjyh.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gulwefmyq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiaaqapj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/geyfcvwns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzrirtjm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaylqhvl.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gtcgeiado.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gawsgpllc.sHtML


<!-- 参考信息 -->