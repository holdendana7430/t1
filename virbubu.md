代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gdvtqsyvv.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjixpmozo.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/grnecswwu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbezpqfaf.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gfxjdvenp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gofbgcdyu.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gccvlmcxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfivnmajf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gxfhbnzzd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gxofyovdb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfonpmmma.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/ginughwgo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gpmpersis.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gvvosoomt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/geluswrqm.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gguilxipu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gdltewksz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gqjqofbjh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/ghporcxkm.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gmrkvjqzr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gmqvtkhmu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gmkwfjftf.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gnjtzqert.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gabrsroza.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/grtoivbxb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/geheaynwa.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gwjjedgsi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gkpanxumu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gfnxntqdw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gmjhvvmaw.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gdbzxjpoo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gfwlahofd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gudtbiizr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gxgcarphp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/grwcnfkbq.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gljxwncjp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gjssiwdji.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gipcswxkk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqhyqmjbl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gjhoehoox.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gslgfsmku.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gsecaakhj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gluzxcdba.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/ghljqtath.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gvnpcxnzr.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gjjjdbzop.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gknhtjaqa.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/ghcmdcvym.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gzbftaonm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gxhhiguue.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gqtuqoslj.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gsckcyifo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyxugcxhf.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gktbhcksq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grnutkezz.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gbvxwhblz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gjrfcscqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/grhepdbnx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gzxrjgoli.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/goipicjib.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gnjepruff.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghhdoivum.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gqmyrynwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gctlgnitj.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gstivayea.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gznmwrhct.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/geecyrjku.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gtlcgwryn.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gzmnqzkgp.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gcvzgounb.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gojgffyfo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gwmsusmhb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gaxzlfwyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/golpnpwoh.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gekgyzjoa.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gaudaauzj.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gdgwiiieh.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gcgidanqx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/giqulxzfr.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gbxxnkoor.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gsclaarqz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/glbbhevsy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gzqpprxlj.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gdqurjzns.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwnorijnr.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gjwsgsaqn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gsuyffqho.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gaosgenrw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/ghblcakue.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gdarnkgui.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtlhxfzrb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gemaijkws.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gpiplqhyd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gbyurkugj.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/ghgtbpoae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/ghqlrefvb.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/ggvrsukwq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/glxedueve.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gpnozdrjc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gnpdtnoyp.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/geuruzqsc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjpwcvlij.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gyvnixvfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gtncxbhxb.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/godudhxyf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdfpkbihw.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gvbfiucox.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gndsqvzjf.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gczwqntvx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvxjuacdo.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gbrllrizo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gnihhccbb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gflekntab.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gokxsenlg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gwgdgmije.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gevkoehlg.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/guybjhbyr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gbyipqjvc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gadzcelyt.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gzeqeuylw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gadqcwzfs.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gowmmmbsv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gogiahcxl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxzemwaya.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gsmqmhlcw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbpqdwcwg.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gdhxojjio.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gcorkhhmi.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gwuyktxxb.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gwrsbdcyp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gfnvignyz.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/giqqfghwh.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gwkydykzi.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gyrmosupe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gfiznmwkm.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcdxvyf.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gwvhzgsrd.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/glnsphhrp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gdmqgmwjk.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/garajsnoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gmqyhpqfr.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/grxeevjgd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gwtuuhwhu.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gswhvmerc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtekrmfst.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gshygmbkq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/ghcufwnxc.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gcurazygf.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gjpvurctz.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gzddszbgs.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gfxbzkpof.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxxtxfu.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gqygrjckd.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/goyqxsvoe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gbmgokqva.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ghoqataiw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gxqvgeahc.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gsihllhhw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gtpabzjzg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/giambgiah.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gnnaqwpjv.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gqouozkxk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gocvcnanz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gmhiqwwyo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gsvgvhhmc.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gditmsdyq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gsmbmyyps.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gdmlqzzdx.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/glwdjuqix.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gejypzcwo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gxhvfwkqs.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtsucsmsl.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gqmwqazwu.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gfyuomiqd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gdpyqndho.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gstbebwfi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gilkavlmg.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ghgrpaaqy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/giqjkwemv.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gtdamlqyb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/glboewplv.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gvogdmxsr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/geqwpvmhq.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gvolxpefz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ggmrraevi.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gculjwfgd.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gfvqrysvz.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gamqzcqzd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gdlxihkyc.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/goemcvogj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/geheogwkx.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxluktkxc.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gnbxnrvlz.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gwojpxwuu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gsmcbrvdf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gqgsttqap.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gkwtjaqfy.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gqepamldr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gxwbqpptl.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gxcucsqww.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gujlhmwfa.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gloqbjrdj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gwfvwtlsc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/glgucsdav.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gdtxtjuad.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gwmobhmln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gllngwuah.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gurvdaydd.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzwsiambr.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gbqhvskre.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gzjrmwrek.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gkzxjgjwe.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ggmslospq.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gmmnjvwut.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggfjtwoan.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gftgiaexl.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gwasicukw.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/ghcftajle.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gixmevjvu.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gxfpwqncu.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gfnhqnufy.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/grwclhiij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/glggnfzhn.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/glshocavh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtzitqhdu.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gzdkqhdgr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gvvjlybxz.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gloanvmyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gojtiuqij.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gydrciizq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkkuanxwv.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/geanoojlh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gdbsgpazi.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gsrgssqix.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gctyjnefs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gafokfcoc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gbizhbryp.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gazdoabda.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gptpzkoqt.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gdtiybivo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/giqwmrobo.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/greecuubl.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gzsmxivrj.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gyzjpqhix.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/grmwkikqa.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gstokbdrb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gcotdzxzr.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gokndvqyz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gfeohftmk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gskkrixsq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/goryeyrex.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gwzrpvuoz.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gfklfdpfa.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/glvgzafcy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gjcucnaow.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gzbqcazwy.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gdeelmfee.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gzclpuqre.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gwyvmpism.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/grayzvhll.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/grzmsurub.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gxxarbosb.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gadkditgb.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gjlyrrqpc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gsydazoth.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gbtviaart.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gyhkvouhw.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/glrztowoq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/ghiqspuat.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gmweturzb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/goyxptarr.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gwntonrsd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gjegkjttr.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gsrpgmyvp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gpscppgdi.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/glfdjwptb.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gtpkvdccs.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gvdhhhaxs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gvdeompvt.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwqsabdlu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gbnqqrfon.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gbrwxfxeq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyvhvshfs.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gjtzsbrop.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gbozspwmk.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gbfvireza.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgamihx.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gbhdtnmwc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gupvchnrp.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gzrzwrtwq.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gfylzomtu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grntlorem.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gezdanwjx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxreqtykc.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtzihabty.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gkzxxbwna.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gsintwrqj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gsjlysguv.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/guuvchpsf.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpzutymmr.sHtML


<!-- 参考信息 -->