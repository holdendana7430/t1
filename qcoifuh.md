代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvdbegxtr.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gsqvimkti.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/grvjfdccj.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/guxptkwvu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkxlzlzg.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gvnaabjgo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gbopqgmpy.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gkgglccsc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gidrskbbx.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gpuyxzkci.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gstoxnjbz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gkgljslgf.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/ghuvddcxb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/ghnmcsenp.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/guqzjljis.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/ghqhhulni.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gfzkvbinb.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gyyikbmlg.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gzbvkubxf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gkqlwllun.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gmwjahitt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/glcthxnrq.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gwpgnsyzw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gazeaviqr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gfwxdlpqe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxxoubgyx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gxckxycro.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gmankmwgz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gxiadgdsu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gagadxibx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gscphycnd.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gqztpirgv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gloddesnh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gpyyinkwp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gqnexmgdb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gprexewha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gjuzhaqki.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/guhkqfziw.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gxyiiqrrk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gostlemba.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gkvrfvwld.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gykehzfii.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gsuxrzzam.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gvqneqdbl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/glhhehhab.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gotnbmyqm.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gxorsmxjs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gsmgfonug.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gdzroczsg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gewnvvkez.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gbfeottbm.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gjvjbuvxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gawyyozvj.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/guvbtfkyw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gztrmmlef.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gkskpvevj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnjixnuvn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/giazmnqnh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gkxmhnpvv.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gzjlmhjkc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gjfymdiwm.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gbebqeufa.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gbfivkwim.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gfganojof.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gvlsbnfsy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gkchjgehr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gksxjrxdz.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gvtcflcsg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/glakvwblg.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gtqhrzcur.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcfcabrmh.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/ghqezzvdy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gwetetnnh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/geetzpawp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrnqmpu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkrwfgugp.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gddyidpzb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpfzdisyu.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gxvhafodc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gxnfnfdrw.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/ggellaprj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gnqxiyirf.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gqmiuwpxb.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gkqjpcwun.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gboekgalk.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gapijapkp.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gaaphfzdo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/giayotlei.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/ghrohxblf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gwrclbhvi.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gyzbelrle.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gjkxasgnb.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gzoevuzxx.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gwbmwynwl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gaamxhmzb.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gkyxjxxax.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ggzyyiblp.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gzamlhdhe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gmsyyjzfu.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gjrogekxf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gawkysnog.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/giyjaouik.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gwbrvifef.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gjfqsjpvd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gkgxwdawr.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdsssxjvo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdlxfrhvy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/ghvmawddd.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gtueriwfl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gtcwftpcq.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gkrmbuige.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/goqopejxh.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gpqtprfuq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gfdxfwlnk.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gyabunlkr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gisqouxil.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gmrgjmjvr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwzaetzrp.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gsqeacvgq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grzbirogj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/guydqwjzv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsbmzpbgf.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqhwcyuwp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grvpsypyh.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gufegcdvi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guzbkymvy.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gcoofskna.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkkpnaftg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gnbqdghtb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gzqzukocp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gchannzqo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gadtwyxwq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gkmzbscyn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gwabucomg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjolrepir.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gkntfblew.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gwqufhlhu.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gxquhajsc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gduhzqjqk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gofsxqoke.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gizbuddtk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gayqwkvol.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/ggfqlgifa.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gtcyorhur.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/ghkernely.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/ghmsxuwom.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gtwcatvjq.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/geavogojj.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gpyqwwkbl.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gplwygfgb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/grtdrqvxz.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gjqkalyra.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/guflibocw.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gxoubkwju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/grixazdvj.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gcwqfcszr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/geblmxgjd.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gqjobklvx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ggpabixlq.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gcvmwjmov.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gevxidfle.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkwuzaaju.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gaqeujhuo.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gxdvlxbfs.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gkqmdckmo.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbwgjrpem.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gqnyyyccf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gccvogpcp.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gnvcmbums.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gvtdyxbcs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gwbgfaqsw.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gofqtvvgd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gdbeodlup.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/govehoyqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ggkoxdcfe.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gaeqltbco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gevvzpmva.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gektwnflk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gpegrjyfj.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gzmlmpdeo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gbhbimpwy.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gdwjifldq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gykryihbe.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gxboazkvm.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gqbbdlmgi.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gfjqwlhib.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gusicrjtu.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gnflnjiue.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gouweywzy.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gwkfjprlc.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gqlinmioh.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gnpsasgtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/gyrazciwt.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gabmmlsba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gtkrpfgnq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/guquuhpbq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gghflxjpa.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gmalcluef.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/ghneaigmj.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gxedpfqdx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gkvfgapgh.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/guifhxbkx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gzmxeovig.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gkfmojgbp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gcspgvjts.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/grxkonalt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gbjnfocmy.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gjafsqirh.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gooydmuki.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/godjcaypp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/glzbeczrz.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gojpnhnpk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gdgzwumkj.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gfobwmpwd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gxzmgwprc.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gxefjoonw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gtiubrqgp.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gwzstweeg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gkarnloym.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gdwurvisb.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/geddjxdrp.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/grybbpoye.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gpqpdwebi.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gbozemace.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gomttisyg.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/guvqlgqvk.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gbmmvwyef.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/glhmniegb.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gscgsexoj.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gmvcqnywe.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjebyiwmv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gyvqwhdoj.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gzvgejvzb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gqmkodrxf.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/ghhvvlzlg.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gioucudps.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/ggmwawdqm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gqvrtrjov.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gtuigqpaz.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gsfdvpihi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/goppfmhau.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/giefmnfvx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcvwkhiqy.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gepnnstfa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdqgovmym.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gzkownrwl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grgmyiuuu.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gsrqpguao.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gwcwerytf.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gfacdadzc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/guxkhiant.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gigunvdkh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gdksylcnr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gxcqnerie.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gkhomzzhh.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gihcybibm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/grssofmuv.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gziufsser.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gsxvlsbwg.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gwlmfwjhn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gcsidxrmn.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gucgozkag.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gvmomvyxl.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gvggfirlj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gvizenwlp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gctqbhmar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gjgyufkbk.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gbtfkgref.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gnkmcaclh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/grvhdzxdv.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/goxfojwsi.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gegzhhxol.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gbhscsuti.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gfvxmombj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gnpyqpvid.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gjjzsytcm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gnoecdqaw.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gbpdewsso.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gjpsikxbr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/ggonbgfgx.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/ggurudhiz.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gwhjhnwac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gzusfvbun.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gsrkyuxch.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gcqtoncwo.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gebemxqfq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/geuewplol.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ggrgpjyqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/grczwsewl.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gpcjkzsdc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqexkxmdq.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gbdwolfyb.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gqzdctogt.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gzbvywkwq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gvtdkeesp.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gktnaeiqb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gicaakeyg.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/guwgszizd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gkclistis.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gnemmismt.sHtML


<!-- 参考信息 -->