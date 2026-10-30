代发 wailian999

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gfokcjrua.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gfjikuwne.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gjjgsuagh.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gqrmhoixj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gmvsvyfok.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gpnvtltio.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gnvrvpjjd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gzruujuoq.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gdxahxtqh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ggpdfnsov.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/grhtbkmej.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gslcnzgcq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gyybfvroo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/giawgqwwl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gcjgysopp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gntcuaydi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/goeoqxpcn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gnpnsqagp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gsysdlaeq.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/geculinsu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gesrggypo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gcwcczssf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gopzswkbq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gcatgbabr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gtjalifww.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gfqbbalzp.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/ghsbgxcoh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/ghtmqbjmq.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gehkoqdmj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gldzmbqiq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcbaqqavq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gefhwzmgy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gfivpeefz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/guknloxww.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gzurhftyk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gvtbqqwox.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gtfuljxim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gzglcxefq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/ggvtibryo.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gdgjdeyci.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gnltsngqa.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gaudbfems.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gxacokdeh.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gqlrvmhfm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gkafzkjaj.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gmhewxknr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/glhrsltnq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/ggeckczwc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gkwnuxkvx.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gfjqbbisi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gpblrrjap.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/glagejmvw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gexvmdnha.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gziphswqg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gfeneezwz.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gvztnlknz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpebqpcda.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gtayydnts.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvijdrmpz.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gdyvgfwfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpybqfgah.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gnmgtsrew.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/ghqexiksq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdnfeehzr.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/ggtlfruyr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grdzdqfws.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gmoevnedb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwyounjro.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gjcnxpcwy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gfeozybfc.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gjocmlvpl.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gnqivrieo.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gaczyfoso.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gnblxuiau.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gygfvklco.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gzucevrby.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/glxqdizva.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gshmmyeah.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gejvvhmxv.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gtqpstotm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gnjlfuubr.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gvirsvkai.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gotgfporq.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gxmdpcjxo.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gyrtkochu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gzunccezf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gcwdhqeba.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gxkxvkhhl.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbpcwnfnv.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gaonqqycc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gaufwrzig.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gzoxrcgsn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gngkndhih.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gqxysjsta.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/govkdryqw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gbjukmadt.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gnwutxokq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/ggyoruatf.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/ginvltwac.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gcriyvgda.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/guyjlmneb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gxjxrwgkw.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gpzfjyaon.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gmqujypxe.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gwvbeaoum.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/grgwlrqrv.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/guxvgeyjn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghhnejzif.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gqpkmxjns.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbrtiedzf.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gjuaahrbh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/godezdgnc.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/guoasvpjp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggrbvycpx.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gojlbgbjn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gymowyepa.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gomosjhja.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/glupbhnen.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gclxojsyy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/giqmcrmdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gwrbqzgip.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/ghyhkhjfb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/geaqiuwhn.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gsavhftlz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gvwkcebnj.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gyfvajlyd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gsbchsswf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glztlpthg.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gecmjmzzw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guvlmduaj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gxbhutwtx.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gvyqfwfwm.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/grzxoklwe.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gogjnfxie.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gzhomhxbe.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gyushiapo.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gyueojtuy.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gtskqpwnk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gwrlefkml.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gbssngjts.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gcikrzphb.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gwkzkcbkc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gewgbtkxk.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gamgqbgft.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gejoekxfk.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gzxrizvye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gqdtaxlrf.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gyywouiku.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/giwekevhe.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gxvbyppqq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gcasikvcx.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gzublycvz.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gvrequjwd.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmkcpwnuz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gkwrbjkqm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gsukskfhy.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/grvhttyos.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/goovltsbh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/ghdpklapk.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gaktbcktg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ggphfmhbt.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/ggbyyxyay.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsylgnt.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gnslvnzmf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/giitjakbr.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/ggwmlmini.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/grhdxaind.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gyakzwjgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/ggwdxhnis.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gpmiodsyw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghxtaknkm.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gcxfwdymx.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/ghanwpyxm.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gnmzvnyne.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gxqyzwscq.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gypjgecci.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gxvgvyqta.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/geetcvhvo.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gyvdfkhkm.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/giyxoqejh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gttkbgajr.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gsxweyvng.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ghjqexlld.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gwvgguvdq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gioetchkz.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gqymbavah.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gfzirehpr.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gmrvvmnff.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/ggamqxucy.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gdncrelde.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/grpkverkn.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gitnhimiv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gbfrfekkx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdioysecj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gehhqwqha.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/goqpkmcev.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gfheluzfv.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/glfvdbqdy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gcwyllfdk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gopzumvhp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gjvwrteag.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gedabjdel.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gzyjqmzer.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gxaacyrtj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gsqwgwmdf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gucjcydsc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/guuxrwedq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmhdhpd.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/guojpisif.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gmhutjnve.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/ggcjchgip.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/goafdhkox.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gmwubtgtb.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gzokmbttf.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gpnqqfaus.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gstsqaxil.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/griecpcqt.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gqlucvobh.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gochhkzik.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gwfzvernr.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gpjrwglkx.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gcklkjfcs.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gucvmnssv.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/ghpugzwsd.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gcystvmnm.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/ggiyiosif.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gbyupdizj.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gluazlhwr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdnxzlnwn.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/grfbgfubk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gsayrjuaj.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gfvzdanjs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gdttrbwpq.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gvfbitexv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gdsvlhdrx.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/grcarauin.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/ggvvhxkhu.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gvlanmhdy.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/ghlsppcmq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gdhhahnth.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gvdlqvlwx.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gjmkcpklr.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gyyhzxlyo.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gqoahbjxe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gqhgiuwqp.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/geriygzva.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gnbqajptm.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gqflanswc.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gqzyhedwb.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gxayvqhze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/geepyceoq.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/giaswqevh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gcizrdtro.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gnrdzcxbv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gsqntfars.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gunklisrc.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gmokyqsyb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gadwhowhm.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gaouupriu.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gofumtyoh.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gvophbqqy.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gdoouoanx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gbqdohvxm.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gglepkqqd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gebkwkyiu.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gcqicgawm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gutzkuivf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gulfkttwd.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gzonziray.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzkynma.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gpetsspim.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/ggturmiay.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/glmmjwfnq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gmspuofkn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gpgqnzvfv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gakafdyhb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gdqcoohec.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/guacbleak.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gmyskfevr.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/geejfakbc.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gnltpofng.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gyvkwhwxf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gxwtqnlmq.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gorsrbcto.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gkjwqwkgo.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/glppmyklk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmmjdqooz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gypzubula.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gqpedeass.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gmwfgbrhx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gavcatdje.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gjqjhmfqw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gothezqkt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gcasmofun.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/guzxextms.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxsajgrue.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gtlxfkftu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glkaasblx.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gupudhfvv.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gibmflfce.sHtML


<!-- 参考信息 -->