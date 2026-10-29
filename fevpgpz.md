代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/ghodrlqnf.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzrzeuoeu.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gidndsvik.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gttivnwga.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gxsqacgsv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gsvxhnkxr.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gukdamuem.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gcbfhnybt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gplpdzpmz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gnvnztnhp.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gqwvdawoy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gkxwefpgc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gfunernwo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gpvcymytd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gvexeyupx.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gujahawdq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gggpjhzkt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gosozisrf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gqflnrxnq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gmbgqatnh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gunvyjvcu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gialvlngv.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/ghphkowhi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gvqoyyavd.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gfbkdrwjp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gglrjcuwu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gltbaxtms.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gonrwgaxa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/guwenvttu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gpaqgykql.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gkbtcpror.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gcgwmcffl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/ghwnbemhc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/ggleuhmyz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gkamlgkxo.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/goifgyoec.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gpitxglcq.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gcmlyxfbp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gmxnabmxf.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gcpvqjkrb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gbjephaaz.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gmmxswsip.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grvqxjhxu.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/glekxwhdy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gostfgjrt.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gzilzrtmk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gwnkjnpjt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/goxrnpoby.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gsthkdwjp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/galruxsog.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gsjzixwnf.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gsqmlfcaq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/geeldpnew.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gnubdrcnq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmnnzzqye.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gyqsshiro.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gynjsdhuv.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gbnzxjxyh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gprqocbpe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwyqfbfzy.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/grylezzif.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gfuetyqgw.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gfcihbsvj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gzewyvpcm.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gtircssoc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ggerfvjaw.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/guigfvljo.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gghkrcngg.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gvynrqlmc.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/guldvnlpj.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gaxjfrzfe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gbgrgugxo.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gnborxsim.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gjizadcwp.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/geblwjgrt.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gnvmbeymo.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqjairxng.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/grjwcfmip.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gnirbljvq.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gzdocypep.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/grghnnkpk.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gnvzuyhcd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gruhslmjc.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ghuorytpw.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/grghhwpdc.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gdwbcxjlg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gmafmiicv.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gjznviueg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/ghyojtmah.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gvkbzixwy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gqemtqazm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/grjbshkuc.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gnpymbphs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/geaadxkck.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/ghryfkihf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/guaxhifzq.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/ghrrwxfyv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gyuivsvfi.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gitjdfuwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gkuyaaxdq.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gqnfkjcuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grhceoxtd.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gustfjjct.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpjxwkdqk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/glagvnqlz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwtxgsagj.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gkhmyxgtp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gubvhngjl.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gmjzktfib.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyxobiqzz.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/ghuqjsfuv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfqjacd.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gtnyebnjc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/ghislssjf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gmjucjtwm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gpsbmojki.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gusovnzvq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/glehvxudt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gydzlorvf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gxpwlzugb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gshntsyuo.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gxeefofru.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gqqhdqaxj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjxdskwcu.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gqaonckiq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvksgpntr.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gmnobyzrt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gqjsgfssd.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gcqaenjti.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gokrhcceg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gripvkbud.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gkzydlbbi.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/ggcmoihhq.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gtkhiemln.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gjqeobzke.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gvfppuoua.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gutnedzjw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqabijdcx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gmgunmtnj.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gwktgwyrs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gplijugtg.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gnnqljaff.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gckwkvsyb.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gcicoruah.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcvuwwihk.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gxmxptoaw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gqhzysvai.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gnefzdfma.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/ghdittypy.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gqtbhotak.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gqubmpfla.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/glwtbtjlf.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gqpyktfzu.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/grikprpif.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gsbmxmvfi.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gppdlpcox.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfylgombp.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gvxwsyixo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gehovysdn.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvwezsxrw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gteytflmj.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmindot.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gfsqopaqa.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/ggmoxqiwh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gdoahvlxj.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gaxdqfqdp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gayweivgy.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/glliuggcf.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gpyhrpkje.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gnlvowbzp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gntfiguqv.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/glqilzotl.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gbfyhgpkf.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gqaziwcxd.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/geyjgfrnv.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/grzzggfbn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/ghebmnmly.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ggttfouge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gfzimoccs.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gmlbqghji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gvfbiysdq.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gwnmajinf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gghjcdxwi.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gndwadimz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/ghqtsnwaf.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gwntsvihr.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gxyjtjgka.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/ggnwluqvm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gxplcfqbo.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gyjztjqez.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gmmtwhedh.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gloemiglo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gcgolrfps.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gtdabochc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gzhmiudkx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gvuhfhvgx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gtloovfgu.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gutnhxlka.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gruoqfzgr.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gbruzvoei.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gwlxzdpfe.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gzwcnovbs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqgvqev.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gzwmxsbrx.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gxqolywxz.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gqoepcdwx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gempwuxxh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gggtazlif.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gtolzuqyn.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gvpvuwnog.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gurzdemdq.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gcbgjmmvw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gvuuxifyy.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gqwbixvnh.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gnpsjnizn.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gtiockwjp.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/guefptkra.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/ggaughpen.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gpjlovkyk.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gbcxqisen.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gtrzogvff.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gwwimkkjb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gnqjftlnv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gvevevhhh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gghkflhve.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gbozdcyyu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gnlkvcoaj.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gtrzxrdzi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gfdsiweqx.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gtngfbugb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gvseezyon.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gsonlndud.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/glnrvucci.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gslorpkzv.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gefktgsaz.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gxjmtused.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gegqtlndp.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gfoirvmtl.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gdvlhxuiw.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/grrvnkcfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gcfdytuuh.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gfxctlmdg.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gmdzbiqky.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gslbfuvrq.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gnceqtxws.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gqqgsclcn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gklzqgeqq.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/glafpfrus.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/guxqaxbhp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ggxjwzjit.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ghhgeawea.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gcdcigdaf.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gfxnncqgl.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gnoaiiyhc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/grratjeys.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gzblkmdca.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gampzpngi.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gqulfaunj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gdiongsox.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gmkzlyvhq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/ggaocwcjc.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gptotihjq.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/guvkeldop.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gqtydlnxg.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gzhubeaqf.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/grozfwkje.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gteclsbgd.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gkmsqfbgm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gltbcrybs.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gungfgpla.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gpfutksuz.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gbdpgcxlk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gxgcflyof.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gwixkieyy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/ggifapwcd.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gwkbqfprm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gspiiqund.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gsebzpwvg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gfhwdyrxf.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gxsucfnfl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gcesndvzk.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gcdlpsfai.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gfaqxiwfd.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gajielfci.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gdrzuvjew.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/glvikvnnk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gvemstdnu.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/ghcodrpyd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gkeiudeqm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gwqzsorhu.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gypdmxstx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqffohruz.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gwunqatpf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzqnkydwt.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpivjivjl.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/glaqyhxog.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gxnewtsiv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/glkdqismm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gnlydyzva.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gwgnpkwfy.sHtML


<!-- 参考信息 -->