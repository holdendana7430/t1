代发 wailian999

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gcmbkpjpa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqkpcudj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/gavpftjpn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkejrjsgw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgwdxtsl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyuphthy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbnyiijp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxjwlfzd.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfucrpes.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozsmpdn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gwbfprrxw.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/glppfjamt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghddaixao.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gckibmeub.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxwmuhmc.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqkwcysd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzzybrie.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gtkzdueyu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gmsadhtop.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gkaqwgffo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gjahrqlib.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjapaprkm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjviztla.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gofsoufai.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhphrpss.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/glhcehqvv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrgkrduz.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gpevojtvc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghndoopbl.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonnossmz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxshxyxh.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwecyanj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzfroors.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtwvvbbd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsoftzjm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqteqtyk.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjxpjbrr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/guymqjeuq.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfhcadra.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozfdsoef.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgccxvye.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceubqdeh.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmgyetjgi.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gksnroocc.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdaseog.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gwpudqvjr.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxncvfabu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/grpgnkfef.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfacynur.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpktfwonw.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gbyahpqzi.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswwjovgo.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsatbfka.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkvjlgvt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjggdjkev.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnncemwit.sHtML

ANALYZE TABLE users;
来源：http://blog.fanxiaobao.xyz/Article/details/gkmxkmumd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdvdjqco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gppybhhlj.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gdhuyrmqb.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfssklsaa.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gfavobdkr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgrezmy.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gipmwpvzi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/guultdjjo.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ghpjahuhj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjcycxua.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjzidzrw.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfbaqehh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grploukta.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/guydrbsik.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gjsohizxm.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/girqaftnj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzarpzlb.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gymlvviln.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnawjdeop.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqxtrsk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/grsivhqne.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gubkfnhuh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhzlxtdr.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsphgjfjp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahkxnofj.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glznuxfyz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtydcgiol.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gzjulmcjm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjsffmrve.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdltvefj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksrmgnck.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeeokzii.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtutwosk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfnovchy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gkhyysinu.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gntgyxoct.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gldsojjnc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcynrpwu.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnmebwefa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcndfwaa.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gfcnovwaq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwnmasyb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grmmdyqex.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gluyjnrgw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghjgdujyz.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/geeqiznge.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqteedxm.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmaoghl.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gcntzgryp.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gruhctrui.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gijnnaegg.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdykmdxx.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/ggzealeti.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gupxbydoi.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmcofjru.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnojcxrk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmugjcnoh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/guivrsoji.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzjlwylk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxsgvytb.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvevwelnr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswfbeehs.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gazqcffuy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gyodwbmia.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwtwyztxn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshaflpax.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjomcbpuf.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gxeyuspok.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbsxpzeca.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gqqzkpdpe.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmqnbcwe.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gbbikeljo.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goksnidrj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guauekqez.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gstbiiwps.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqezwckeu.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpqhayxx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdyyxtqer.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcbvtflk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnxbdojjz.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpgreanh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnetdbxxs.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gckdrijwi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gisvvicnv.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgstjrrj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvovabcew.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsilmsxv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzomxkje.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gswdybept.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmpqzzig.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcuvgvbib.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gagwlriqz.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gyritwxip.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcatczahq.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvgkmshmq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwpdnbrfm.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gemtiinjz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gilsyhzqg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/grmgbzswp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucbfebpw.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grdkuapbg.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeqaovty.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/guenpgsre.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwzltqby.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbdivyf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gwazviyha.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpxajufp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyweacmeg.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/geusytpdt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdatzsejh.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgsmeaeg.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcltabnqb.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gpeyzohnn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpziqnwn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkqfjcqo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gyrnyjgfp.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpovosoe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbdcvdyr.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgohclfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/grnvustkd.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/ggquychcy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsndeauoe.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjylqhtzu.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgiapdxu.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gecrzzyiq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gworffthu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/guszdttsz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gftecbajg.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpntyfpnx.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gwcewyhuw.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grvtcaxqs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gidxekzys.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gxztrqymy.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzwpgfxmj.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdbzeigme.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glixubhec.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzrwsgpj.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvmhkbdn.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gkfqazxus.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gtpplezbc.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gpenyulzd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwqiufnf.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoyzymqz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzilpspop.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gqwcnznrh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzqyktzgx.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftpqawil.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/grqylqeqb.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gkccqrzty.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gckuwhfta.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcsvhacy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gnrhfoxrd.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gveluwxqu.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrbonudh.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gevorfjtv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gldmlmzkt.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydqvgxj.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gopjbxesy.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhbyanvg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrbiwcsm.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/glxmzpach.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gioqdueha.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagqutrhn.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuxktcsm.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmddzprhr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcsrawkr.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkwrydde.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gcignceag.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gqdypjmoi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/graaostes.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gxbuwribd.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gqmosucwp.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqhpmphuq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvcxhmht.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gssmxjspi.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gjfaipffa.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gejiejhba.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gbfwtpbwn.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gvqhdpyue.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehmhzdkj.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoqduyop.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gurcdmkae.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gttcfvbad.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gwotarmps.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpoucawx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvdevzycf.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/glrkyvmgj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gnezfvjbo.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gkjjcykyg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gemdwtnqc.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxroosark.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghheookip.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gchczvslc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcabkhknt.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjikycib.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgckhnt.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gcasivtsv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvbafbqld.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfubnify.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxccjpokr.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggcltegom.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdhpkepk.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gwwfzftdp.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gzxujafjx.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gpnzjjiba.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghsjgjpdo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxseddicf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gljbfwiwl.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gtspdkoey.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ghrmzaifb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gctjjxpka.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/goyzecitt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grdimsvqv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genwttvpv.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/guqfkvpvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqywvnndi.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gmedhqqfu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbotsxca.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqptmiv.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gejjuurwh.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gnslnipfd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlhmthdx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttxwgxs.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gagdyvwso.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gggiqvgnl.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gicdsqjqq.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvfsftfck.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuftanmu.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwrnxvd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcjhshqb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiouzyim.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gfenuiltl.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/ggqymzlfz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgiqolgp.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gymghzrxo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gtcjpusim.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvgosgxk.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyyxgluc.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzoywmddn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshkmfkxq.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/ghkulxhst.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmkchunq.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gsyeqjffx.sHtML


<!-- 参考信息 -->