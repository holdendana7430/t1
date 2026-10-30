代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzegnzqvn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjeseazx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gcuenytzi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwzoqxueu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gbdqwkxde.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtofcwtit.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gjubvjjhu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gpynaqfcr.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxvzjrye.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkutndhj.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhavndle.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjjcwofu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glwmuouoj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gudnzzcpv.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigtogex.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkzltifg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyawtwbg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobpckhvs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwnnxkak.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/ggsknzydt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gymauscxd.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gcayoregg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gawdhoseg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/geixwchaw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gutmzjcww.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwhcwcl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfphgghc.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gxzmisqvb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwnmtftl.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gpwelxinh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwipiorap.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfztzgfyl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzfgkwoq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gxtumpubo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqdefrjz.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhvrvcwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gswayiiso.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpcsiwz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gvdueysfy.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgmdkelb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfkdfqjv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlibmzvo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwljqdgjo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gaavbznei.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/gxnmzrwrq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gobldswap.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gamoejdjj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gumtcodrc.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gdustoghy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzftihpz.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gyugtogre.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gphjvuqsr.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfidpxjf.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gllhdjgnx.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtfbnhrde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gwrzuuslf.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gohmnxhgz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsbbwyne.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gcaswykgq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geolqgjda.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/garnwbiqk.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gznwsfsov.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/glqijupls.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/givslxgag.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpaflqnq.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gutwswrhu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpomsqto.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gubrcedjz.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gdibtfbra.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/getggvxzx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqayadmc.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxuxrtxkk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gjecrpzwc.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gpzskyxql.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxhvqyzv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/geuahwxgz.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdzijdee.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gfjsxorym.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/giafuazpt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapynrnrf.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gkyhvabwm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gjvzttnug.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gippsqjpy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gdkfxervx.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxytdhtg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsbdefhz.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glczadrsa.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxylfyfal.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwldbgxwu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaiegpcm.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnsumrnmr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glcmrajct.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtcxfzlg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gknmjmpyd.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxplyaf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/ggebcquck.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbbpijjq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gafcloqsw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktwqhcdh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqukpmsf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gtpkjlsfj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govwuqmjp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gputkpseu.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guytuorux.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/grqpziupg.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gglsfmcgo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzplarlqx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goielppjr.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gpanyptqn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbkackvlx.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/glietloun.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gdkosjcny.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdrvjbys.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfagxcayo.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcsihqjwq.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gskefsobu.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjrufsan.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqajixwo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gouivmxls.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gglxdkjwb.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gphxyipkc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gspmrxjbt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmysqsshw.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glmurawog.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/geklyfwrq.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gicqcnwgc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqmaoxfxg.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxrfyyid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/grindkhsf.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrrdwchw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gboakyzwt.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gquophcis.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gfwgdwdqj.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqxzqatx.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnharwxyd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcifpweex.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gqvjeblua.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glfeidxaz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfgywnrxg.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gklhzgxxo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpxvonxzl.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/guscixsll.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gaekmoatr.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwhkbrip.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzctcbrr.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grcudskjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gowfzfkut.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/guxarkalc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gouwfkjiv.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/glkqjwygv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzfewytoj.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcebxlemu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginuzpjtw.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/giufzjmmr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsesnjvez.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcgaldhji.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzskjtrf.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/grzqvzwfh.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxqdbaxpl.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuddpwxm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/glptcpxmg.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqptuhcv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjujaqlr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gfckwfsfw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvappofjx.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwzaxmxjr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gumgahwbc.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gcydhiqfd.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzblancgo.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuklbivm.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/geeraijcv.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpilxabck.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghzwsxjci.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goafuuwtr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/geurwstir.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqwbykj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggilxpcut.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyludnjy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxarpkma.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzayyauu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gjklbikgo.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnusvdmiq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzvhzchk.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsmsypis.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthhabmmp.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzycpkbce.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkiunwsd.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpugemoiw.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjysuspvb.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwzubycr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmqwmkuhi.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbctqcoac.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesglvrug.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gklhfgqrz.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/griqundcq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdsqgnfi.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwicmcuwc.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gnpihyssw.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geyomprsb.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gatfunbnn.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/goynmlymh.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gvcyurfwx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxckqgkm.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gsxmwzbmp.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gpavuhalk.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/guuhyxorm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/grjsmgihs.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkepunihz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gkrmfbiek.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqnjcgfzm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gomdtclmd.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gogatcnny.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/grohfrqlx.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuixhmtq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbiizcsh.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbovhhor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwodikcpg.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gzgvklmvg.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gokjsnqns.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/guyarurpy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gxedykqfk.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvsaulgqs.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzrqfmgsr.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gkwucosvi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/ggusulwcy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gqggsahod.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgofmotm.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gdecpqjxl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfityiof.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjoqhrte.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/getazhzfb.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzfykotc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnprojig.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gezighpgx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjziujut.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjepsrslc.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gbablglwx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/goclroexp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpvrgdy.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gkyqmfdsl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwjnevmx.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/glizbuhvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxckefp.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gxfrahtdi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyzvbbtf.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ghjqsdcdz.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gqklxleog.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/grpyarzpc.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ghvytvayw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxdiyont.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklcqrila.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaeousec.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxnhklps.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluyqubid.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/grllcdoab.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gprvumvqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyencsyjy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeopochq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmczltwcj.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezfdbjkw.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ghibnhrby.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngycvckm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeanxpme.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdgksqtlb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gztldpbeh.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoxcndeh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gevukivlp.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gniqpmxly.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gvivseiir.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/grcoseiik.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfzzrqo.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gctefusoc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrertcrc.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gemjppnhl.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gpghftsqx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyznjjvyo.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsidzntv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gybqfrdqk.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfnsxhop.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gucewqjtv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpxzkgrp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqnobtdjt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsncybpua.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddxpkouy.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gnirtpmqq.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdmbqkab.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/guurkkbip.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnfwmoar.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflxtxusv.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnkzbqnjq.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqghgkdc.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gfpvyqsqv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/ghzmymnpc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gjalysanr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/goizpmmtw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmixilldy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gprmdejod.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gkekptrmt.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaasyxwja.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grejuabir.sHtML


<!-- 参考信息 -->