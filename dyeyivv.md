代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gadzxtzrv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gmowwaooh.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gmsmhqlwu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/geqigltjh.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gygcmagty.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/griyyrvyn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gqawvhrek.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gmwrgvdcp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gbqeckuff.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gpoozneai.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/glfifuqdj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/guzgikzwu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/guwfeudln.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gszxuqcbl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gddfwqgxw.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/ggyepgobm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gmfwxgjpf.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gptwcdppg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gmnpowthf.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/goyezknje.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gmhhdlgij.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/guufmhdav.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gbzrfdlnu.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gamsnvhut.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gponwawpa.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gyudqlovc.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gsqyyygir.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gznkppkwi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gufyooaug.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gmlrxocmw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gidimosjs.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gpgdcqnsf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gsdjghuos.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gwfgedxlr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ggasxovwk.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/glryuvbxg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/glifxbtay.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gmhlazkrr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gfolizqge.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkldwwdcc.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/ghsboqdwa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glnyamzhe.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gtmsbahch.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyasieamo.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gdrtdetqb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/glpxfdvrl.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/godqtmsil.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gnkcvwxeg.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gstluhqvk.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gfdywlrpl.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gexxujcdx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/ghurajdbi.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gpsnzmmcc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gskqhpvcs.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gtnzaqfyk.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gnydovtpr.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gnestvpmj.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gyypclrsh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gsfmdhfcs.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ghjrkbzzi.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gqdkrusju.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gpybhweut.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gvanybghg.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gwbttlrjp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmpnsmnze.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gpgakhzps.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gsklsbrto.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gdpsgcofl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gvrduzhgl.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghndxzgub.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjsrvzkfy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gsysfmpkl.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvanqop.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/grgbhiylw.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gtvseurul.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gkqhpcktc.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/grzsnejze.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gyiduvnxn.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gkvnmbflo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gyoxeypnn.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gvnvgpxbi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdueqejdj.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gdtpexaux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gtwcccpbl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/geqwfsqno.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gietvprev.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/guqqsoqey.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gvfaeyspf.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gluwimtbc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnflxwhat.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gzkfmoiqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gheyycxwy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gzjkbcpic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gjezfjvlt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gpxfkkvcb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gjpanvkqp.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gobvdcxqe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gmrjwsbdo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gymmgkpvk.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkdembwmb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/giqswxejq.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gqtkvberk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gxkwuelip.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcdirpfxn.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gjdeqassl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvlenimnb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gzdiovqmh.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gndbshror.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gjlgzupxw.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/ghnbyupig.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gihfjgkoh.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gitmffayk.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/goumawphx.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gdivagejn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gvbxdngne.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gqrowudgb.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gxkypwart.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/geiipcpne.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gdhrojrgy.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gjywzdlhq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gknmzbwou.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gjgigwbqx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/grjanvjau.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gyoarrrzg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/glehqamqp.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gztyiqyrt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gcybhuxif.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gjvdwilxm.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gyomjvsdl.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ggzjkdygv.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghlribpob.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gpfcfikpf.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gfptgaypc.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gobwkoycb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gvyhphdpk.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gmdldmsza.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gbloulklx.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gyhcokuex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/ggdcecugj.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gkoiupqeg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/ghzwtrtqf.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gjbijcyvq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gsbvnlznn.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gckfvukrv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gokbjljec.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gebbttmun.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gqvynxfra.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gbcssqnbv.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/glphrydvt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gxrpyhlgu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gxerprgmz.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gafazhmny.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ggymfmefz.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gfixubdrt.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gtzkmslfl.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gokzyblfx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/goxggyeeg.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gehjjxgeq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gfodbiasg.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gkopnaclb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/ghlqrqhee.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gxjgrikpf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gozoierqr.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gxlqjldsc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gwvgeejmr.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/ghudorfxq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gsoqkmtav.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvcsyrarx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gbnnducog.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gysgladfw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gcbtwfyjx.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gdhrymjlo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/ggkhhkvey.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gvagehkjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gauglndsi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gmccqhvcc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gjydxfzco.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gxdnenljk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gnemlubgy.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gvzcpqkol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gpeffuwir.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/guknmblyn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gqrejhzch.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gwotuqzvt.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gymdzfngv.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gwhaufhnn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gcechhzwd.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gnqhjnogs.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gadjkvtxb.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gwktvtyjl.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gbbvscbbd.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gumqvyobb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gzittdhid.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/goftkfsvk.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gnouklsud.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gjtyorowg.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gusnksnio.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gmdhywwed.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gznwmooto.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gzcqxffer.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gumbryppv.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gqbssfzel.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gexblwhoa.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/glfghyvfs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/ggojojhwj.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gsuzwoork.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gbfrpdndb.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gboqfqbog.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gqexruamk.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gjsjlngvj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gpqabskef.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gptrfdmkp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gkyzkdbvt.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gecqjftzy.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkrajtdqt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gtiucdncf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/grtlpajbo.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gvsrstjjq.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gazlyddbu.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gnxgjwedx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gqxpxqurg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gwmrfxidn.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gfmvdohaq.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/givbvgovt.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gmarqpilb.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gnzlibpzl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gsdtnvfts.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/ghjhztjne.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gxaminqqp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gjcxqqlbt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gfdyyjjnj.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gzagjwyik.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gscymxnnh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjsjifdfk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gtapugozl.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gusgevgly.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gyelknyke.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gwxercopx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gulvnynzo.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gtsqovxln.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gvbgpkehh.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gyzfjqbpd.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gzbvlshpv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gafgapemt.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gyzxjhabz.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/guctrdqkn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gzwpcwbcq.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gewooqmiz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gfbdrifop.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gasmyikzz.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gosjrvwiy.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gdhfcitrv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gtmzchfst.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gjimakrey.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gxwhjoews.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gfynkajyw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gluvfiaxb.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gwsagelsc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gkifjylmj.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gkfpdfxxg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gayrjdkwo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gdslfzdqz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gjbobntrq.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gvwppphcg.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gxhtyvapw.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gvuskdlvk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gdfddmowq.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gbgysnrip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/ganxcnmhq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gvzbkyzse.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gmfqazzlz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaezcxmlo.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/ggqmcrnss.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grpigklmw.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyvussjtv.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gmgipshjp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gnehnypdz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gonmcsplf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gxmamvwhz.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gvpqtohzm.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gpzupohmv.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/ghivlczrq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gxypvbtad.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/ggblqprxx.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gvflrlfqu.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gzmzzmhfj.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gfgmpedzm.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gqdiyauxv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gxgfxqkwr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gxlcppbex.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gpwuhilqn.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gjrmjkfue.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/guoqffzbo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gfmezzmgs.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gjkhynzny.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmjfuzbtg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gowdyxnms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gdpqhvuzz.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/giszweijz.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gokcsziag.sHtML


<!-- 参考信息 -->