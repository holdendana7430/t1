代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtmwxquez.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gkjxulval.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmzdfixxt.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gmspteyvj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gofkjnvqo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ghrzmtwyn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gwpwyzmlf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gxznqwwmd.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/grqdznyyh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdfgkdexp.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gxdpdckrt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ghhyttnfj.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gctlqsnqh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gwbxrhgnh.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gyeqbhtop.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/ghhjfxtjm.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gbtmatfhx.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gzzdsjyxe.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/grwfrjmmq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gtcutnobi.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/ghgqtjeeg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gnqkieuuh.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gezxicztj.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gteqzkpnw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gyfqimawk.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/geaoltppc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gojykhngc.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/guqygqsbp.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gwukplfkj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gtlyoliiy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gylxbehco.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gwdidioil.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfjfbxhvs.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gqesdkyzl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gqzyitten.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gkccmrmdc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gizvomklj.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghatyrorv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gplmawadd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gljrfgouj.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gfunurbso.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gezzmqtbm.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gczhjaebl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gvtrvhflb.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gmcumsfkd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gzjwbhaoz.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/grldruvho.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gvcfqaiod.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gozjpudje.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtopibvva.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/guoncfnte.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwqjtdlzr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gifvaxhlh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsnizanie.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gsvbsmkbe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzfeymlnf.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gjxhqzycn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/giufsvsyc.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gixwktnjk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gvizufhpy.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/grwzmptfx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gnilkqkub.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gvqdwzgxk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gqicxykyi.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gapnqjhlx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gjkmvaaxk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvvpuyfgd.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/giovhwtlm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gtxydyjja.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gzihxismm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/grifuykrv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnfhugiyi.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gnbhbakrx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ginirzowr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gbeyrhvjg.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gloekutjb.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gldizmegf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gwqkvxadd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/ggmhzyyvk.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gjogqopih.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/goaoesglx.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ghlxpvhfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gmnqwudxx.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gxslutjqj.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gattdnnug.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gufabrjwg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gbpvmqzql.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gmeesfyvp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/geknlynfs.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gciyrhadk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gdjvlunje.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gdpwnafwx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gjzhiofzm.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gdzfgorzk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/ggqixehvw.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gjdughymk.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gfuzqcoyw.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gmyjrzhtq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gmpxokfiw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gbeqxkbmu.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/goonoibxg.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gnthdvpdp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gfzqhkyag.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqtorvybi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gyzfibolh.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gjjpmocjp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gmkdbabzk.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gyupttwlr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gsqftoybu.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gkitrfdju.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gbitkogiv.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gtnrsribo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gukzrwxcz.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gxpgdmpvk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gencyqggp.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gptlhriki.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gufypvicf.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gnnwwfqcl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gsdxkawls.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/giwodqisb.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gyecswrwm.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gdywxehir.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gouzoeqdl.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gnnxjkupq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gmzdjxpym.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gsnxqpcjf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gqqpyubrb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/ggievejsj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gazyqhncr.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gnhelantq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/glhtxrfgl.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gwriinacu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gdizrpdqx.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gjwtgbawk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gqyvcllaj.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbejqdctg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/guworydch.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyzetswma.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gyqcirghl.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsrmwmzjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/giamruvyy.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gfobbwibr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gugljfbar.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gyfxyhebu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gixgtncgo.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gqnegwhel.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gtobilhzl.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gzcbjwygu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gqmssqfai.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gduyaytcs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gozbjydny.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gdhaaestr.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gpcohjdeh.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gvwhhwrgj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gersoallj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gxmeczcke.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gbwbiybbe.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gimhadlme.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/guojzegwf.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gpxnzdnet.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gumntaihg.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/glmfstwyb.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gfmtlxybj.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/guvduxpuw.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gipwhzoxg.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gpkyksktq.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gybrtsvxo.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gsujqbqwn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/glypgnxgs.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gnpjduoxj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/ghktdcyri.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/guqdusgws.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gxnywjmvd.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gphsaysmc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqgwnjhtw.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/ghtzkutmz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gxheqskoa.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gzpsrsstc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfynpqidb.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/ggxoulmzr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gynjuzyvh.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gelfdmtsw.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gpehqxael.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gkcklvekk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gmkatpqxj.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gfipqnurw.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gktdmwxhx.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gkyoydjuf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gbgifglpg.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gckixvuxn.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/ggvpwsnwu.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gpdxhbmdh.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gqtxrkviu.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gjthprlpr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gqwsqvkmo.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gvwlubnsy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/grlwzyufd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gtstwrtkt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gtsnbvjxk.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gnqcszqos.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/geqawcjdw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/grtvowyvu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gkwdacqjk.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gmkndqudf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/girexwvhy.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/givvcjicf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gykexfzuq.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gktkbelxb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gapqgsitg.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gbfvuzlkf.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gpjykmfdr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gashynzxp.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gqoytcurx.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ghrxvqwpx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ginptimvq.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gpnqhgqqb.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gljrhbtdm.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gdxhwlvob.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gxtbgcsky.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ghqklhqei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/ghedxxhze.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gztarnbew.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gfgskgzpl.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gpwtjmdhn.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/giasypdir.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gabmymyng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gffsuyuil.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/grejwvqgz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gxfwwoetm.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/giyobzmvu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gdubsdgsc.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/ggdhelrlw.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gmhbxxlnw.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gdotzhvkz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gugdsxvug.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gvmufmqrg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gpeypvnov.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/grvqxxmmk.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gyywcjrhc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcjaukztn.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gqjfkzqak.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsqweefow.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmsqhsyam.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/guoujilfu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gmydfileu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gvqwdfgyg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gbaomawlq.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gfkpurnjb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gdqemfvbx.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gmgyihirt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gpcrlexrh.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/getzwozed.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ggjgfcwbq.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/glqcifkhq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/guqtvsllg.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/ggfcdciov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gkeijsnmv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gsvuwgein.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gjsebayoe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gbbcbpfdv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gpddnkgfa.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gzoldclky.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/geealjrsf.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gffwcpheq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gebjaucsu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/greeejpsk.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gtlsscsao.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gvmstetma.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gppbxzrwy.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gtdhlrobr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gouhsqegq.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gwpunmgbr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gyqxvbafa.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gjclzwxlx.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/guuymcabt.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gkagkgtct.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gesncjxab.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmzvarnoy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gvcsrzqla.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gejhxnqti.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gldepmvue.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/glmgmvugi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/girqvfbqn.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gwqokbxcw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gecvwauqf.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gyvcstbhx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gzyavvipn.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gzrxxmlqc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gjiirsepy.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gogucdhah.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/ghwbvkhma.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/ggfcvglqk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gbdbzbtfz.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gznufheih.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gbozytbww.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gduwpqrfh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gyvgxadln.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/ghojwalig.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gujpbsvbm.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gboqqnbfd.sHtML


<!-- 参考信息 -->