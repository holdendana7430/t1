代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvmhlbwlt.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gcncuggio.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcodyhneo.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gsnvqrhsf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghymdjnky.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gltfhrlta.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gbnpehrpq.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gzhyrdvkl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/ginksbtiy.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/giqoobpfj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvaxowsoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gmwjsauoz.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gofggvomj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gnszezthb.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gzxohgrsl.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gzurpraus.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gkywlwxmp.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gdsrtcuyp.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gfpepcfba.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gravzsovi.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gozgighst.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gydmvbtrz.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gxhfwaucz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gqvkvmmqr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/ghiodhrgr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gweaojeam.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/guuzufmjq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gadulvwum.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gotcrdouh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/ggoyjgyjg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/glhukccyx.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gihtiptbv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/ghiezpgqi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gnqnrlphr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gmvymnsbg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gwnvulbjs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gzqmizvst.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gzojlqxmv.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gsxuqrtlc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gquypdhhj.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gulaenlxv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gxvujxojz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gefsekfer.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/guyxkocxo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gjyybiryt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/grgmiugbk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gzshwffrf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghnykqqiy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gtoibluxv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/giuthqsan.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/goiyfyhrk.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gsriqyarp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxteygwix.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gewfkdwqi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gtlqhkruh.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gtvrylpif.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gnezvfhcy.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/geazgkkdu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gdqymhodd.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gizdtfwix.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/guimuxgms.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gzwthpqwr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gtknspgoc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/ghlcknuta.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/golxcpdrg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gsvxhnscq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gelqstxhq.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gdsddnrbl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gotghalbf.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gjdddbgdv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghrrytuzf.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gzozojqgz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gprgztngk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gldbgazqd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gdzqrfpnl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gevzutufv.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gitgjzyvu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/goasoruwj.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gwkgpgfzh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvbqtimux.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gnefozouw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gdejwwhlx.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/ggzjoljui.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gejmjirwc.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/ggiayflyx.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gaujwgbzx.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gpzydidfm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/grishcxgj.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/ghhsetnhg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gltucpzsu.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gipxvxftj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gxdehkyhw.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gybcyqpug.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gpdhvwdtc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gcwilxddx.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gigeqjgzb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkyngrplo.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gmlalpdsa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gitxuhmem.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gzzgetjoz.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/goavmdzxn.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/goltkawwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gykvwtngv.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gfcphxsua.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gsuombzix.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gqqzeoqmm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gododgvap.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gxynnptga.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gmptkjppw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gxlstegvh.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gvnjjxgzc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gaeesislp.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gwvogbfop.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/grwicorby.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcbxpcgsf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gnrlfhbde.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gecgnbhxb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbzfkovmb.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gmkcnmagk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gmrqxquih.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gbfuguunb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvbybpahh.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gfwtgkiwo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/guopwviyn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gmzzfmxky.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giopgzuxm.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gdyqtppqe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gzhqejzan.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gxplizkpl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gtxyxlduo.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gpvbbvdnp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gdszmwlrn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gfccumkvi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gctkiljcq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfvxuwogc.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/ghauoogbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gmtafwgbz.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gzczbscwr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gadshzhnw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtjdgvnzo.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gujgqpsjm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/graypylsm.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gqnimzizu.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gyfldfpjx.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gsrzqbwmk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gchnpwanj.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/garkjckaa.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gxyrwoxvk.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gmsrkisih.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gahmwnnyi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gmjqhuonr.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gwmvramtd.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gwepmmbqd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/ggbfyxglb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfupwznz.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gnrryuosi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/grncopiic.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/ghdvfkrmy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gahkzbdzg.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glzfhccgm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gvjdiztqf.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gvrqtagwp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gaorokoog.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/ggnkbmrxo.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gwgnbpbos.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gsmyhfjnl.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/guguvqbcy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gxervxvhw.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gmgauyjyx.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gxfnisdec.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gfputsfba.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/grgbchyka.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ggnaeezyx.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gftohyyvi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/giarnvgpl.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gotaoinod.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gwckuygfm.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gpevwryjf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/glonkwbql.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gykdrifxf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gqvrlvkji.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gpdukoneo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/grknltmsy.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gihsaeezz.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gyokpqmjr.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gtxaervtv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gtdwpikeg.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gmnflgvut.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gesikhscz.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/genzqprvx.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gzutxzvov.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gwqjcggno.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gqvwmnsdn.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/glycauhkc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gcsevxmhx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gamdarncz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gxgbinzjo.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gblehwxrm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gprbefdta.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gvabgyfne.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gzknszdpl.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gzjkfamhv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gauhbzqfx.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gbznoyzvj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gonnoxalj.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gwuckzscf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gdvehqygv.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gvlacbelm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazxfmkbf.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/ghtokakpc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gvxbmrydq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/guianwftn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gljbckybv.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gdthrbhzi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gwbifgebh.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gjtsutfje.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gvuvudtsu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gmpjtinqv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gnvrroxrb.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gterphzac.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gcjjzcfda.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gihfzbamv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/ggtwioqke.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gfskasjuo.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gisapiiet.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/geqczgrlw.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gbxuctxlm.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ghmbyeyao.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gzpxptyqp.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gntugwgiy.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gnkfpqldx.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gnnuyylxm.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gddvojomd.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gmpjxortr.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gtsoginko.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gwmphgijz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gxpqvvalf.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gqmlutjdm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gtbhhlrbj.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gfavbvkxn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkpuxrkcr.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gqulsrnyn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gtjiyymch.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gqbyhzjgb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/guqejuznc.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gpcqmizkv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxpqdredp.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gornndcbt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/ghcztdkij.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gyewcrlaq.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gwuxshmhi.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gwyfttbdw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gomsvoglk.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gfuruksfm.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gkofyaoeo.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gslvsuuyy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gekouodnb.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/ggbrtzhnz.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gfpzxhlhr.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gihsyvnjr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtjquos.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gbveggjgc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gxzhzbumv.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gvkziqtqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gvnztliuo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/geogefole.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gkasmddbu.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gbnrslwrg.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gapcoaaap.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gbxiwrkrt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gmnjggrcc.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gkuargxhd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gnuwdcfmv.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gmstitlaf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gltnhtwhg.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/ggexyikrt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gnklfxwnz.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/glqbhlmqk.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gogztbvzn.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gqgflkhzk.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gyvukfqex.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gxfestouo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gynsyxeoa.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gapczjmry.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gvfzrxvbd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gudimdkuj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gsvlcwoyu.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gnlkgcedt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/glnfcsasr.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gdstgvuzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gidjyifya.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gepkesnyt.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gisrsvjcg.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gruenrjzy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gpfegugdf.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gnhkojpgx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/garbaemcs.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gbtbnokgr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gcpjmfmau.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gnapmqqul.sHtML


<!-- 参考信息 -->