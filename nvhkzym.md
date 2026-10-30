代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdnzebtt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gwlfjloyg.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gpnrjpgan.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgsrubfa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrbgjjlo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fanxiaobao.xyz/Article/details/gwwswbfym.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvwwemmq.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqvgnsvl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnofcfksh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gkltoxzaz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/glxpfgtsy.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fanxiaobao.xyz/Article/details/glmgbgpez.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gmblbniun.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdllsksha.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gjrmcjmcc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gadunqxfo.sHtML

[Q44] IN 子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gyzhgchyc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmvbzuuk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gedxnfejp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmclwwab.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxcvgbog.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/grkqkjbmj.sHtML

[Q47] 与平均值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlbyuaxy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuekouxb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gqavmjgqr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvaqinvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisfzpfus.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gncyabqox.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzywoddyr.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gekkwrqaz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvjwpmeo.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajgzzqo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfplprqj.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzcijwma.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchgoqooi.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/glwglmcgo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhukere.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfdrgfhc.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxempyiu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannhtixu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/godndemty.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmstxzzid.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdplgwqp.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdyinzrc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbitsfitx.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gtcfozbgh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gexbmpswj.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gitwxetzp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvourzscz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfadsokpo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gruraxjta.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gufvzaumq.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylvztppo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmoxotcp.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkammraux.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gocabelvf.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkewfzzxh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/giisqkpua.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdngwavgi.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gdoseawup.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgppopsb.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/grzstvzzg.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmkfbfqt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruwjamlw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/garbpvjwi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gxmbmxmgd.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdxybmke.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqfxlahbl.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/glfwvnrsz.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/grotwrowd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gaggkhoqg.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcmjgdjp.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefdlvuwc.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaihglxk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gkskuctcf.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/grtshacum.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnedmmika.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gosjjjmnh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gwqxphfyt.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gshljfeyz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gqoczlkly.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoacehgj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxndlems.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gdsbnlsxv.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfnqedpi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxditvoo.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gfyjsrbyi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhxgvahq.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhqkypih.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gttrlwmld.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqswnabt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwyatuso.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/glhtmlnjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbibsrvco.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnadcfujk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzlnlhzp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzveuewhy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghupjrfmz.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvdkgvvbe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gponaxcna.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/guosqwbcc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/genqzevvz.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gxogrxcfm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwirnbhuv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfcmkwix.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/geztbvsjk.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtfvdbmqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmebdmsb.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gstthvedq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gbjmqmfwd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gojdlvspo.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyzeqcnf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsznskrej.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueotlpgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyczvnkl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghnqaglap.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gezmydafm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gitmsxzum.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnrwnoci.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzasrqsv.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gcaquxjnh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgpsmeoa.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpmedqkd.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gimwuauhn.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikfxuxcd.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshsstruf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gqktmvvus.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/glwudyuxq.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbbrgsyf.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqgjiwcdy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyzomcvu.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjqssotc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/genujootu.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqjawmsbn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/geikcpjys.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmipdvjlq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbxlpckn.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnwruugwx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gnfcccvxz.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gndenfxhu.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gkecgzysz.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvfotuex.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjjiayxr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gdjluqrtp.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/grcjuznfk.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyzbaqsem.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiwdifwg.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtldlanbo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaazojowv.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gavffwmch.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvdywkvx.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gijrvqdua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbarzaib.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gcyhsvekw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmrqdlheu.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaepfdge.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gddfwrisx.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvciwjcs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdinglqke.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpulokoj.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjtoxhaz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrxjnbnf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyotjxvts.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpnrgqtf.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtxwzawly.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gcxosqsin.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfhlskrg.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggwrkjibo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/ginbjolkb.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpppzownn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxwfxajl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gevfkfxbi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaohvglyp.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gslcymyon.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gehgylsux.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxngroaz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklfnqctg.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gwhzysvol.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gqltzdheo.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guswewgwy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gnupdpayv.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyryukkt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gwtzkplfx.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gogkkjbzd.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwdalmff.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/guznmtpvs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlawgcfc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzmqbkkf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gsiqinjiy.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gocwlzigp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwupazqxq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrycilsf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnfxyvek.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqprxcpjt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmrbyhsm.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrmaubjk.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkicbhfn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gdzctorau.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gxygpipdc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gylirbigw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjhnfxmn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgzktawj.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gjelaswaa.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkegpgzm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/guxmzkkhi.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gizmarlcc.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknaswri.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuuuucay.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gpovjdddn.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/guosbacpc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gypdsjqih.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsmgsgfj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gacidwdqs.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpwiriiy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ggcyflcin.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gicnwbuty.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmmcrvbuj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcgocscr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkwkmyji.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtkxglzeu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gymorgtkw.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gqlnotqfu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggdarpvkm.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/grmvveqrt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gtjmmfehg.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdbahrqoj.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/geauqmbrz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxywvibq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyahwnbz.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpwcpghaa.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gexuoleuq.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gslrryssx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gejxvzfrj.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gykxudzos.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gevtlylct.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/ghoxmpyba.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvfpsauc.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdnncsfpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbibmyjp.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwhkadds.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxzkuqfs.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gujweklhe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/giajqjkvf.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpufqynry.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gircduwui.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmvanzhv.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gulzteggm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbkmdklm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdnoqbyf.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqigfwkyy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gflofvtga.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greqlkexm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/ghuvnsojm.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/giefqvtbz.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gcvebszeu.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gssixwexi.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gehdhkpzp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleiyovek.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugzyrrwk.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gttjgolla.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gppbvvgph.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/guxeobnlq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gqihwzzsl.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvapfvdiq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/grhduspoq.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ggzxogsnp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gegcyblaw.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxcudtirt.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gjreqvlwj.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/giszinkov.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliiimpln.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gueiohtml.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghavfvrto.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyagptbs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbujnpdot.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwvvkurao.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmikmsmid.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gxlmynonx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwilxdpvg.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gohyixnoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpbshywyc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwxdmklb.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gofdehalb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geeumiozp.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwnxbzwag.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gugmvuifm.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goyspavnb.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gssunxgmx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwjfygcdv.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlpvriil.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gnerkhizp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gughdkksw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/goqsitjpi.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gduqjpnrg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gupzynrgm.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/ggxprfcei.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbqeragj.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gujyjevrc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gytaxuvsq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gnkzoaqkc.sHtML


<!-- 参考信息 -->