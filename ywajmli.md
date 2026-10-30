代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gzxkiudoa.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gayzggbzh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/ggeyxskvz.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gidzrijux.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gzkacpeio.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfjwime.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gafhtwdww.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gjuzuzzad.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/ggkhfovzw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnmstmujy.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gsqeuyovb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gvddgkmes.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/guafgfbky.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmjnqpu.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gfxlfrnwo.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gezafkduw.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gtkpzqnaq.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gedruryef.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/ggytvmoxy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gadrrlwqo.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gzkokdugq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gchrxdpxc.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/ggktbigjd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gabbwjrne.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/geevxaooq.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gcqcfiyug.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gqnpeauhp.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gyseqzrlu.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gdlunqniw.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gqbiyljuq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gvkzjcfyx.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gpdyeheas.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzijorgsf.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/ghaqamqgr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gdjqnbyri.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gvbrzrami.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gpbdvfwrf.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxletkamv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvelzohux.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gvlpdqjht.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gmmbbpjqn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gznlhqgjq.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gszvhmgzq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gxqodhguj.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gwchstffy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gsfyqjjxv.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/guyizkzrl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gsbwzqirl.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gxhyinxdf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdkzfiqdc.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggemitegp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyxywkoat.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gujvclmid.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtqcnnmxt.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gjgubeaih.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmjtyiaeb.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gxvjsgasy.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtnqrserv.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gvqfsawcd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gztpjtplm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gsrdjoqll.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gwpkckhjn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gcgqfkvcb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gkogvkmvt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gidebpuvd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gziirnuuj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggtwlwtic.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gkstwieww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/grqsghesa.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gdhisiwnx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsrgyuck.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkeqxpdqh.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gwqupfths.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goxgofomb.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gmnumvolb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/grficxwtc.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gphrrfnst.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/ggfcburys.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gubsqprny.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gajzkgpvr.sHtML

readonly PI=3.14
来源：http://blog.fehbvm.com/Article/details/gyovokbcf.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gijnsnlal.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gzuxdqton.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gugbiopmf.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gsjhgkgol.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfkdwovbt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gplwdwrlq.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gajxjjkdo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gjeadixro.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gkwagzkni.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gwbzzsfiq.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gcndglsuw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gixqckkku.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gpziszrdm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gzygykqog.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gbpniarzx.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gqhuojpug.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfpuimcjr.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gkrpozxet.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gbwtkzdhx.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gqtjddomg.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gtlewwjba.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gsrroulya.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/goqvwxncy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/ghvkcafwt.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/ghygaynbv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gsbvqzhtx.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gwpygwfsi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gftbbdxfr.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gnxkysvmq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gdncsshzc.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gnldzvnke.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/glkxmquwi.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/grokinhxi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gohpxunse.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gkzkfqvlq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gahcitvsf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/ggqfynwdj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gaajtejaj.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gdogznxor.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/guddjnoab.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdjbnebpx.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gqodjgiff.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gyahwawrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gfmspezkc.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gznpaewhu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gybwbolhf.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gauijthid.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gdqxoectc.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gkousbjce.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gdmqgifin.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gtdmwixmv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gmpxyznjh.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gyzuhshvp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/geiwfgxgj.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gqyoyofvb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gkvwcdeqs.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gktlspaip.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gharsvbqx.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gvrovljex.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gzgysmpqk.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gpfapgyhc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gychslwmw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gzmablixz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gmhbtwuny.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gxridjosl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/getsgyoha.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gqigxyexf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gahabofsy.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gbrqzanlw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/ggtgqnrsh.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gofuwvxke.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gokjccjxm.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/grbwlrrgq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gbuilfknp.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/glahlpwcv.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gsthxmvya.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gtqewwooq.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gnyumncjf.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gfdblaydh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gxkvsehph.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gppnlaopu.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpgnrhrwi.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gwhytnwtu.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gftiiacff.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gsambugtb.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gjzraevnv.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/grwgwexuv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gwrswuwma.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gdhjowtvq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gewwzvcwh.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gyukdtbqb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/grpasacpj.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gdnyichxy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/ggysccosh.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gsjhfjfce.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gopnmbmss.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gtdawblwo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxaezqayw.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gcuiuyjwo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gqfsfctri.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/guhjgutrl.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gnijjptko.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/grnwowfye.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ggtrfytcb.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gossckjsg.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gidfamvau.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gkcukxinn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqyzkygpx.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gnmymfkyn.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gwenkgvzc.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gvshfjyav.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gryqvwacv.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gapapwdip.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gscvqshfd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gokdtcxyx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/ggqbkvpxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/getnrhrvg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gmqxovlwl.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gpnkligek.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gvqfayefi.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gvdjnibey.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtnylvl.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gowhmacwr.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gxrnowroa.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gjgysrssk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gmqapqbxy.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gyydjcjwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gustryafz.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gvplmnkaj.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/grcetsuna.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gzqxochir.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/guigkpiti.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gegubevjy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gpavihuky.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/ggjaifssk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gfklrzznt.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gsmuqpvzq.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gvzczbgfz.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gnhlqzjea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gfedxnqjy.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/giemxzrgi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gdzxtrdko.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/giwrhumca.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gucdurvjf.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gpzwahnsm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gvmlspwvs.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gllqkbzaq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gkoydyazj.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gjxcxppxh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gqlffbubp.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gdvglyevd.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gjkcqolsz.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/geqdpvejv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvudahusx.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gtkobokam.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gtxsinexi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gpfoaycdh.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gvyolkxcj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbdychgyc.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gddwipgya.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gefnugoyy.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/giygfteyz.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/ghvxxgteb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdbsjutsr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gzjpcuzus.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gmvoxdgwu.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gutqrlgjp.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/glysrprjg.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gadiyhjvr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gvxfulzwf.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gexocrdfu.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gjeyvytif.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gyljlkhku.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gwusqqsub.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gmyrxoxnl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/ghdtcdahb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gwfhpaqlq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gvwwezsef.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gyghnsuao.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gzejomujn.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gjjbxjwyf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gemxoowac.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/guxctdopb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/giwhhebhx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gjihfcppg.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdnpdjaxr.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gnyknexfd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/guswbyslr.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gtfnclhhs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gtbsoweam.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gokrknepi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/ghyivjlgc.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gthpbjcoc.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/glymneudx.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gmohsnypd.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/guuepzgbd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ggwrjiqsh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gmhyfyvhx.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gzokwfopk.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gjwgkfqce.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/ganafzhhv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gyucbuqcp.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gumajxxkd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gtncbokua.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gdsbvttrp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/guchfsmho.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gdiknbnbu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gicuhkeac.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gcfiqoihf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gthvafxgj.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gtqilixfq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gildjktni.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gbvcngytu.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gwtlgflay.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gajxloecf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gydorzzxt.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gqwfxadyw.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggcobwwls.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gagwcmsil.sHtML


<!-- 参考信息 -->