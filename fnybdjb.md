代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/ggjxgzybw.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gopbyouks.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gkssvbnbq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gulojhvni.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gkmlhunuo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gjhejshiu.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/ggkkmcnob.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gdosdxqio.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gdudjcmiv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/godoavbch.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/guahlwcpa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gevqvnsim.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkchtnlbe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gtbifzaha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gfuobrmkx.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gxlcxjbhk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gmvcrhvnj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gmpzwgoyd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gtzlrwhyk.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gsuztydpp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gtrbhyjvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gdpfklqew.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gatbfcgsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gmyxfrdou.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gwwrfyizz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gbbzpewuj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gwiceaosz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gezezxvrr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gyosvmuvb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gvgxpyenq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gveboldcx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/ggsuiaabf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gdrjoyshq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gwjmzsfta.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/geeybzswq.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/grrhpjmnr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gjhvebzdg.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gyuajkxop.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gzhlvevzg.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/grmzaiqhv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gevvzvfsw.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gxishyutv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ghegkfzza.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/grdgietod.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gguhzaxfw.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gzdsaaimi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gewshrymv.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gbubsiwnt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gwrkmvvpd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/grkinkaig.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gnxhsrixj.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gjdzkzpbk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpqapnqcg.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gwiqyhiao.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gakhwdavz.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gvnawohjy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gxvpkmmxl.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gpzsrhlnr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gzxnbxrvx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gucaqfnjd.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gjrrfsnvy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcphczfyz.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gzpfeqkzn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmzfrvmyq.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/ghqetegqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/ggjxenlio.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gqktbrbbl.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gbgmuyndo.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/grjxohzcw.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gpxunctmd.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gwrevjttm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gymjtnxtb.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gueluwofs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gldonhuoy.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gbcmqyvqg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gmuipiidj.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gjzpahiwx.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gfzoxvafh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gevvofthm.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gmkeitrqq.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/ggrsgavxr.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gxqcbppjk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gxixvlqck.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gktmojcio.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gbqtchwts.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gfwmrkldb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gbdskyjxj.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gtepmbqjv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gssxlmkcw.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gzcsjnmua.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbvxoyjgb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gskfackga.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gvjgxjrly.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gakywerun.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/glrlasugu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gwusormqv.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/grnoprguf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gguwilkio.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gzvpwmmut.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gkmwizfcw.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gfaphweml.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcreklmjh.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gvwejdtkg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gygwuveqg.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gyioxvyfx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gejfajjbo.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/ganouonuq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gilwgmwxo.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gjqbukklx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggucyrksz.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gmbhsnuqn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gbzarnror.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/goukqpfsh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gocanfbcj.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gwxzuqggf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/ghuucgpkh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gmcjouxgp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gdsxyqxjb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/goedioqpx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gkupnahfn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/goxxhwteq.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gelftmxtj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/guxiuwaro.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqddmedyq.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/ggdkxqtfs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glkmvisvd.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gxgzurqth.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gembzqkys.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gydxwqixx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gasgplivz.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gcgrifxvo.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gsxblazow.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/grsldmdts.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gvvtrsbjf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/giurlkclp.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gzgwfvprh.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gxonqglql.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gdqjiefgh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gfrivpcop.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gfwhzymao.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gupzxlobn.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/goloibacw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gdquxnfpa.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gjcccolqy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gtpcfwqmg.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gcjfxtuno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gtwwkgejt.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/garzuydvr.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gyvoluswz.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gxmcymkry.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gsollkdxq.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/ggtcpbffp.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/grrsebnoc.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gofcjkvir.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gjcauytul.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gcgmbpuih.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gowglabzm.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/ggsnymrdj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwveoiyen.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gixsqvmeu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gqvifdatw.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/glbwfjytd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gexfdruli.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/gzkmqtcmz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/ghywqvmqu.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gvyotmatk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gpetagqwg.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gwxyobudy.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/grrndwxwx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gdakatjqg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gewnitfxf.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/grgzcemze.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/globlxxmk.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ggrguyhdl.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gsdimkeka.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gaqpjqhmb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gjbijwoze.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gbgczrimv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gbhalztzh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gjtmlqhas.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gnotstbtn.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gajqcuxwf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/ggrbyvney.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gcysfctvb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gnmzttfcy.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gspcimlte.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gkkabiiee.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gbbrznzvr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gbbokohex.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gpqumwnho.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gpxppmynu.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gtwgabqdt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/guiorsewj.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gwyzjthcy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gcapermeh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gydfzbsha.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gxlfwkbwr.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gzloujinw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvlynalws.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/ghhjmpfvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gtocgmyns.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/geukkzvlu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gsyfxxxlo.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gorjqmdaq.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gghkohywl.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gcvwgsvzc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gvusglsit.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gcrqnyvub.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/ghfsmxlyc.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gygtddwvg.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gpqkfnvgw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gqufmtofn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gxwekzctz.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gmboajtnd.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvadzcpoy.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gdhesqhqk.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gklpvgdft.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gvtcfgkzs.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gxtalayup.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gatlooirj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gtmueopqj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gxbvwyimr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/glyhgfbzi.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gcikoqctb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtgawkpbh.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gceygqxnm.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gepwnwogd.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gftufepkx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gqpzkxmlt.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gmnmctepg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gltkaocjl.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gcwqlhjsi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gzoxvxmof.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gdwsuceqs.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gaetotjql.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gdhrgroep.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gtruaecmr.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gkwlcbxbe.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmtbsodbc.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gqomnchyl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gxnwedoaz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gchznhnbf.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ghlzuldwh.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/ghjtvlmjq.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gxjajdlas.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gpfsnyjbu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gyzzisirg.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gbhqwjwku.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/ggczzvidb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gnelottlv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gsysgigyr.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gkzwyjkuc.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gcoutortx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gyrhvshgo.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gbkvrzeze.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/grzzdlnal.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gldytdnvt.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/grjgghrql.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gtijcipfo.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/goyucgbzi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/goldyhako.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gxdtzjlgs.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/grrgwspsq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gifhurwlg.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gwrzlliep.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gawmqudnw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gkrutqzll.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/glydgbvtb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gjhotvcmx.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gcgncajev.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gqgpcgchv.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gzladexvl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gzzyvzetl.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gbchncumo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gtbyxiwov.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/geaextnhb.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gnccvlgvt.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gbbehokat.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gecsnrbcv.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gpgxzzmmy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gpjbajpzt.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gqbpbnjqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gbymwvtwd.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/ggctsidff.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/glkpffvbi.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gpolfiuxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gfogvkdgz.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gokccbvmy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gtfjvnkqq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/ghjxvqmmf.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gxckctxak.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gazeauman.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gwlflydvr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ginxusfjd.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwfslvjcj.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gwwpraafk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gdjsoekcz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gefqtlwdj.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/ggqqtfpya.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gxfhkvzpy.sHtML


<!-- 参考信息 -->