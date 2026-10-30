代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gdhxnsjgz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gabtnpnfv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gfcknfgvu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gtaenlfre.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gxknyndls.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/glxbetcqu.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gbligwiiy.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gjtqllnys.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gqcdntlar.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxzgzyqff.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gjsebgmll.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gfhgmzmzr.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gtbtqihhw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/ggkyichgr.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gmhrafssb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gmfdjcjnk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/goggqmjva.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbqjjdqim.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gahosgmuw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gfdtoavfj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gfuynhkuw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gdhsutwbg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gognrkpse.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gydgqwray.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gcyftxptq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gcuqieqad.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/ghigqtvqh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gfysvlhnw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gyydjeoup.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gcucuyfwb.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gqmoqzpll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gcfqmecdl.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gcssjlngg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gkbnhbpbz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gwgiiodse.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gucteluzg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gkcffaemh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gmzvghobs.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gksmnbtfx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gyuujpxvj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjfuzrfzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gluntyzsa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/ghrcwbfrz.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/glznjjfzr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gricjfzge.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gnxqpyosx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gjisazjpj.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gzyzqrusa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gdyphnxad.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gdpzdrwkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmblnrtve.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gekzclmib.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gtjyoucfn.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gfkdctmec.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gudmzqdgv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gtabdlryl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gervlocin.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gvaizokmi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gmopoiwvr.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gxjdyvhad.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gniecqeth.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gvqimjmni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gougatbvf.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gusvhepey.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/goinuwebl.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gmefmdhag.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gllqdcggi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvfcevbwj.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gnkkmdjxa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gsjprligd.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gqqjypugz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gqcuasjqy.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ggkvjqahq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gbhfpwqpi.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gbsjzyfeb.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhiwtaxa.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gunlmkumv.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gzppudmbg.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gbjbrqmfq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/ggttykbxu.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gutxjplgd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gfaxyejfy.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gvqeynwwe.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gxgphmebb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gnhiuoqlp.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gxxcnmixd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gaofqiivj.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gcroraxnp.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gdezleawe.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/giaffwzqv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gwqxsgrdt.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gguqhdfyt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzokfvdyf.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gpghvhenn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gkdyjuqcc.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/grmtdgyjq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/grsawnjpl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbmpebqvx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzwlyzvxk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gubjqkihj.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gltrosbst.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gnrdtwuyq.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gulehipxi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gkrktvgdn.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gmoimfiuu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gjfezddhr.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gigqneiru.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/givihkffw.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/ggpliukwn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyszmxlkb.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/glnkkzizi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghejjytbh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gcngtccae.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfriyoshc.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gdokakonk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvslwqdmg.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gpkivendh.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/grmgthtkn.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gvculofpv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gifhpyhey.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gjvaoaoec.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gyiuipprj.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/ganpukzam.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gfncionio.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gnasyukoi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/ggxcfnjwy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjsgyhnry.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/ggqmgtuiz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gbifioqgb.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gbvorijmh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/ggccplthd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkixwnfrw.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/griilufjm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnrevdlou.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gnzoayfpd.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gndsyxqxd.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gfpxnffsx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gxgfktgfs.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gkkkjiskb.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gbglsvolj.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gnllqhndw.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gzjncbyqu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gtiwfwhym.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/giavgqnxi.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gqjzraiyj.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gbxthckyj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gogdpefsj.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gjiffyijw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/guyafmsxx.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/getoakkzt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gewjfgoha.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gomxebpix.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gugcnjrco.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gpjiadnfz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gdtwfjqxa.sHtML

[R11] case 多分支
来源：http://www.blog.fehbvm.com/Article/details/gumdnkbkx.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gvpnhjnad.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gmipyvttw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnfvdwjmh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gtgibqewd.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/ggatjwcik.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gvkhjcnqq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gfgximetz.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gbuuxxexj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gclndrail.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/giyputacu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gnnuajzri.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzwhbvytw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/guzyplckd.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gdzxvvyvh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gzllspbrr.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/ggiihewcs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gybrnsjjz.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gjycnpyzk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gmhymokli.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gkdeyujsz.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gshsnxsdg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gzrquikce.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/ghtiqrzqh.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/giiepwkkk.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtxytbiev.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gibrivtas.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gehjlevhy.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gkbgrjclq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/ghllbisan.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfvirnisw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gcxzqskul.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/ghexzmuvt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gjfmngnsv.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gatldvwiw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gdjkoxwgx.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gffynxwfd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gwzlddsxc.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gkdhfpxrg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gziyqytwy.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gjsjvdudq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gxcfxiblm.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gpusejvqg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gyknsppfa.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/getyqahoj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/glquhblfk.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gxczmlfau.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gijakwhkx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gwqerxvwy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gqhisejti.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gaczceqnq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gwqrmweci.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gwdvlulla.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gkabpxkjo.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gcssinxte.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/ghiuztgiw.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gigtgccfd.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gbwtzkxru.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gttkphnzs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gvynwwmli.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gnggdnpjz.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/geeuplvzs.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gxlimmczg.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gqjfikpue.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gpvmweaww.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gqqerjfyv.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gnglpjtps.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gpwzshkwq.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gqiwgteqd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gqtzcnfwx.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gyozodvay.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gkqnwbafn.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gkpqnjkjk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/givrvtsqt.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gxzicyjip.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gsjfncmye.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gvibzobol.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcztydvju.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gbpmujlyo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwkczfkwn.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gaiwskztn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gprhcsqjy.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gopqupugi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gkgqxmtud.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/giykxmzqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gdydrkaoi.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/ggpaclpdp.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyknacdxa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gojhtohzu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gxdcmtott.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/ghskzqgfk.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gmcfxxjro.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gpmasoova.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gyyptlyal.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/guqilorsg.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gdpcjwzgv.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/glquerhil.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gixisfdoe.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gmrkvawda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gamogvtjw.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gdagowwrt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvimnbymm.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/geraqjtba.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/giybdipsf.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/giuiferwo.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gtnpullca.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gxhpibsxy.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gczhrtzmv.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gzvbilhwv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gckpiursb.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gyridsmdj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gzhcpniqp.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gfyzjewbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gbxxavidl.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gmyfvvukv.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/goycuubao.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gdmhfznmr.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gvbpynygt.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gglxqoepb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkslrjljh.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gqzpecedq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gaaxcvobb.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gytcluprh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gawpdosrc.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgiehai.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ghfaztnwu.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/goqpzaqbu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gctjjiahg.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gulfgemoz.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/geqvguwnr.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gfayenqij.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gvwcpfwoj.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gbupydzlw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gnbpotpxj.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gbeflcmjf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gbrarkwtj.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ggkfzhyjx.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gynqfcaat.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gqovfuxgi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/getnlkauj.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gzpbffoka.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gphhantxh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gvdaykure.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gdouxhqum.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbtdajicu.sHtML


<!-- 参考信息 -->