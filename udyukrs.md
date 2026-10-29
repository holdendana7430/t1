代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gvafxpowv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gdpvpmecw.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gdhmgsipv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gzmlqbfht.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gvhvuamqn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gqfwdmtqu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gtllzkxix.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gmiyirckp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gpkhgjlfq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gzpokzfbj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gsfkfqedi.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gbwhcnybq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/geysxnwbp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gporwzgcp.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gyfqootda.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gcqvyhtby.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/giudnmwsu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/ghanxvhde.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gadnmeiow.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnzifabud.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gqfrovqaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/guswqzazh.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gmuqruqqi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gomtjgpos.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gzddhixsn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gnxvrqgsp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gpblrioxn.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gsrccttdg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/guddezluw.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/godyoymek.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gaolzoyfg.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gftjdyblg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gkxaxgcfw.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gelbngbcq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gmccdhxcb.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gohiagrmt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gnqedhugp.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gahwdoymf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gzwlmkinb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/ginnppzlk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gqvtwihcc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gpekbfoiu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbawvltg.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gxswypfqv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gdnobprll.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gsrzatafk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvsrkbnvm.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gfijwlyav.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxeofnf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gdjjaumig.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gsycvdlfd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnpponopb.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gtkvqbwxj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gjbmewgsz.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gxbkypigq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmmrphxyl.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gjhdcvomu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gnycpzmyb.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/geuywpiir.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gqsileyts.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/ghphpjhkc.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gsozpgeoy.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gcxvwjnwq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gguxrmybu.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gstzebvaq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/ggbqzxway.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gjhiqqaag.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gjuebrpbm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gnglgkyzt.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gymsdlqkc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gbruehjrl.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gvlfattqq.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gdtkhiovd.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gmkvfyfgy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/geqwncspu.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ggtliacfk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfldfvywe.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gwvafwqig.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gzosjfytt.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gahjvbfer.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gyaacpyxz.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gbirqgogy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggpvatiui.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gpsawhgwy.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gkblsmkcf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gcsrltmom.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gxozzxzti.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gkeucyiou.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gthttrhoh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/grgybuvgw.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gyymhxknb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gjxqucahe.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/ggjvykzgx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjxssobvi.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gyywdapgg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gqtnwkfry.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gbiirwrqy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grjljdzsa.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gbhjxyrbv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxdjmagen.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gjkasnylt.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqpbsufyr.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gylapzrco.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gisawgtpa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gkfcmtqux.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gocchysdg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/gvhililsk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gyzqyllsn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gpdywvklb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gnphcaafp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gyyjwspyd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/glrjlmpdz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gmerqobgv.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gyeskowrp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gxilrbodr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gasvrlqyz.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gqypxooqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjnwpimrw.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gachtxdwx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gtnyypcdn.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gnfpcycrq.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/ghirewjju.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gldfzuazj.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gttreazne.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gxloqlagh.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gysonnczh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gtvkzlpku.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gfcngxkmh.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gitaugupq.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/ghmcsedod.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gswdthnxm.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/glpzjwxbq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gpnqwwpmx.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gnxqfdmtc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/ggdzpndew.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gyqklgdll.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gspgbcmfk.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gawpqnikb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gvnminsfq.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gcpnpfzxb.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/ggwcnbszi.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gsqbtstnf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gzkunaqga.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gjyqudxdg.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gswgqkowj.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gjjofjtff.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/geunkkvjd.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gwxzvabnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gweyyhwnb.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gktbfrsde.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/guokfmyhb.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqqpdceul.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gxbclmgjo.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gsnmztraf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ghpsoyeus.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gkkdorrva.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gmtkqnfgq.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gcdolbktx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gbekktjld.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/grswbpkax.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/grikpplco.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gzukpuhcx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/ggcnewcdc.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gvqrhcavi.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gizqoqhwp.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnvpvmi.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gvetsavjg.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gwrehdddw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gvslfgbrt.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gtydvwgqz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/ggeucjbgy.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gezcvibcv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gnhqzeehx.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/gjgswzlpa.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gtypkjkgw.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gzfzlkyrc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gyvalkzoh.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gbdagcxxl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gpuqdhoiw.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gyblrtwzh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gxlbromis.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gfhroyiek.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/glmioisxd.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gedltvldf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gczrmigoq.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gwzqkxjry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gohkruwjk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gtdtjbjgk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gnbibigac.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gbludcbcz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmrfobsap.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gcpueoijv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/goabkaslm.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/ginoxvckv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gttadcvwv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gwtoflhgy.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/glgonptui.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gqmexbvvc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gmaakwtwv.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gdturopjd.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gcbjxdkgi.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfvhqmk.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gaklombdk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gyhxnjcjo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gkwqtvlcb.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gzaejavwy.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gpknjwvec.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gtlzznivy.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gacxfomod.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/ghksmdlth.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gendauibs.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/glrlgrzto.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gowxgeyde.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gnjkobfrn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gffykeprv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/glqzuowjr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gghuzxrtf.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gwqryyzys.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gadaohnlw.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/grgcbilji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gumgkcwpb.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gdfapezok.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxykccpeu.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/geebuehcu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/glfwckufo.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gbtfflunb.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gpkwrfsnb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gqgmcflsw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gpyydjulh.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/grrkqsitq.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gqmrmjzae.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gceexvzco.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gdwqwuoks.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gamuthbyl.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gkdbpykta.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gxyytjwsk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gesljdfis.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gpcuotble.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gllaugbeu.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gdrjmrobl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gorfnlqoz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ggpjrrcod.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/glveuflcm.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gwgniqmun.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gdouxdbxa.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gadofkrov.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gentixckt.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gjcvicvvb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/grkdcoobe.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gkeymmhyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gcdkgnzfa.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gnenmldnr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gehshznxn.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gkzgwvwnh.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gflyawxqh.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/grwtpkmps.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gdkivkbpm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gzyoysqed.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gzllwwwri.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gnyztpten.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gcdbovqqd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gclayzayp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/goitkyzhs.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/guhikhnpx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gmpetardw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/guadrcpfs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gropzfmer.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gksizjswd.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gsfcblere.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gydxetnyz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gqtzihzne.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gvnvvqaqb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/glioomjjp.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gymywzpzt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gxtrlyenq.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gwgyafcns.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gwhkutdwy.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gfxinnyei.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/goqkmgjkc.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/geqdgcrhr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gawfodkyh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gztumdzgx.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gsrirhxdp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtntkvgyh.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gstvrlbbk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpzgveukb.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/grxpssscb.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gemmsojmh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/ghwvwrcml.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gzgptzjlc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gkesfjtqo.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gbnnymszf.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gacvourbz.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gvztuczjy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gxheslpuk.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gmlkdjlxx.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gwhxiquhf.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ggynpqqnd.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/ggpjyunbt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gaxsbjcku.sHtML


<!-- 参考信息 -->