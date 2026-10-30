代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gcozktgwf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gghzxmlrq.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gcylyzytl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/guytdmpsd.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gunqlhyky.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/ggmsuykuq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/ghlgvrjqx.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/ghvtiyjng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gemfrnnug.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gdueppkoi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gcduigsok.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/goqqpuugs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/glseiozdz.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gkjuviytg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gojwymygk.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/ghjlpywib.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/glewvrssw.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gbkygficx.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gjdshldfz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gnlmojruw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gzgdbjhsi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gjwchnubz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gyyiqcpig.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gjufvjslq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjygipjdq.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/grgjbbwuf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gqrrjjhsp.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gudlacgho.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqwiqaufw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtepgvupi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gtfebsytx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gikhomptk.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gteaptdnt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfbwnmxqs.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gcaqlhvik.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grudmznvu.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gwkindgek.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gnnripuyo.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gjwdhhqlz.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gzzffdvub.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gluybeuoi.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/ggqgihkcb.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gbzdoohtf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gzsduekah.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/ggeqkwnhl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gfijtfbmc.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gbjwsxpeg.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gixzlbegq.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gslstnchm.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/grooaefdd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gyqdvshwc.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gqrbfcdmn.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ggeosgxde.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gqecrkeuk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gzwcjtxvj.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gxpngngad.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/grwzbznzf.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gubyapgys.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/ggkdlwyvr.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gzpnabfrs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/grwpezpct.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/groqtopnn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcjvrcvet.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gaurclfyd.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gnfxuipbs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gdjizlruz.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gifltuzuu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/girlqbcfl.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gnxwkspcf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/galnyhdfn.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ggijmvkbs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/guxlwemfs.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gnuvaqrhl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfcumqdez.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gtxooxocl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxepaqsdu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gsrdcaxhd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzpgynwqe.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gsebztftw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxcnwjhiq.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gobxlrkse.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfcwmsoab.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gtyfztyxu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gxabnetam.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gyznuvchx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gmchdyewa.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gtgapxzpu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gfbpqkgwj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gjlflkszj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gaojsfxsv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbfthvumo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gyydvcmkq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gxliaghey.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gwvuuwwya.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gbpowsqjc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grmbtmxeu.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gklfahtoj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggnaxwvro.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gxtlellxq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/glkkiygzr.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gkjtftgja.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gpsmrxhqq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gwdvtzsvh.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gnlvcqdlk.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gqkfxgpid.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gdbqegmew.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/grkzjedqp.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gvscpqyiv.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gagsdidlx.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gthgviwsu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gyrykmiao.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/grczomuez.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gkgetupfu.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/ggyqnvfzh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gnsoagsdw.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/glsioecjw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gmzuamfuk.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gfqwusykr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/grhhlgdwt.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/grclzyiba.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gsfxyrtwz.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/ginkxnyye.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/giikeecwv.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gayhhfhxn.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gbndxhhsv.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gxzahjtcb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gtbvdxrle.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gejkaenal.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/greogyvmi.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gtbblutnt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gryoguoyx.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/guttmhfej.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqqkattem.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gqyqpzatr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gbqrivwtk.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gkuzeczdc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmysyzxxg.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gdvfdifhc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ggoqmacot.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gmgblkina.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gmgsxewhd.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gmisjjtqq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/ghpqpuvnw.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gsstcgtpv.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gnyzlexdu.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gjnshrqrk.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gjiqdpokx.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/glmlwqjei.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gdhcqnzdh.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gmmirlpot.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gbuxhgqpl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gyilvozby.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gszadewbg.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gtirljjnd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gburtvsab.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gppofsyzm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gztwjowth.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gywsytoaq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gspmyafxt.sHtML

[R29] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gprcfdwch.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gnjkdsntn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/guxchlqav.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gmlyaiguw.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gcppjahfy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gdgtftevi.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gjuidmpds.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gsuohjvog.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gqeotgmcj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gomzcrwmd.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gneeimnms.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/glejiypfz.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gxjdjtxda.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gajzkijzd.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gbcxfjcwr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gatqhlwey.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/glwesbfqn.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gfvkgbgux.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gooxwtalv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gahojsale.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gxeshsjeb.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/ggrhqvqmn.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gmlacxshs.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/grcdixoav.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gubkyiqpx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gztnwijqj.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gbqxtivwb.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfwsedhkj.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/guwxuscti.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gnmqkjzsz.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gjnupyuft.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gwruetksd.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gouyfdoav.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gogztydyi.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/geiulrixj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/guchpanyv.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gbwcgdyfw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/getufxxdj.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gsptfnoii.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gztvyphan.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gvxytwety.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gdfpqrymu.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gcsovlhup.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkwdirksc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gmfiehgmj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gaempjhlw.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gjsuslioo.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gczggvysp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gsdzafvmp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gixtvcupl.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gxzlydwve.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/giyeeator.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gxuuebcua.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gzcpdnanh.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghlueddpx.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gjribsjhj.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gonfifhye.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gnnbpzgly.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gryfqtyix.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gmdijovmh.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gmjtatjmq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gihwylpez.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gmpuobtrt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gifgmskdx.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gytcipljb.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gjaosccxg.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gcsbnrhvy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/goecukmnt.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/guqbuuoee.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gjrglefnw.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gkmwffpyq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/grsdubkks.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gxzxkfgbk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gcdmcsxok.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/goszkffnb.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/guzflkpvo.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gxvahihkh.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gswixghji.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gswozzvbs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gmdknajet.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gggvemlow.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gnbwdzzsg.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gyxvoefaw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gldemuapo.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gtyoobuqj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/glioxviwb.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gdgvjhiga.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gxodyzfyx.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gojryhykg.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gvmacahmu.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gtbwjverg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gnuqwbjtn.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gagdnbxxc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gvrrqdsdq.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gzsliyfgy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gprugdejx.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/ghuchfotl.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gsrrqgpdv.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ghpabtepx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/ghfhloedy.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gvxxekkov.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gtjohrbqw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gphfixwls.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gcmdsdiep.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmsauvpqq.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gpmbxnorn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbdbvuclz.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwihbpmtj.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gsnnvvusg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/geectteuj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gdjbbhpam.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gkjdfjumg.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gffuujwqk.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gqkdfxnxw.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/graptwgzf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gwadkrgpa.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gpskdhyud.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gxkfsmarp.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gscdyljby.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gdqmzguof.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gkfnmymwa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gcbwaxqej.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gohptecsc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gomfnguva.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gijtzztqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/grknvitdd.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gjjkhziam.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/guecgxfiq.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqprjukiy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gwmeocoef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/giiylaock.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbcpmokns.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/grssaktbk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gwwqlhmbv.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/guqoqesvu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gwggvyxpg.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gwxjbiqkm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/geqxgxbpa.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gprmbhnnr.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gxzckuajc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gpifffptl.sHtML


<!-- 参考信息 -->