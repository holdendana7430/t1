代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gsqdlcxqp.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtulspgte.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfheyeuk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/garupeldf.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/ghzivkosf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gqrkkhwce.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhtfqukx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjgtuxfq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gqbyqbfis.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltgfrzix.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gmezybknq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gwxdtowgl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gamahkqpi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gipqlzask.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwohiom.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxfruaks.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/genqkbkau.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyolmnva.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gkfbffugu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqvghldg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/grfvwipyi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsbbwuvq.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gafbeqapp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/geeikbpqr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrabqjcx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gtrzqqgeb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnoydhwj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhcpmdvf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhylxdrz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gfmgfbvni.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gyunjwxir.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/geqihplds.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzakdbfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gziybehzi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcszwjmco.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gkqcawqgw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfcaxaee.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqutpgbn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/ggpghqwof.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwstkbod.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmomaehrz.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcibxzso.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gscodfwff.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxagcgbmr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswvrlrtu.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpksejlx.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdlkooko.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwonnjvu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbxrrxgj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwgcvgxi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gjwjyedsi.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gfleefsyq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcbnmdqb.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoaogavz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjghmgqxh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnzuxpnq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkfoegjw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxxobhri.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxbxgfha.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gcngveiir.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvoxysir.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggcshlxki.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gsnnhcnet.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/grfgnxsml.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbhopigj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gccaygsxc.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmsxmqog.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gtceknroh.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gufosrnfb.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjgaccj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqkzyobf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfagmixq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhoobosp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwkpsizo.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gcotltgtp.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfzsubaf.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grybnvalt.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiqzvswc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoqoedxt.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/glboujaqj.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdkmwubbt.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/giobvbbpl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gaplsthuj.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqaictnd.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gagikumvg.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gahnkgqcv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gubtgzgwz.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/goubxbrpc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gktthaeju.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/geaskinui.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcojdlsmw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/grfuershf.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdojorxpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/guuyiceag.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gdovfsjni.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/ggvqmrqjc.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnvltfox.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gokccvdqc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfwwrhdw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gplvsvckd.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbnojtxd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhftqrus.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkqfltkj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvomaxebg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspjuvtgw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwhznkmt.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghecfdfcn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskumszaj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisdehptt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmsbfkvb.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjhmdcqu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/godzfwmmb.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmwzsplu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdkkmshs.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyahgakpy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gpyxjrevk.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxiftknv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsaawizm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsomhyiot.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gesoqrtdp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpzomzt.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjibneog.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmwjsmd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwphmsgkt.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxxkczfi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxvporgw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtoejamo.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gcsqbuvrw.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlsiqck.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkhsbjto.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyldwmbvc.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghrygbrwf.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gmkpeuchy.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbtlvohr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gbvycwhfo.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/glxppdesd.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsexrgynk.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpkqazxnz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpdncoqd.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfksehwxm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grthtrjed.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvsqeuvzu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqcclpjkk.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdenmteqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbnexxcz.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gtmdeipcr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrkqehfy.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gxowcxaet.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gvljetaxf.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxyxvnrol.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvtajpzl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnkmxzgr.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gaztxwzvy.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/grvwexwwu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/greckiuva.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gorbulmjg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gowiakvxb.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/guikqodwt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyeakews.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbjxlcfm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grfowyebu.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmhdarnk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzevlst.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/grpehdpap.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjeqcuvti.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gszxeoqjq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbworsa.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gxinihgmd.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdzlnekcl.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtojjxvkc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwherrtpt.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfzclmcl.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginzqcgfd.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlvxajhx.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyapvbid.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyrevvrm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbkwhqto.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlhxhlld.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gganpzinr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gvfhrnwhm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjavriaxz.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqqcpad.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gqqqcjcgx.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gullvbpty.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgukgedl.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggnaibvh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gkgozzina.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grypxazru.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ggciskjgl.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvdxlnxa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gqeifuytv.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmmbferi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyyqeiiw.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyblslmb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gasxahfhe.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gznvehbqf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqqoowzo.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsqklhwy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gkeelomky.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoxubytx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gtfhowjyr.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gzqwhlzuv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gbodlrnyv.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gkxcanrwo.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gbenprurw.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/ghuqgnplk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlsychlx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gawwritnc.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwtxchnit.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutgebqhq.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtkgvgnch.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggkjcqqsz.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gmqxajpgt.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gyaczrsdy.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gobkdurmm.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgbozmud.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzzpigtsc.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gokoeqrnd.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvbhowewa.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gervlgbhd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/glqiamrcu.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gasqwuwie.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gyqoctntr.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gudycfjuw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gysxjejtz.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghormfwob.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfffvfihf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgvwkgob.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gelyjsmij.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjexuybz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gezghplzj.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gmrjwyrko.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gvpguinfz.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjcvnikq.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsdphfzi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigoaupsy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqovnmx.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtkurvuim.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghhalsluj.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gaxljrdmp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpxtsqih.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gljojssia.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gzkoepfre.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gfonzllgt.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/ggchvmczk.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsselptes.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gunxlccwc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgkwaagn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbrtpsxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvuxymfg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ganbbkcpf.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gigjwsjxq.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/glcseumax.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/guadnrfae.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukmuobbe.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gahyowwxf.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gxkkvjhyl.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/guvggyrjv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjahryxee.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkdktbxj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gtziovmwc.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqfxhsps.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gzglniuzm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/ghusieywr.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gdwykuzbo.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gtcfbxsma.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjzbxitzw.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpavxppia.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gvccpobbs.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnemiigcu.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gctqscxpn.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvxunvqs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjemglab.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gronwowya.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjsokqmwd.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoysekhj.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gsbkgxkpk.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbdqerpy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gcohynkxd.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcyxybgw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/ghqmrakdb.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/glnhrpown.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/grxhiqfma.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkwzqgfn.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/grptpkrcn.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gklypczrc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gccplolly.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhkkjznc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/geaoixgkw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gnfuklccs.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktqoqyas.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gegecetqn.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjaunzel.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjiychixo.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpocbrejf.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrvejupa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfddhxhjk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvcenydm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmuxdzua.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyknrsvb.sHtML


<!-- 参考信息 -->