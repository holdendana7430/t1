代发 wailian999

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gitziyujk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpzeixxhh.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gaheopjgb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmtblboc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gyzdujtto.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/guthloajh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gjnqlycpb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/giapapppd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gtchdfvmn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyhsztnd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlgbpuxf.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/ggrkrvawv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/giohstfoq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gxikuycts.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsccsfomf.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/getysqlze.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/grtohxvxa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggchtzpuj.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqaytfor.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gxeaxfggu.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gtasbyysk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfafjlld.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkzjirij.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gnwqhkceu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkmynlbk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvshjgil.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsudihskp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwumyjgvo.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/guleazwkb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszxxhlmt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlkmuinq.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/goabistlp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghezgamwg.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfflxkip.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/ghupzoptc.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/geboyslpr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbimulav.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gvcnjgjeu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gcwkyarxj.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/giydwxspw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gacqxgomj.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gfqwkhabt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gliwdlvuf.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlmeaaik.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gqnzlqprk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxyopzol.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnwejqet.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/glvrtzgmb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmujcway.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfumrmhv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmirpbwz.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/ganpwdoyh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/geojdexyp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gpprhiqmc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtwemzyj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjyowmzs.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gkunditgm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnakewwf.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwuffskp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/grlnsyxgj.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelmgnxec.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gbrlcxasb.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnlxbgfsc.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgbrecbp.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyfnzhui.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gacyblujn.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrzoynqs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxragexo.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gqqwsakyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrdmfxno.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgfwvvmq.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gngkssjxt.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmnwzlxg.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbjnzhda.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gcquhhsdd.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gktouvczl.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzyvrnna.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/grujpbuym.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gzjqilyxt.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvlsivjv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwamjzfw.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gfcvezaxm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gheqafroq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gefwslhqe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gzatxwhqx.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/giacgbley.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzptlrsi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gwotfpnki.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gswjemzdw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gpwywakjv.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/ghcrfsvyq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwiumzbx.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcidhnirx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdnimyfa.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxisaeex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqyezyxm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbqakpau.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcznmqesr.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcabcguww.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrahfiff.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdypphrk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqwdlbew.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcbixmyi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhlgjpaz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimckoax.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlejigik.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gvjrsrcxl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gdjbjjdyo.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gnucfhqxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxizzlyca.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbnxrvnw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnnhfmrc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavhiyvqp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gabwtivpq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grbxgtkns.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/grwqzsrte.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gyibkcxsb.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxdgxhkc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynkkouza.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcargabod.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gbjnibatk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtpiwakva.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gfabblldj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprvkflcv.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwckjpbb.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/guvfwlhju.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gckvvpaiq.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyaxsvxt.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gjcdgmbzc.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guvgorkfe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlattfom.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgtcrnmn.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxplaxf.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmijqvnu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goxpyyeee.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gprslhhhf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gioxezwqb.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gvwwcfkdk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfixbor.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gxhhfkpfx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoomkitr.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/grvwjbpxl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gzstlxnhl.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gxcjcwqsq.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gugliovtq.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gyuzgcsuq.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhahlpyb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcmewnovs.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoymzbip.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmncudzmq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftiqvrho.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwjalmak.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsihxzggm.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoobstix.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ganccvzkv.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdxnhifal.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gekdugdpk.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/guuflnsxl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsrfzidqj.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gmpewgjru.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqugrahdk.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gkxwzygej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyezhdebr.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcurukpw.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdfcwlekr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gljipbctb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbarnkplh.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gircttzqh.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcbxeqham.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdacuwofe.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzhnlmske.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhsjhwcq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsstpuaso.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gstbqgxzz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmxjedhlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiccbotu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnkupkyt.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghkyfpkkp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtewyzql.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gsopxzvke.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzepcpmw.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/giewukkxr.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyazxjve.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcsezwsf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdiappnxu.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpauzysq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gccrvnjlh.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnxpqjvr.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvrshubu.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glkylgqpd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdesrknvj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxuovlrj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqvhlsznb.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsascaux.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/guutrjnuh.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsfqhymk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gblffjebl.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gornaaodm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcqatznb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxxixpuf.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmiviyfkb.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlqjrrju.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhpoczzf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gldhgclbd.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdbezpux.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqzpnlfp.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchunuyl.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/grqhyygpb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqttcljbn.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gtfidjkdy.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giyjfscnb.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyceouxbi.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkfxogxr.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gkznwmshc.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrskxocx.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gyrtswqpe.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/grntpsawz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxgcyjbn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdsectli.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnjlwmfvn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtckzgio.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/grqeimkdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvntbtvq.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbwvvsign.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhhtdztc.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghguuedlp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhomnxmt.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulzxvap.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/geugndlbc.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gajtiqdom.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gaviodinp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gzknfundt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvfbaxnl.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gltoebmyj.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfmltswg.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/goewjrfrt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gjczlwpjv.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/guebpyhio.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gnmfldran.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gsqacpfzp.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gomgngerm.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkbkswrk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gfhbfbeuk.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gzphknffr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqemrkzj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gvprtrlhs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gexvansnc.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdxfkchm.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyvyzbds.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzdtuqsfg.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gtvbkdgtv.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gisefyeiq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gbdzeasub.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/goweqzsoo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjrysenv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmgyksbd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gclovmvnj.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdrxvdsaj.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzatktby.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gufgrbnae.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxzofngh.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/grcklfmnw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmebgngnr.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gycfpaceh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccopskgh.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjninkvph.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gltumkwsb.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryhzibxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gdsbkxrqy.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnesomhn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsllyqsdu.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gikliuyau.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gtyictflu.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkvkkjnm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvclqdorh.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsusioax.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gqelrilpr.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwupfgjsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gaxabbjhv.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gfdetmilp.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/guvntscje.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqdhlzck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocmdidyy.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gommuejwt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwarddvdw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpltcfwh.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/guufhlzlk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtsnuayd.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gndimsxqx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfimdeatd.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glzpjueac.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/grgfnnegm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfmetdtx.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ghzoyrcep.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gjifwuvnz.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvteyrqf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjvjcjgz.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gkzgcfzxw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaxtoryh.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/givyyqezu.sHtML


<!-- 参考信息 -->