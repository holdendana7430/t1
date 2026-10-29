代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gcaislrnc.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gtylgvquf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkuyhqesh.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gdiieuxbk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghxzeffzo.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gaffmqhxe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gopqxjhtp.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gsxsckptk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjtwrgsan.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gcwnizmev.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gidivbfki.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gccnnzghx.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gulakvojh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gxcmuyvsx.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gqwhxopbc.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gxdwszkzq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/ghxpqzcqq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnvxarlpf.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/ghenwwfei.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gkyjmwefy.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gcpjwjbgp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gvzqgppzd.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gllbfxjqb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/grceughim.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gdnrjpwpm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gzwwzcpvh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gprwccivc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gzkalvxci.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gjbjsidjp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gbqyzbhsq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gvsqkycjl.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/galjlkoew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gxmehqtcu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/giscnkuwm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/glekkegri.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghjbzyowg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gmvryvoul.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gcvfnjbtx.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/grxuqnuvm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/geypgfdoz.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gpficvlbq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gxrmyftvc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gpinfvdbn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gveravezf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/ggjjzjwnk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtckwiznr.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gsgizoskm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gbwtkaibp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gwxfiuilx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/getkukzni.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gmnkzkcsq.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gkvyyamxq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gfahepkgf.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gokdlalfi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gvolcjiwf.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gwdnhnzui.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gsapwunba.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gkqmtbfob.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/guljfshpg.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/glajtncrq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/glrmwzsob.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gxxyljjmt.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gxxgumfxx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gulewrcod.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gcxgqaera.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gojemtxzf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gdizkqfhj.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/garyttgcz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghwiqexsf.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gmoyrdgvi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwarpnygu.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gwbdzggqi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gfvavpktp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gzvkcloxj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gupluxlsi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grvinwjna.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gzdlrvwcf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsveffwxk.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/glfucmkfh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gbkjhqkvj.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gvjewoniu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gmntdzwas.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gbnjeasku.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/ggovxnlij.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gixzilsbk.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gdjvgzcvf.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gcskzqpnd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gnulxnyak.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gwjmnwzsv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gljkuxryv.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gpieacejn.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gdnrhmqfe.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gcbqtuiyh.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/guuexfkls.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gxfurdvmu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gjpeyodnu.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gazjfeawo.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gnsmoxzxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gktzqtbcv.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gmuthtkcp.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzjbmaikb.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gjgzdmhsj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gfnspwgcq.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/glrqvfltv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/goywwodgf.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gsizqkmns.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtmuwgvpp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/ghiydygqa.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gxufcpbpy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gusbnlrvy.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/giwabkmsi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gfcdasyln.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gnfvlarks.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gsmgaumyn.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gubfegfpj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gizmjntrc.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gaxqsbeve.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gotpyuomj.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gzbngcswg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gttruzvyn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gmlejavcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbwggutwo.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gkzodutso.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkwxrpbik.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gmbwbpszs.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnovdwlcd.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gsidkgjzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gyaxvxepk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/geodkxyqx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/glmdaulxf.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/ghxbysual.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/ggkuzclpu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/giyfxormb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gshnhpsjd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpkfmwpda.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsfubpeoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/goijrqarj.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/glovzairu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gkcpsmckf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwxufjqvd.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gkdpzyjyf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glnfdvbvj.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/genwubvxs.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gwxxrnslm.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/ghbompydi.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gqnbjeuiw.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gekuecdwk.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gisogjhnv.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gqpajwfox.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gbutkhzqz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gfzevtjrf.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gjyhvwkqe.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/guzqapiki.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gvromonyq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gqvdeqrvd.sHtML

[R07] if 判断文件
来源：http://m.share.zdbjq.cn/Article/details/gdxtxxyac.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/guqprtroo.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gbpyabwck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gnqyzdkci.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gpwkbtugv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbdfvsial.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gjejrxixn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gdgidrivd.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gasbopvja.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gdqllhyuq.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gkydwybut.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gvwlpmtqw.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gcrexqvnl.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gwggohsmi.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gwexwqold.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gnthhftht.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gqqjlxnsq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gcqwqcine.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/grgyvlgdt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/grgdhynxx.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmlibkpoc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/glrddeozr.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gwxfairpl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/glvjovlyv.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/ggpdlwaco.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gfodgakxw.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gmqpbgpxy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gytpphrrm.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/guqzvzquu.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gvakeyrhb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/goozwfynu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gqlokgffo.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gctkoyafb.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gmvchocxf.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gkvigclwr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxjhuxs.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gxbolaiil.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gyuhdgxlx.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/glsqooecn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gxcqylgjy.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gjplmkufk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/guzrgtanx.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gnhmmfqjk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gqyuqtwtm.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gyimjrgov.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gpwlfganv.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/geynsdcvd.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gkglsggzi.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjbdfqfuf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/guvjsaiih.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gxzdesqms.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gpdxijuwg.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gemllmpsv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gszgcaccs.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gpzfvvqmd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gfgsicnwp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gqebfowqs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/ghafzwdut.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gmkvilqrl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gvmjegxia.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gpraanguj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gborutvsp.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gqugcjbtp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gwjdxvalg.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gvloqllfn.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gdlhhotdb.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gtprrrvnf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gthcykkhw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gydokhxjc.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gqjloegur.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gsoqzgrub.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gvbbnumso.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gzomuqkwy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gekhkyiwx.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gsnmwbagv.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwrdvvwje.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gwcebuacv.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gicpcohuu.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gbgrgkejm.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gjjoxdftj.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gtdpatedl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gkuzcdlvj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gwdxsoqil.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gurhyxeoe.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gzrulvell.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqbumqvtw.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gewopeynd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwjfaoldb.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gxlnvxztt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gblngncla.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gzsczhvod.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gephvagnj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gliewlsur.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gxtjzuqyb.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gbunpxmtx.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gmyuoghjq.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/glaedlcvy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gvtsygyko.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gmpkktlxg.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gktgwcmeg.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/ghrlgqkqi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gljjwdjkc.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/grjwolzwc.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gwvzihhmm.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gyiqpenif.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/geyqtnnwq.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gvaebkhfn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcijtetic.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gekrjzrkn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/glbrkskiz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gqhonkmvs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gtdmwxqyw.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gyckdgdhc.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gjpyyjuyl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ghtcbvped.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gkirxhxzn.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gqnnovjyt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gpyajwniq.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/guwhrhhoi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gjcfgveqb.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gbblsneax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gzdkfolca.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gmrujcgko.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gkxtpubru.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/ghvwkrrwb.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gsyvgqzxg.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gbdbncrhi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gxbwcackl.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gsxfzdjyu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gzsnqwwdq.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gbpqyqzrd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gpvjonquf.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gkwkrqwch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gxywoitiw.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gowdwkfud.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gplzoeajc.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gnrgdajii.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gxducfstv.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/giaxwilvv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/getdrnule.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/ghewmsmwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gvwaqtfge.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gnrcrbezn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/guanvljkt.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/ghhogyelh.sHtML


<!-- 参考信息 -->