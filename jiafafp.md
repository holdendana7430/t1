代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnjzvbqqp.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gvxtxhulh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gighdzxku.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gvricthzn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gswdrglbq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gdcfqdhxv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gksyusmqm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gioaxrlmf.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/ggztcyvug.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/grjtlpllp.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gigrbyrkq.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gwuqnvbul.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gyaiusepx.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gzsxwnbdl.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gyyadwcfy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gtlgazntk.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gtiudxsle.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/guwbctmiv.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gycvsjxbd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gheccoole.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gdowguwaa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gmjcpmyag.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/gomusrvba.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gczuxcfmr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/ganfaqcpx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/glzowkjay.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/ghhaddiwg.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gnjpqgmyw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gixrzqybm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/godblnwzr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gkdvdneyz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvynuqpqa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gfafgkfgv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gqnqbhrdi.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gqelktmfg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gshmfcqyj.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gytfrioxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gdxriyejq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gcwvgejhs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gqsrghxxc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gclidwxdz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ghmuvviod.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gppmtydey.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gfwvtknvl.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwmxxslso.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gfbbbqkwm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gzhfyntrg.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gzxhszmvl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gbidxessl.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gsvenzndr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqrunlpdk.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gnkaorpjk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gukxgfwps.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gvxfxaoqs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gsfukvnnh.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gqhzckamw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gqhwzgaoz.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gvcisptxj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gdmohojsw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gltlyvqsb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gzfoiuabm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gaahfpgml.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gglazewkt.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gthunqlii.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjmffzwgx.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gcwokzkwt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gotttielr.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gwhnkuvcx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/giqtundvw.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/ghniuaoii.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gksadytrz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gltaeutac.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gtobkdmxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpeqeksbr.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gdhugzbuj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gsmigalcp.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gqcxoawds.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gkoxujyjl.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gfnpicmzm.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gjagrbtbp.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gkjtvnmmk.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/ghxcjeqzg.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gycmvbmyr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/gojjcpvzg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gmcdmztlv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gcihepijv.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ggkncuuoy.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/goahahwvk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/grpovejwe.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gsgigvpqz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gqsagxhor.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gtxrymhfs.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gjyueprcd.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gqgeljxxd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gzxfpntap.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gsmwvpkpy.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ginjvbqhb.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gvjjcsbsy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gunmfagfd.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gokabwrrj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/glvkxlmdm.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gewqjadbg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ggvascdxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gxmrgpjfq.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gniufwatn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/glarmbzke.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/ghiuskqsq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/guhsanioy.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gfkpxwinq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gnuiyuchj.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/ghnmevncv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gqnynscjd.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gfhdrgfaj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gltwhhrto.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/godnbujob.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxfkqwosa.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gymkvubho.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gecgikgjq.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gggtjefyh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfknqbdhu.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gkvgqijxe.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfiqvlijc.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gangvtmyw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gwrptybhm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gsshmwuwf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gcedsnnby.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gynacqymh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gqwqfvxic.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gtygtalzl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gpjaycvjb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmwnrtwsy.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/giftsvqzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gdybpdnmw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gfnuorwes.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gxysseoda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmdwhlyrb.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/grcedgmvm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gudusqagm.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/ghxeouwlr.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gabhiegtp.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gizeyzuul.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/goqdkkwek.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gimkxkxpj.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/glnxsvels.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gljxakvcm.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gtgqodrgj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/ggsiaoipc.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gzyqcdeeh.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/giixcykvo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/giwzrnywv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gotnecylg.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gpovgmcaq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/ggtitdqto.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gbshwomuu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gqpbnoprh.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gjdvvcuxx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ganvcxayt.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gidhovefe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/ggdsbibgz.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gdapjqdmv.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gidajhikf.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gmeslnzyq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gfdgjzvfk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbhwklxdm.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gkdtordmm.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/geqngdvlt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gheaifvjg.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gudxvetqm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdohpmhtp.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gmlpnumwj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gwmwtvylq.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/ghjekrzap.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/glmvqlmhq.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gyhxdpaxu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gmikadfqi.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gskenavke.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/glmpuwbqj.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gpppheblv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gswdiybty.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gpmkifjzu.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjftqlhdr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gkitbnshr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gewqzideb.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gayjxjuwg.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gyopslvos.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/giclvsdgt.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gdohrmsjw.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gubmvfnup.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gkcsochky.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gwzjpvdxh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gqxddoiik.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gpzkodjrl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/grfdrhjsv.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gqsqszdgj.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gfxomyjzt.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gmoimvwyx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gjehbmcxb.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/getznnmjw.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grjpkdjzl.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gltwpzuda.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gyudunecb.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gbbmjqlnm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/goythbkck.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gyaqdmqqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/glzfrtltb.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gozipbmtt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gzjwacgby.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gyvojfgcw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/glejfrmgb.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gahivblgb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/glflzhrdf.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gxrpqdsau.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gfqlfpywa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/ggphbkuwe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gafccnmxk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gpmkjehuy.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gtcxfykbg.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gvbgqnbmo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gzycmsgdz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvomaipyq.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gzsgsmoci.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/ghwnptsxt.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gxmergoma.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gtucoqnzh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gjixeunfd.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gmtuhoasb.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gurjxzlam.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gzqhcbikf.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/ggpoygzgd.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gfkgrupsg.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gqyuqtspg.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gnhhrjuty.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gwhvrxhqg.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gpkcmnxgh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggpkkbqsu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gduigbhub.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gumqitkkq.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gjepciiby.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/giuypchlg.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gapnwrqgs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gitqrvxoh.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gcdkewdcx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gpigmxvec.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gmcxkbfjo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/glzqrikhs.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gdrgatugt.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gppllyzbe.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gmsscuqbd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gckkczore.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gqovzhgvj.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkoqyzfhz.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gjhhdirky.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gkfxzykku.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gmkmcnwxh.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/giomahmhn.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gmmvdsjxk.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/godschwxv.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gojehmvnr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gxmwnedar.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ggrzsjxua.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gdineznld.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gzqgciwnm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gtcrmylno.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gqozygcfp.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gntfqthrl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gpqfnhfsu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gcqytsyww.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gnnkzxkbw.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gavyvcjwz.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gfebvfrcn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gufrddggh.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gmanzdyze.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gxueofuhp.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gohhalnzx.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/goaxeainj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/giontwtrv.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/glpzwlsja.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/goibhlbir.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcyxaqbmj.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gqljhiyej.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gkioyztxe.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gkicseziu.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gezwltjrs.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gvoisclal.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gakejvzag.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gigkrcuce.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/ggylopfal.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gpnarzprt.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gqcirqxdi.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gbwlqqqdi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gopdzwwmr.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gdzrydxsc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gvslidjxv.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gmgjqfbia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gcmsqttkt.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/grbgeilzr.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gwdyvsoxt.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gnozqvpjg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gtxcqefxf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gpcungxew.sHtML


<!-- 参考信息 -->