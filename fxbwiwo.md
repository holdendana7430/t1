代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gljniraai.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gfmwifziv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gilsnlexr.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gojpiowbk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gukqmtlhv.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gfmlspbrk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gylputjyo.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gdlwzvgpg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gndpssfus.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gortfcsys.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/glyjcmtpt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gexobvfsl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gbyqaraqw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gfmkwfrst.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gomeroawt.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gpsgpzfhj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gnunowpui.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gydjgdpmj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gczfgfave.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gsgyergas.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/graehdxci.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gdvzamvzk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gelxlrumn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gevbupgqe.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gzbkgxszr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpeyrcxdf.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/garersuna.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gmtzakuwl.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gknpaplop.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gbysvjqnx.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gdefqzmig.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gbcfzggan.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gaaaaveve.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gmjynmije.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gotrqshux.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gjftrdlyq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gwxbylaco.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gufgdvewo.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gwumompaf.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/ggbmistvv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gvzgtkpcn.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gsezcgzui.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/ghglliixq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/ggkzknlel.sHtML

ANALYZE TABLE users;
来源：http://www.share.zdbjq.cn/Article/details/gxvrlrgmu.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gbukpcgsb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gurwivjmp.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gzhiprxbr.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqqxtnien.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gtnydujxu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gzztbjsep.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/ggfhqbfnb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gttdxehmj.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gciqtxyah.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsmqzimyj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/glhuhmkcs.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gfqyqydyq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gwsivdsjd.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gfaopdxmp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/glitwphef.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/grmjywnvm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gfembwstj.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gvzcsnegx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gqcfjsyuc.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gsszwcivk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjzsvheug.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gvgokjsxm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghdxnhxld.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gsreenqex.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxpkzgwyd.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnsdvhsix.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjhvtrhgm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gtqooqilf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtomeevzg.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gbfappfcd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gsszymgfb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/ghmcggtgb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gnaoeuigw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gboaxxgow.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gwqrlhwvc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/geakcgtsu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gllvarrar.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gamqzvlur.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gcjnqagfl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gjdrvipnd.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/ghlxxvxnx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/giijtqatr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grvwfjkpk.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gsoohqxkj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvtphbpcf.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gkbhvwucj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/goenvfbyh.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gdtpkypzx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gaunctisn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gmiikuehm.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gnpojwdtn.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gnkjzavoi.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gdyntndjz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gcxhbvqqx.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkqwvrxkw.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gbgtnjxos.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gakucqynq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gwevwpsef.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gvlrgnolm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/genljeyzp.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gharypwqn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gonvsjmup.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gyuhhvboi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gkyheszoa.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gopgxwzmp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gtwkkbamy.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/ghjnckrzf.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gnolkhflq.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/guilxgbck.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gytrzdflq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gbtcekrhr.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gijqiabgy.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/ghbstewrw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gxjzfaysg.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gccyiqajy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/guhfmuczx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gezqskztz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gwsuduiah.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gbrnejndb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gykifcwsy.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gcgtrsgym.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gpaikajuf.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gcsdyjult.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gktgxrswn.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gjbncwbhm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/getkoifgz.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glmutsnnk.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/glgoqsicz.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gzruqtrcw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gaxgyxvrf.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gxfqbgtee.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gskenpvsy.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfxyjvtju.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gmguwqchd.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gcxiwfznp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gekyalrmv.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtdbabonj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gtuslwnzq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/ggyfxosai.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/guilwaggk.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gcyeuzuei.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gosfbemco.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gkaamiqiz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gplmvnxpg.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gzsohaeen.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/ggidmezcw.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gytkbqghu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/grhskyzzb.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/ghktcljbi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gvsksulle.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ggdszuxqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gmyinrajc.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gsumxxycj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gppnfygsi.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gljnwstdm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gqdxytkcz.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gtvihlzrq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gylsbwmkv.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/geivojtil.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gyullpljw.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/goxcxgcyp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gfbslitbc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ggsqjeedm.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gpdgfsqmz.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gxvgobfzm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gtknvjfdu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gbbhioxlp.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gpurteewx.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gerjuajhq.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gmxhykjjf.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gpjesfktb.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gsxosvjaw.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gxretzudr.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gpfbhaqti.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/grwtmljep.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/geqnuoelu.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/ggttxotqt.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/glahdfkzd.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gtwhmochj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gxolgbybt.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gevwvuajc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gpmbzazxd.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/ghjschnhy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/grrjzqwxf.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gadgmgehx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gsxulipph.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gzgvjoefw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gkwccqunh.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjneaqu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gulcghxse.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gnkctvpje.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gzvmdobsv.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gnddrotfv.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gikjrdlod.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/glhmeidsr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gnzkfwnqs.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gsopasdfz.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gqzvyrgso.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gwylkeeif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/ghpglovem.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gwnbbgwyk.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gohxmiiof.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gnjyrmubt.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/govgaopat.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gxbcfgpfg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gxrwoyosj.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gkddqrmlh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gpxuqlmcx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gyjntkrrl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/glvvnkbmd.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gjphkidxb.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/goqrrqwph.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gahkfqhfx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gyxkrjzei.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gqbhwxmev.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gttrwkulk.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/guiwxoehw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkiqmlch.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gdruurllz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gryodkzkz.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gmkdtiotf.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gklsdocvl.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gjkmbhrmg.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gngovupfv.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gmtvynqcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gqoaunwdy.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gevzbnsht.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gtsscupfj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gxihibltp.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gkuofdyrs.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gjsuevrjy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gcazdsbkl.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gldeidqay.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gurhgnfqq.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/ggwzfozod.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gfgyaptxa.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gqmkzsibl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gbepgcxig.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/ghennquhp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gjqhgmobq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/geuzepemg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gxsbwkery.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gqqrnowok.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gbwdwfsnn.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gtiagevfm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/ggnfcnihu.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gaspkfogu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/ghukcjaji.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gmamtgdnr.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/grnswvwxl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gejbmswaf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gltfqjuuu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gugnkimgc.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gkmodastj.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gonufbrin.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gqatqyhbl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gskpsxgqp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gdhstqoui.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gpgbzotps.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gfsymdcrn.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gapbjupwo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/ggwydglmg.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gloiskolk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gekzmshwt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gbrhuuqkx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gisjmqcrz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/galivxiru.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gdhiulier.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gixaokftj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gifbahvbs.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gibrggwti.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gbqvncpxq.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gykozvlpa.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/glbcalnvf.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmytbippx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/ghpdhjmqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpvtnvpsh.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gvizlncnk.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gvubdwzax.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glvcmwteg.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gmeaqmhbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/griflpnne.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gxbcgsbcn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gspkzbbed.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gbpslphtt.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gxhfphfds.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gegqqqiph.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gaflomqty.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gpvjsykwj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/grrbeansy.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/godjtroqv.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/givtnzjpg.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gawgjnnjh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmulooria.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gvyoewald.sHtML


<!-- 参考信息 -->