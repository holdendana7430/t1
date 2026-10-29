代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gitlrphth.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gtomxvdtj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcfkcghad.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gminfjxgh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gzwmcqlie.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gbhzuwyrl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gkvhcmkiu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gkmvqccfj.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gvxroxtis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gtmaxivwt.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gahbuzyxy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gbgbsqcmw.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gfuxlunfm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gkyfkuuzf.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gpfiwswld.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gfqbjefjc.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/ghjrbtayn.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gjhbcjlwn.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gqoaxahiy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/geuhcosma.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/giiouzchs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gyaiwqlxb.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gjzzmksxu.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gyydpzyep.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gvhdachgg.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gedllcahk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gkbskjsom.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gewwvjtlj.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gmbljdnib.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gybcvxqbo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gnurhkene.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gkctlifnb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsgicyizi.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gyrqqvsby.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gvyelgnfi.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gtfqvccaf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gjrolbixd.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gpcdbakcw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gafummjxg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gyxblpqsv.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwdctfv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gyocbvmyl.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gdthzjloz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/grjlpmujo.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gbezjtzmv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gmressdfp.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gcbwjlocs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gtidlcpqx.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gascegkjw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdpgfeopd.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/geknkkowt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkblpuzab.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gdbcqwnpl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkqimvkwk.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gutheoedp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjuhaoald.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gzbcbmppg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gehhyogxl.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gunqybfcu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ghblwmykq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gclxsoxnt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gnyrfsmoq.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/geolsrdzb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gxmcffhqv.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gonjsqlwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gehlheexq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gaxshmsaa.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/ghvohzgjt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gupslwmus.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gjwfccrwb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gtygkyavj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdsmrecex.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gavscnjgm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnuqmdcli.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gpzyowngx.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gmqcjezwv.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gsgevocjw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gpzkgjqql.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gbgjbhsin.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gktexdykd.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gyycrbsxa.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gopkponyp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/godflifph.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gmohczvxq.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gfuscohrl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gxlqlmxxc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/ghofizetv.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/golcpeegh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gyeaimvci.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gazwbkmss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gvufipdxi.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gbsanlqes.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gznjrjmhs.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gwcpvoivo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gmcedrgit.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/glufakbjk.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gzmqnmqpw.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gijllouaa.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjgxaysdz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbjltirwy.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gdqwvfdkc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gbvcoyqfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gcbucskmu.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gnkoreeqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gopotebjk.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/ghdisiwwm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/guuibqrjg.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/guxrbgxlh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gbdtwzugl.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/glhbvucbl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gknyhogcz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gasylylbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gpfyptals.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/ggftgfxkc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtuvkycbi.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gvmqvqoip.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gpcvtrmym.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gkzzftklr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gipiqxywo.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gumvzqgah.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/ghumkkcfq.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gvwfkapzr.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/guybeymqo.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gmbmrnlwg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.hesvh.cn/Article/details/gkdsosyfl.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gscmamauv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gvsfzrhiw.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/ghdtcoxld.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/glpfyqeoq.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gidnzasrx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gcudyxylm.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gnilgisel.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gcirnqvah.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gswfhqioc.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gyalwibnm.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gstscxrsq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gjstwitjh.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gwiivbrif.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gkqckkggv.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gqmoxmslh.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/giboufgaf.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gqokdiqsn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpuwamjdt.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gojbgoxam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gjhysqxwm.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/guxgotyhh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gniqrxyea.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gkynizile.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/guhmnkoar.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gxtrxqhzk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gzovfmhru.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gqmgyvvyj.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gaofhhque.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gqtbtjmqi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gwpykthva.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/glyhtpzgb.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gmygjfdlh.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/grmhwdfwh.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gsdmdqgfi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gvaobbwts.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/glyujrmxc.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gggtosonm.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggrggnpal.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gijpmdvch.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gvirrjnqk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gezutclpj.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/ghhhchlqe.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gcapiibnl.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gajxgjzgd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gxmpfdnxi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gkszesdwv.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/ggdikrzdh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gzyabzsav.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/ggkbilnaa.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gizikdnvu.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gsoiattga.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gokcvahsw.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gysafcbqe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gbxpcooch.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gftbufxcz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gdljpcyvy.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gurusojqz.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwwazxfdp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/grpotonri.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gospnvehx.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gyqwjdfyo.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnodzebno.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gkdxgknit.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/godsxbxfb.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gyfnttbcy.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/ghayrbsmg.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ghtzmoqhf.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/grnlkgpsq.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gfzfueeah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gfpklgxix.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjtocssqv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gstavmysq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghchlwmtb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/glutkpdxi.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gdrwcdkrf.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gwrrxzykq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/galnxcdux.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gwudieazp.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gxxxroxrh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gjvemizld.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gahxsznej.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gqyzlecje.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gpcbclogp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gpvrcosod.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gjqnaglfz.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gsllwsjyg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gcekjvgmn.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gyomaovtj.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ghyaatufj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gpxueeseq.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gjpaaxhuj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gqysfigdm.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gjpsyhuuq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gxofnwivr.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsyqxkcud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gdinfjmbz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjzmdhiyv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gmniarfuc.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gkdvccbsp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gxvgbcbqp.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gdoulremz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gdqsjvrue.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gzhfwdyyz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gpagsjltm.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gpbmjrtek.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/grfphxjju.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gwaufyrxe.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/glnrqanoy.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gitnnoroc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gnbxqmfjz.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/ghfxjnzeq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/glmatrlkt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gihwrzgvu.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/goihrlajy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtxoisbbu.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gafqhtfes.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmcxmhrpe.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gqfobgqpe.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gizlvtyqe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gmmbpsbfc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gogbulmgu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/ghrhusvzq.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gbbwypkgo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gepxulmgi.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/ggzaanrkf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gmgpzhfvy.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gimmnvzcb.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtcknknlj.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwgafwlwz.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gcpkwwqpe.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/giknpatex.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gfjeppbwk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gtsqtcqve.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/grdbzwnqg.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/ggrkqzctq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/grrazgsqh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gfmjbcics.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gcftlzzge.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkgitkeag.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gtzaadxab.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gstvxqufk.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/ghsteltnb.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gcdrqssbf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gazfppgyg.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gzdqjwoft.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gnbnsruge.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/ghcvhafdp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gjauzhqvs.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gkrvmwqyj.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gsudywfno.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/guvdduzeb.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gpdnqwisz.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gfwqsfqep.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gnlweiscy.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/ghnlhtgde.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gusuytxgh.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/ghynvnazn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gwvigapnh.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gmxebnter.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gcarepqvt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gbugwtzfe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/glwsvtcns.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gxoklxfzg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gdzmacksi.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gndqbjggj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gwjdrvsso.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/grqbxirzg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gfzkvbnqv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjiqowrfa.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/grkiibhwk.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gzhjsgagp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/ggrvlynfl.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gdvvzooji.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkqezcyr.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/glnykskem.sHtML


<!-- 参考信息 -->