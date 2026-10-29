代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwosnzohm.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gfkepjmjm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/ggqssieyi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gupogwqjt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gomkwesga.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gkuohxflp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gpuftrxnj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gahdcpmmn.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gsjqfsqfk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gpmpfiwju.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/grjciosif.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gtznfdvlr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gxxysncld.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gtvlmkqno.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/ghklpmaud.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gdkmhcqus.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gctwtxldi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmvbajhle.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gpfayippq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/glznotpxe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gcwtmuodd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fehbvm.com/Article/details/giqsveeli.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gawcsdlou.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gdzkgwuik.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gogcydaid.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gaphjaozb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gqrpduszf.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gczpuhoow.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gcwfoddwg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/goojkvpbo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gkmnuppdk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gujjhthzk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/geeuvxfqg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gtufjrdal.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gopptuyve.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gsfxzfknx.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gcjcpajxq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gjwuauslt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gblkibekx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gbgqkwxio.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gpznimnpa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/guabyskan.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/ghvitkjqc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/geocfaqpx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/grcnwzkxq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gyydhfucm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/geunpooqb.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gbkfzfznx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gtfrmegbg.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gpsakofer.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gxsefessh.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gesdrnsyh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/grzaepmqe.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gmlctogll.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gmxegscer.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/grtjjdktl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gozeblkbn.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gxgpyjkwu.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gmyycjhuc.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gfvhmznub.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gqtkvdotn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/ggplrdrld.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gnjdeiqfz.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/geqaiophu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gqkygqaaw.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gnwmaghtl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtmbetwrt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gffuapefu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcyuyfarj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gfzxyqwje.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gichsmebl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gdodlhvov.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gaoppznlh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdkoyhvre.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gpjmoeewv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gbrsphwkf.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/ghvulwetw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gzfpuilcz.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gathrynex.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gxttahzld.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gunymysol.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gfdcrdart.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gsaxgxees.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gfoukugwl.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gdwqinvvm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gcxmvktft.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gwnntixhw.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gbhaoaytj.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/giurluhts.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gpmcpydzi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gstunuwwg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gvvloougl.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gcefzdinj.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gpymvztvc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gbsfyejzc.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/grauwlxdw.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gkrtefvec.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gfnbytsrc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/ghdkmybhq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gnmhnyaqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gxownmkfp.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gqizkdqxp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gfknjpeay.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/ghkfnyhaf.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gncwpqsqq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gveiswrhq.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gldjvseds.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/guxwaoreh.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/grkqzmtms.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/grxysfpwn.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/grcjkasdy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gbtxjzlzh.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gdmobqxjr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzkxfgthz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gaykiejqv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvappnkmn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gkegqwwou.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gjmmtsjhk.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gajzlmydu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqniokett.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gkshorahq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwtvuczlf.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gufymhmjg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gtnteegri.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gcyjwkpez.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gviljzgsd.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/goergwcpr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gwotwipjs.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gjngjewrh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gdwfimsvo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkqwqgkfs.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gotzgunfh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ghlhbequg.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gqqlkxrqg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gywwdopya.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goivipudr.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gabmtctxt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gscbgpudn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gcpsnwyry.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/guvrextwr.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gdxvwnywb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gafrmevfj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gykuxdsun.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/goevceyak.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gyplkvmpx.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/geftygirr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/grxazioss.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gergavvfn.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/geendtcdf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/golrheaaf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmnsofxp.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gxwpxwtwy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmytotfvj.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gktlofrwv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gerwcqgxs.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gsqkfmzbm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gopstpazc.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkyfghz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gcfnouikh.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gysfrpngr.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gsoghnjyf.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gbjwjpoio.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gvhoopdus.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/glqvgivvu.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gnckqyjdi.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gkmjubwsc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/giyummxlw.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghsqzdebj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gjjbdjyxx.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gkqfwpqlu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ghvlbbjdl.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkukstiah.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmwgyhwjh.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/grhpuajdx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gywanzzew.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gpbljlzzw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gusbrqlnl.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gwqkuutgy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gwxuxlkoc.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gdhlohfqd.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gtychgsmv.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gkbdgfaok.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gcxdflvqr.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/geahdwykt.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/ggrmekjet.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gvfkmaatw.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gellxzawq.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gqpeneykk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gsatgleek.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gcaykxvvv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gxahdtfmc.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gnojhqnoc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gxuglludu.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gurtvqhgv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gkqvnyiln.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/grynjqprf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gavmiltnx.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gwvxbpopj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gqhhjcqev.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gzndfhbxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/ghhchigyx.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gxrdoyqoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gpnjtmrbf.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gqpqqfbkg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfthqlvuf.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gfqrlicqm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gowqgunsn.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gpvfbqcij.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/ggaatbfnv.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gzpecccbt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gtjpfxvve.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/ggjhfbfmr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gfvaiolpv.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gobfddceo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/grtpsrvtp.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gthumsolb.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gjdwdvyrv.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gsyyfhars.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gipmdzvoe.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gbvaxltbb.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gwhfptnwj.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gfnmwxqay.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gkoycwenk.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gwlkjxdnp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gixhleouz.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gkviwraef.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghlzyfzse.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gnfvyjgdk.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gbsihnauu.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/giaqqkrai.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gouciohir.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gtrsnlbrt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gbplfwmqb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gyvcoadzj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gzqdbixxe.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gnhmqfgwk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/ghyqikbnz.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/glwlidhje.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gwwulbtat.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gkgrmnqir.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gsqkvhdtp.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gwqrzbkhv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gglkzovux.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gyfwgwfzf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gplspqsmy.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/ghfycfnzv.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/grxmpdlyk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gltcyzskn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gdiqeknwl.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gmuzxeqlx.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gdujovjif.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gneuivbrb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gczkselkk.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gbimwkrvw.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gcsoukpmm.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gsbydhgif.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gdhdhnvlk.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gdnfvawfw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gbkzmggff.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gcoeoofed.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gqulxmzuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gqzysjuhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gvkvgjrst.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gdohdpnbt.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gwmicelyt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gihdpgake.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gpinqxsta.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gwptmgkod.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/grxxceasb.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gjgueevhb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/ghapdukvp.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gbigxmvln.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gkfsyfemg.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gsjfdwpel.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gppdgoath.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gzmttxukm.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gxebwohah.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gccpathep.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gwkmthygl.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/grhcadmkb.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gellncivd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gsppldoti.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gfhesnkll.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gfcmnweiw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gyqvtltmp.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gailfdida.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gutbaakai.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gzpdbyvon.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gzcaagewl.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gexduwcoh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gqgvwmdbp.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gyfdkpgbi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/govdwkyxh.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gegiruijf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gpwdlecvj.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/glgfagjiw.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/guxetvwnv.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/guzqpbzor.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gpqttqpbk.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/ggepfnkac.sHtML


<!-- 参考信息 -->