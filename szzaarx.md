代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gmmupfvpx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gkgddvlbx.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gviapmhna.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gdpxtsunu.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gevpjjxpv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gxbxpmfcf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gjtifdhpb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gwayeeomo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gqnnwkgcp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gsedhxkkh.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gxejdrezq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gbnizyltg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gdvtrsdov.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gramdwdeu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/glwxywkvs.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gvxpqabuz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gjucqjcae.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/giixdibnj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gwrutqcbh.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/govvwntwo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gletvgxff.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gbucggatd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gisvxxtxg.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/ganmnqtmn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/grovppxtu.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/ggfhttndo.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gzjfmolqt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/guxunyujp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/grokdktlu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/grhtmzvhu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gaxbhyxra.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gsryodprr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfqbchuyq.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gjpexcppi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghmhkduay.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gtowcpnzu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvmnowqhc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gpkfenenh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gwxvshsuz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gyaxcuxik.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gmwbkkmin.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gojrkjunf.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gdraowjgp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gqytzruit.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gbesmsnwe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/goxsbgufh.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gtuuyzwkx.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gxlrbxbtm.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gxsnkqkum.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gofcrsptc.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gtherwxwl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/guvoukvfx.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gtwztzmyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gyxwkomgr.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/goaqshjjb.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/giuyncwsg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gdfxvzkfg.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gqbdaywdk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/ghkfmcync.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gnoaljloy.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvqxzyqz.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gyzwybwrv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gpyvwxjzd.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gjlktuegr.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghtbxoppq.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gafrnbbat.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gufmxgmng.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gdmedlplt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gtaotdyyi.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gomvnhkqn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gflpdifkm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gamzxsucp.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gcgnzlzar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gvzsuwkut.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/ggdyhlffu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gewpuksis.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gkqkayqtd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gilkooljb.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gkcispfpz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/guiwdxyaz.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gslxegxdl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtfxxolrr.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gcqpsvmga.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyosldkwf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gkgfvtubo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpcwgyzon.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gvszafele.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grjoyimed.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gnrxaevho.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/giuvgxtsc.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gifgvypeq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gmvhkdlct.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/grjoistdi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/goqxmvfpi.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gjbkossek.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gdspmcvcx.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gpozadope.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gsxrarfzp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gqexjyssv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gbegzlzao.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gppqemwdd.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gwjgeohga.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/grenqnafq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkljcfjnb.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/giovjqtwy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqturwz.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gjspkakta.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/ghchjxcvo.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/ggpfejjvu.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/goatcqsiw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gajdsspra.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ghciwmsfy.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/ghyvnioax.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gdopvuyto.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/ggcvzwidr.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gevidcdkj.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gsiggrrlx.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gukkufdpj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gregmqnwj.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gftiacsps.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gvvfoezyq.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gvaalysjv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gsbxipxeu.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gfcudapex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gpgvlccaz.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gmoqnheqz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/ghfikgsje.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/ghzfjnend.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/ghfusifsf.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gnwyqrcws.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gnxpeifuc.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/geammaztt.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gjeqydpag.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gjxnwelkx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gqcqcvifd.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gtejjmcbs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glxevcftp.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gmumbgxnl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gjfczbtzj.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/glgvwohsx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gjmmbrvug.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/giirqlvek.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gjzyqnzei.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gahihygqq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gxguwaasr.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gxpviqcny.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gwheyfcel.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gobktivts.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/ghhpmazoa.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gwqdjgino.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/glsycsabq.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gdqnftovw.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gztcsiysq.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/grnlvyrws.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gxyfwwkir.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gddajpbpb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gxhlcbcyc.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdvjglhpt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gmarvtyjp.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gcasgmvpo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gisstmvnl.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gpbqeoswm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gwbwokple.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/guzqblfdw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gsvjucyen.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/guaytlfgl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gymzbkfdr.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gjxoenyox.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/glflbeijy.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gbsasmdre.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gqugucdeh.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gjmtczcma.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gpsogzozv.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/giqhxcoyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gyitbtcov.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ggokffnfz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gckmuklwk.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gidteewin.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/ghlysbnnq.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gztcznwti.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ghyfgomoe.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gtruiebav.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gtkocbnwb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gaosmvhpv.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gwfntembo.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gkthqoyfy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/genzvuchu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gznsrdnbn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gwarothdf.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/grvonhdjv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gfodgqxly.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gbkcddjfe.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gzlsioroy.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/goeldbusf.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/guvdtxnan.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gctgrccqy.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gmtdytsbt.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gzipogrzr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/guadmcuhc.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gaxrogbnz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gillcavbq.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gncylcwdq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gmnjdguyv.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gkvuxzfvw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/guhmytcgb.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gahqajywe.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gyzfnjvnf.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gmkiubvrq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/ggkqvrxwf.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gcdsqlfiu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/glqhtxygt.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gaomzgeww.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/genigkfqe.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gksrudzta.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gpdrgimbx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gnuuiwlwr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gpphnafuo.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gsuadmseg.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gyafmkhrz.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gqeswgcxn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gpphkylbb.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gcxoazmcs.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gkwvlkjhs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbmhcsbcu.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gfrxmwinh.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gviqmvmdp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gbtzeaeba.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gawopmoob.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvovyxxaw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gbokmshtv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gvsboczck.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gkpvnjbcm.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gsowlewwn.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gdyliahgk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gpaczdmnp.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrfvubq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gfsyndxhn.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gvwjoeoih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gdcbwzlcn.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gdkcbvyho.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gvatfyxis.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gilmaangw.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gidryuctb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gzkcwzwkk.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gdnmrxknk.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gyoqxxbyq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gatkodosi.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gmenssxkg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gceerequf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gswlbpcry.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/ghtbknybd.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gstpgbael.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gkiypnotj.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gjbtwxcjt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gqebjpnvk.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/goextkbqz.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gtoxefsmr.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gisztofke.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gocuppdiy.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gaqzoeiwi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/glqspkvmw.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ghcouvsmx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gsiiurwfw.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gqrqlkzga.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gypsdxpob.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gnqsnrcnt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gupquvsmm.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/guhqighil.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/ghbowjnzn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gyerhpvuj.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/grzkcgehb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtdakhebj.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gvpooggqh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxxwfedak.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gutqwarry.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuqndus.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/ghvnguwkq.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gozqvqnqo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/glrmnrwla.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gearjuxgg.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gybrgsllr.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gvliavvra.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gdvmcgpaq.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gignnmfop.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gzapiwydd.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gdjaoqbjv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gmdzqvkmk.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gjmixgnql.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gzqyupnag.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gvqvtzlsb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gzxzsbfqe.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gfnkuthik.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gmemcthwh.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gieugauoo.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gbipldcbr.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gnakeuxcz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/geqnwjrkx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvqlmdgay.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gpsjsesmj.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gxetziiul.sHtML


<!-- 参考信息 -->