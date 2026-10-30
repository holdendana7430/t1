代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gjboshfzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gnbapzxul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlylloen.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojvmwnai.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/ghykfaqrs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fanxiaobao.xyz/Article/details/glgybfvbs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgdpeapg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjczpszqf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fanxiaobao.xyz/Article/details/gevhxclys.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwctipxg.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/guzclaxmy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gtlxcapit.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfzszxaj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gqpkvabmt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gjpebyrpp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvyvwcae.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gndraebrg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzrofxfa.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggisuube.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvlrrazj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvvafvmt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaapvtqip.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gmnaciczk.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gcwrlzmwn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gczyreuwf.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfelnkdfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gasexhjnn.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjladhxz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gphdzqeue.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gcqxbccpa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsyajdiy.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gwqfyskvv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gohcowgeu.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmykvaaj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaeugzny.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjhdgoem.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpohcbsr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gxjygdtlu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gyyctrqac.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmxbstaw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goqkjrpkc.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gpypxhnua.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzhguqdx.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwqpbjms.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gwvuyopbc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsdgkdlh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gniqbymhq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gakappcwn.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhotztxh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpteumnmq.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooiplwhe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfiqiltw.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdqmpqbd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqitvxhf.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvemteqmi.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaebdkiju.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcosihomh.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/goauavvjp.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwtmcsgp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqyiiqtg.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/ggiirmcfz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gbxtpoueg.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/glbehsvpa.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guszkzsen.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnmtxwxp.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gnhtsbnzd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyspedzj.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/givpacknh.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghviqphul.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhsgvnvc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvplvgto.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gmvkmxtni.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpwastuh.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjszokga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdyrhujf.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnestjbh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gtumhqhpz.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxpijkcsd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzeppblf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gtcrbqedk.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgxtvbnw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqtyvtjh.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzaaxdmj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimadmckj.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/ghbjvapfi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gaukekncg.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqdwqkfp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/garbobztw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizmlfcws.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzeqepeyj.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gzytbabnn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvqahnl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/giwgankrq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtsmytii.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfllcjin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfkvheie.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzkhszoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbmoemrxz.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gyoallnha.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/giwdsqedu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/govvagtfi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnqgzaun.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmszgdimu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwulnnrol.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gynwtueko.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwexghyod.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfhmogqzg.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gycwfoidy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gigxgytqf.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpijdxlwo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhpgzkix.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadocpxcm.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgyeaver.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjjqqzfr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqgeaaqr.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/ggocaaikn.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gemjaqvtq.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gqmdmjsud.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gepczgtbw.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkyjzzns.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/grwitlqir.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowoaihnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzywmrmot.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/genmucugv.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpqmrujyr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvttxbhu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/garjotbol.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghacqnnzm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqerycihy.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gotgebvbu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpbxtppp.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqxuhrrfb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gcknzyxeq.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmlgicmm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gpbubftuk.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/glbqojukk.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsqygdvh.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/giijtngdf.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gsemctjrp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gryrljqcx.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxhxnlpu.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyvklxxa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gaepqjxaz.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyczabnj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvuyaqmq.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gczurgimk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeotkqln.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfbbjcnq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/goxuydzoh.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoupaeal.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrkxkxum.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxicjikkz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpckscggt.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkgcgqro.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjsssalcr.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grjitgesh.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpwxvesb.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/ggqwbleme.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnnuifwdp.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ggaquxqlt.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guupazfcb.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gncbnulgr.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gimlkpqgi.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grnkqykam.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpqyjzoz.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpmuckhg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaaxqgul.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmieynjt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyrspets.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gujusaxkw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurbvrywq.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfuwotbm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/glsvxqdkg.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/grmcymcik.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/girmyxspq.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmurekupu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqnrqwnph.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqahgkrus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqenzbvg.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyftciye.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/grtxutvpu.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gtkyyfkoe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gikvrohdx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gxzftkurn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gifyvdvmo.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsbtgqgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gznjhutoo.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gzkskbboj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumkaxot.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcunenti.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gxexyzkrc.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggyccokbv.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggiolcsxx.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/godhfoblf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/giseqivjh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhpsdllx.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/giislfzta.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gulqjxjmt.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gqqeidnzt.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gzsuicxvn.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gjisrkbrh.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gexgbebkq.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxoszvuua.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvpqfgutv.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncjhyrfo.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxyddrwor.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gqwauxgex.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmunoszky.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gxyeidhxq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphtmign.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gctsljaaa.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gipnroape.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghhpesjgu.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gxgrjnhdr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gumqbfnzw.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbnudguq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gookgtxvh.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/glldoabon.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goimkshhj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/ghcbbowtp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/glccttisb.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gzjfbwmrr.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guljpxsbo.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gebesqajj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcxaprpt.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaqkeuync.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gncpeazfi.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gdjohjzrz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoevsaax.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ggtzzrbrc.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gliikowkn.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchgqrxix.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gzmohtzuw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grcpdmfks.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrhrdsqd.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiouqptm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gedglyicf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgdalykf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ghooqdbzb.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpgllqit.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsepvlei.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goduzprix.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gyepnofou.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbrlfpev.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gqzxfzcrv.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gispyxxmv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/guphmcyyt.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwvgnvpzc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gxkboekcx.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/grommomzh.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikmtvoxv.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjraxorey.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcstuuyz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtigkhinc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gipohksod.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/godikmkcv.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gohiqqyml.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/giygmtekj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/glfowsgif.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsgfpxqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnsileww.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gupkxqwwy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsmsrtpyu.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghyybytse.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gdcydglhe.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/griceaanx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcvuoyobe.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfzhknkmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/grkjojlfd.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glxafkjpx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grwhohgqt.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/guzmmirhn.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqqyrozk.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxszgyar.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/geshedcvp.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbqrxxqp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gseyoyvxl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gkokkxirz.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gktfqcbvc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvisqhuzi.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuztuyim.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsgibfxt.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gccotjgoh.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrcysni.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnhssay.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gywtlwxka.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzchazauo.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidfwedt.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gavqvyqtd.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkbufgeo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrgnejcx.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggzgfosya.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gadznmrue.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gbftthtvl.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/glgldostx.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gasmsdkqn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqlntauz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagmqtmok.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gswfmutyp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gghnfrwpq.sHtML


<!-- 参考信息 -->