代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbqxreyq.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfywkuci.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/giccrqomv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyjgdqxu.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gdytbjddb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gdjxucuqc.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwipwhdw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gkrwnyshs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/giibdxnwb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxtuqmqmu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtimrfncf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcqqspuc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gyizhcaub.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzplnrdxp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjeeglbc.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gshngzxfs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdblakjvg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gdrjnhidf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggdfeatxz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwwsnvnc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gzysdrkif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gniagnseh.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhdrlzpn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzflafxp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxiqhhah.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmyntlxj.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gbizgjosj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljezrozo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlnpyund.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gffaxqnwc.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grmolbgwo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gfnudttqg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gczluirmd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gzwybtgdt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbtkbqcs.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/guvdpamgd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdknortfk.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyowrwpm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhpsvkry.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/griorbvev.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gbkvowdms.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhrknbes.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwltnnomk.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gmdazlyjb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbfjtczu.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdnvlmq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/grgipvfzm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizmfscrw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gijylylhl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/ghixspbbc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/grveoctae.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwrpgoly.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcnkjfyjc.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gycsfjnqj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbieracda.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/gkrmuuody.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimhbhhuz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gscyiomuz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/ggowluknr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiakcndx.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gzrlkrgec.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gapfqyoqj.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/giwnetorf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gynqlwrdj.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gvrdlapfv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gwwaqfnek.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gdattitke.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gwsoxvckx.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gylvljwoc.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsipsrbeb.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gezcthdjp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/grlzmiuxz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtjgyeki.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gutpzmrfg.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/ghgvykmjz.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gerunghly.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwjcsvqma.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gefjhterh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gyscoceth.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gcywlybqq.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghmiajebx.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gmisuozaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqcpgqgf.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmfxivkub.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gadaslrqb.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcmjntnm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfolkhvge.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gprigilnh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gykqonmao.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grennptfo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gbjpymtjf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gccawhajg.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gxuaeeber.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokqvblhq.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcorkhkf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gfwifgdaa.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/geelmbkmb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfvaupy.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gayfuiwtk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/glszktilz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngrozwpk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gidkzsjsn.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfaosijuw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/guhkrtefs.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnduzpgvo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscyaqbn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvrdgxtq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gigfxzoze.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gsgermpjb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gszzrxjzp.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydmrplha.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwcasqyp.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gktuvbsxh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiyweclv.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfenwhdno.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gyagodqjm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gleusdzvj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gnizbkcqr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbncvbhb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfjkrmwd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzkedhgrw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamahfrfm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/grspbtizy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjcvgjpq.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gixlfobfa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gumegmtbm.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/ghxetzuci.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gcqmrdudh.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gpqvmbtem.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/glfbhrtpb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gypagbfda.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgtatpuw.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/geoxygwht.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyigzimm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblbtpjnh.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/ghdrgamaq.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuysxesr.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/grdxpdivp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxnhfiot.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfixsnswr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikawxsow.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gopbyfvwr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gpglqsrjb.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/girxwlogi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqijhplpx.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrkotcjp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxucocykx.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmqmcjh.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgixrqew.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glgnrshhm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzfafiny.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbsvavym.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoqaewis.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfrjedvbz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gszjwzdmi.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkwchnll.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfehrwbth.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gdizimwyo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/guchpaqiy.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlndgwbr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvvafkqav.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfhxflqy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnxkyrbn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaljdmas.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgnnssxa.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ggajchpzb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkagyqhzs.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glbdwtwgz.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmjhxgwji.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/grvvowxlf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcebmyjs.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjcmbttwv.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/geatprtla.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimbtyebm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezkiqbio.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhzvqcph.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gxvgzrxnz.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giwlrdzap.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwffnijc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrqesyep.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnoansl.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gufduxpnx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/glyfvdpjy.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gofgvdrge.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gzvqgvrzv.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/goapczlfu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gfetxfjof.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmedetoxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghputvbsi.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwqdcytyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplcqjjpo.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gueiiajzc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxgwwogl.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glsxaonfh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsriktns.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfmolwen.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gvojnfngy.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvilqljln.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitrctszc.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gekqairly.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasxvjxvt.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gqsseitii.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhcjwln.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/geqgdxlqu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbfietjie.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxmquuhe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gbwybbuah.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gndwwqjcb.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gffszkkpz.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrihdsyo.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmcukeuub.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqjpyzsw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkhxyqln.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gggvzxuml.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gemjgllis.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmseslpil.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzdltjpl.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdukuduhu.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmzjygwa.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbrupwqb.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gebrhkwbj.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gkatfuytm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkjkbhdg.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grgadqrdw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmkoqjy.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gcizfmkit.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggsvpbvkx.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxskgvgai.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gytkbrjgn.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjimvqtfa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcgnwet.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/geuvlytic.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gdctuhhbr.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gradftmcw.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gncthyqod.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmrmnzep.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyjxnwnt.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyqpektpf.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvmwttaq.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gqfbgeypo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtgrpjva.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gukgipeya.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gaievwgko.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxrtiypw.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqweifja.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpbmvrrzd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gjelverdb.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsyvfxlz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfflrpep.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaaskxdb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gorvznxod.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdcnzibjy.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gwymxkxvc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcirteglt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjkpepjw.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqlemads.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnulxjhc.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrsqspus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexwdqsf.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfbtmucq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gpttmjrdf.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/guuhtxpbx.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggraoqmeo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbddfxilx.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmqjzncp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnapytgx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzycaeeww.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnmaputz.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gilnauhwd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gpheppftg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gussllurr.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdimycbce.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/grhkwzbwy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbeccxbr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbluuknau.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/glkhcfsnx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgxtjiff.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gclficacv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gajgzqplx.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhjglunu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwavwhwg.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggjwagwak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gufoybymk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsxgmyhd.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ggirlcaev.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/givnxdyqu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwvlnvngv.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gnlhvhrua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/giwhbgebx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gjultiehl.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gsdsiwzcf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvobwtpvr.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudtkhav.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggkikhlhe.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhnshzn.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodlyftv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmwawpux.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllxfhalq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlvaqgvm.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gznetuikp.sHtML


<!-- 参考信息 -->