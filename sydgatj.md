代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdfqcgsm.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggxnqpbeg.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gvryfqoeh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gokooehte.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmkewstn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/geipozefs.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gtglfuadd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrwowbtn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gogdjfytn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gyyfloaar.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gcopfqxcn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcaamytl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gylaakrcz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcjnsmsj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymylwpnt.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gehtysmxq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gowroxpii.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gyfrbsrkj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbblnijo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkesqzck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gjktihlqk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/grnbuqnzd.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/guqsaenkl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gunsmsodb.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gugcsvfec.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/gceqbgcox.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjfishnq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/ghbkkydjr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtxnkkdd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtdnsowe.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gddfrojrc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/groyytjsq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/glrihvwmx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwjjrmc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjrisubx.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpwvedic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghrfohdia.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbndlagi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gtqjpauij.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftacjen.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gteapuabd.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gsnbtvhkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glprsjesg.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gwyudnqrf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqowtglx.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/guvxwfzvm.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlinghpa.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgzbzvmx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkgfxfai.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnyiocsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxatadouk.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gyicqhiyf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggedtopqv.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvpuzuxgi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzjyqgnp.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbluzrovw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvgddkdj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gotqreswi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuypbyso.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfugpiyo.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunthftg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokcothiy.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgxgptsp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gevruxekv.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/ggelqnxal.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjcegpfk.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gprrpjltk.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gwuphtmhb.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmgpuki.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gumhgxtmm.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvaerlpp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gizucpngz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gesjhxoqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/goupsjmoo.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gsdptdstx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqtbaunr.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbitshecy.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gsanpshsi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtssmlfxs.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxuqjlv.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkgrrdowq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwisofl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gphalevzl.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmdiegpsp.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjebsjfxa.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/govzutjur.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvephzxj.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkvdgdvl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gzuzniori.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/grhuatypk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdqouqdfd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gizkrrzfy.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/grvnxtvzd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhsctsuw.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/golbnxidf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/giewmlktc.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrghibpx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkddivgf.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gvktpewla.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmpjkwyd.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gkfszaeci.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmvjdxkv.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gyvumcizw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnrnxzcm.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/geruekwmm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfsrdpdie.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaddopvxz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gvkzpvtvi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjtzhxjm.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpfzvgagx.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/ggeahcxtk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/guudqwccz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtebamzb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gitsozior.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gatryouqs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvqlzcwa.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gxhodmrad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gqnfdcmef.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gibmfnclr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gibqqglkm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdanxacn.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gtiubllqd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigstcbvj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdbmstiir.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwmfoayd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcyauywa.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtncsbsew.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gfahjveua.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gptdpqelf.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gbitijokl.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvrvcurdn.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnsawsitz.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gylhtgjyx.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmowqucic.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gcitjpxcu.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqwsuxaz.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfvefjljv.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvslrzwj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpwoyzir.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwrjxjutu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gzlmgongl.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gucgkljiy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzopsldjb.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwsthefr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/guhfhcjku.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gqhkfzliv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjubcadm.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gyxftempk.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gpgqtvomu.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gmtacpgst.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpczcqwn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gidsxlzxl.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gcjgrqmty.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gswtdhwzj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrqyxhdp.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsjixhwgp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjckmahux.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gzjuipjhb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/grbbxfcil.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcwhfkjg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gftfngwwr.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwmqaohvf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcnrgwamk.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/ghrtoeisr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbexvdwr.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gldehtjsu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvxyzoft.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqzpffqx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnnhpeii.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedhkfvqq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvjlzcke.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpligmdm.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gedlxjvey.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/grssexqyt.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glzkwljou.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchyrykor.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvvaaeiy.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/grgfibuqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/genmshlhu.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gitkexjcf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnvliytg.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqisrhqk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxpdiew.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/grmcjakuh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbczcvmkf.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavgzmko.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizrsdan.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkvdrblm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmyencyt.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgmdyoau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkopfyfsb.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnkpihjy.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxypbmmt.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gwzsdtaff.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidhesuon.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvauolob.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gozxgzjzt.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqlsekbw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyhbndca.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gtalmhxfc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghklceuef.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/glwoqatrk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gacgyhczz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsdnwjiun.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glxfvcije.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjflssa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbyqifdu.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gjcnmeqra.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ghnycdapu.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gxnehckxa.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/grrdqbofq.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiawqmoj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeuqvcuj.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclrxrejj.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gemmvdkfc.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkmhnfu.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gggjzebdg.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gegyxjtuh.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gzuudujwk.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gbszcomqa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gutjxsiir.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gycjbalww.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwmrrik.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/grdhpjaot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gaizrfmul.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gxgxmgpxe.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/guopwzlef.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/glmijxynh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwaqljii.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhmkfuu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmuunenmv.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhhmgbde.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvnjxtss.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gxbtdwfvq.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydguhqks.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvhjbmagz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnkonixh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvghzjimr.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnczjqmy.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gruuyfsja.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gbstrhwhl.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxecaavsv.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gohfredab.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gdzhacrln.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpjzoiuf.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkschfzo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gsaqlgmjg.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/ghafauicv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gzwghtebg.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gnexzufuo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuifmzpq.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzicktmkk.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gizffgfrp.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjbtdwad.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbyndcyr.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpypkrraa.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgoosrbm.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/ggkmmdysg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gviovoayo.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gzqxetlme.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtthgpcu.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gelpwxdaf.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlqbfeeh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gybektlcu.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/guykrsxlx.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzemezc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqhrkaxk.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbavtocn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcpfcwx.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gehkcjulk.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzjogaaj.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsumkxre.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gmsmfbmnj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagadjowr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvwmkotgb.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gufysadyz.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/glqvseprl.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gglgazgfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gprxcogup.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gelgoebyp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gghfxcblm.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbaizoocj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gclsbeisz.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gcchfzcev.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gzqnlwgne.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gboownoci.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvqwvept.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzuckqnx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/geeohpliq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gislyikxi.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gowbhhewi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyetrzvjn.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktjymslg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmqblmsi.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyfunypt.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gntpndysd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlkjagea.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsbdkyya.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/ganphuuve.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghehtoywa.sHtML


<!-- 参考信息 -->