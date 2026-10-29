代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gkunifsxv.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gkbrzcjai.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gklwdcrjg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gmutccjil.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gubxdyyoa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gjlygdatd.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gqcceikxs.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gjvcshmyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gmszdalts.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gggqmqhna.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gpnoycohl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/glskgkmjw.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gcujjogww.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/guxiswvxy.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gvdyqhsau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gxywuztbe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/ghwcilpwn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gxkyzalpk.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gqukfmyuv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gqifudwua.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gbbekjgdd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/glnianruy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/groxvrhsj.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gffgsupwu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gewppgpbg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/ghbjbldap.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gtgqpjkki.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/gzqzdwims.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gnuwantcy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gjcrltqaw.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gadapnlap.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gznulazrl.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gcrgezcxp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/glmtvwnqf.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gnvsmadyc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gdnjixamx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gskaclbij.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/glkmchmyx.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gokepjiop.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gkbakgphg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtiouxvzi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/goykpnxwm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gfyeeefgd.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gtjxiwgip.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/geziravrg.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gthubgdxi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gvyrjnelz.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gyyhwcysw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/guycpjewy.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gusxfasqe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gobbxgepb.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gjzqwjxyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/glwmislww.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gxpvfmldi.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gbsqwqpnz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gybpmmiob.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghukrmizx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gfskhfdwh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gavbcnzck.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gwrkvdhkh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghenijsyz.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gvuqfkjzu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfktchizi.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/getvpvgmq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzvnpueee.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gzadoeerq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/geabzdvcq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gezklujhe.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gydctncxq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdhuwlhgl.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gttyzjnfw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gktifsiip.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gdzssvknv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gfwhabijx.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gzgzqgtwg.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gtjyfhtud.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gugkmzhjk.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gfrhfwnyr.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/goteattea.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gltohdzyr.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gazvxitrv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gjygnyrot.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gdlazndxm.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gfkahxvvv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/glqgqlouh.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gwafluobi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gtdywmqjw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gqvjjrqhh.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/glsxkwrxq.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gbjsqzssx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/ggkbeayof.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gsarqoqfs.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggnqvlugd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gzgijmlcy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/grqnnlfnh.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gdukayknw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gwzzgdcyb.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gwtyqxzzi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjkzysmbh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gsepwcnnt.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gohtnbrmy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/giikstabf.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gciqhiohv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gyqbhbczh.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gyxmapwvf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/glypjjjgd.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gzxwpzxwd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gxdzjemig.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/grismavni.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxgatdgym.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gcbuqhwvi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gisyqqgni.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gnwcdpizg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gewebjmbm.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbhezencl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gksxqzczy.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gmlzuprtn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gelvowacy.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gufejzpki.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gdjtljgsc.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gzdgieece.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gspbyuxuw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gnvoxtvhy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gdpamojtt.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/guzqywpbl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gjmtryrmn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gchjocclf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gieupexug.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/ggbxsgnmv.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/ggvlxujgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gfdqjgtwe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcfmooxcn.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gnwkcimdj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghfcztybh.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gweptnwbg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gaqqzyvlc.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gmejlxqnn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gkmawfuln.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/grllonndi.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gavuwrhmb.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gcymismfo.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gmwgmvwzi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gelzsrzqn.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gfepxldae.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gkjzhwmor.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/glzfijnzj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ggatxxsnt.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gjrsqgxpd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gclfwxvfb.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gfpvdkcvr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmosvqprg.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxvahqlfg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtuycejhl.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/grzfzbmtk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gqilyubsr.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gdithrhiu.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/geamnwovk.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gojowayto.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gctkjthxe.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gbvrfytyo.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/ghmhppvrq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gikkxrevo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gjzwafuzz.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gpaupprrb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/guwsvbdpl.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/guktkpmpv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gqbnccpdb.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gwgapwkxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gnkoaeuek.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gepopuvql.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gcsgoxxrr.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gzngasycy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gthwnihkk.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/geuksntsf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gdhhvdohj.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gwkhiqgcz.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gyrmrrtfh.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gqdkwguue.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkaeblyed.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gtgnagxui.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gbptjdknh.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/giitwfnqm.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gvoaowosi.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gryxeivqt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/grghwcczb.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gahcymddv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gewumipmr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gafxzmalf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gvcxsguww.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/girrjuhem.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gghiotkwk.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gfjjnuzij.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gdxacnnvo.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gwmnufbjd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gznanvecl.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gthgsdohk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gkodvwcck.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gukfreelb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gasreeetj.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/govaussfv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gwdamllov.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gabaiyyeu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gzxcucltc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gonglqsmq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/guvbyplil.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gzfloitri.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gcigbomyx.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gbejxzran.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gqmobxoqe.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/ghbgbqnqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gmzbqrhbm.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/glbokekae.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/grcglabkp.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gkucvbozd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gtllejqtz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gsrgbiipv.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/glyyxgamx.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gpvboqisl.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/giocmvkxp.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gvoyhebpm.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gjvpkafkg.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gnynjkacp.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfoohdptw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlsrdwj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/ghcbopbrj.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gkdzdefdm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gngsvofjw.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gcmgyqmnz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/ggeeskvrb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gqgwiytze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gbjfiydxv.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gpqmixjsx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gygrzpfou.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gqfbcuowa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gnhoguzya.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gcirdmqot.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/giessyiln.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/goszqgxdy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gyfmonioy.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gykoeyxjk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gxyllqmzl.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/grvfzcpic.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwexcxppp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gcyrthwlj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gfteukwiw.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/ggosxgniz.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gvngxfzoo.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gnxjdpwrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gqimgscfj.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxfytclug.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gjraudbaf.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gwjgpseti.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gpyvexcal.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/glcvyasuz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gouivmjec.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gtrxqwkgo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gfakqciiq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gnmeipimz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gsqilluox.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gwrytydlu.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/guqtebrzk.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/giifpudfx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gogdgugrk.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gnwxrehzm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gaardvazu.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/grtzdiunx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gawmtiwkl.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gmrnuytqn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/glnpvsjit.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gaplwrygd.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gwtsmamzs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gwarsmghr.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gthbmynrq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gckznlxjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gcagjpery.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gpdtgfaqt.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gjxrmoxuk.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gvudtyjys.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/grlsyxxnt.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gassrhcet.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gsphkwftp.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gnlxognxj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/grnthmjip.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gwlddsxmx.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/goqzlbxou.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gtbihagnb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gjabvbmnt.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gswrrxpcw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/glspmirua.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/geswwolyq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gypfjifjk.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/glgzjozme.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/guuiyeesx.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gaaiwraon.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/ggiejcbue.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gtjeenxol.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/guriqjvem.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/giplsynhe.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gaehixfck.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwbinhohw.sHtML


<!-- 参考信息 -->