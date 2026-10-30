代发 wailian999

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwsnukzc.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gqkreqpxy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gygbnewpa.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gasrrlybn.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grflihtyq.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gggqsemti.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gnowmrjak.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gidzwsdhq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqwokzra.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkvphuse.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gaseixqas.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/giptvazer.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsggvwyhz.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gcdnxrdss.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grydzjulk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/ggbzgompj.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gvkopasvk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixnwofbw.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywgzwdms.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gynuzhixr.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gaifsdxlw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsagqzar.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gwhwqzsub.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gaixiqlcn.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gkluraoru.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/govdulwfn.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbmvaval.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbkzpaulp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbkdovxrn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvvkxpjb.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyuuvniu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqrakjzvg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjebcmaa.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqowxdgb.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gtmpeyisd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhywfxcn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqlirzrj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiiepsnt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdfcfryf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gtnsqfpma.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gspwzghfd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/goqypxypl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gwptncmfs.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gptbteadv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gksoyfmfx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjszqtxc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gplnmwtph.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gszhpsazi.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gqduvuszz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gprnefggn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/geuqolpry.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/ghlohstgk.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjobbeh.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gqabjnqjb.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/grijzwpwn.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevkxcvcf.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gsgcfhhct.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtdkgsvhz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzzuspsr.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfqebrzh.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvsysgre.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gczjjgybs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsenlalxy.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdmbnmehn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gkfktaijv.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzqgmsoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmxbtreg.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/goietwsro.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gudndwmpz.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxhfybfe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvjgswvue.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gugotrcpq.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/goithkvuc.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyqtjvqo.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmubrgpth.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ggeydslil.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/grqdxesbr.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gudulweio.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvaigyvc.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqnmutdpv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gikixydfj.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmvqtwpy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/guwewwolu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyiwkvop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glyfpxwpi.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtucjezcm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjrjvlhu.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/grcvpisfs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswszlftv.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtvniyvtf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrsrxbog.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnblnspnc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcqpodyn.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulbhijbg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gokuysrdj.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gyvtfzgnz.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyszopkdj.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwekevdpe.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gleorlefn.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkngosjjx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gihnnthea.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcscfxjz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazgegazw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/giurbuhvr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzranubp.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxbzklsf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gqrvhpaeo.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpjbxaan.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcossusa.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gyauhwiws.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gvettnuwh.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcjomxtbv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpaspxj.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunlzdbf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/greqtahuj.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgpmthsh.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvoppiowr.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gesgryyyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpzrivhi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmhrskbq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gapmoeefz.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gspfzvphj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmllqwmm.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gdvarjmvk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoujkqxv.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzahefpm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsccnqzy.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycifedoz.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/genmvmbaw.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gyahzmhvk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gocxxeiqb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvplqheu.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtprrsqzp.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/grhnhwrli.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gerkfrjcu.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gqiddnjtg.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyqohbuu.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsaqsbkp.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glzqmwuli.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giiflvnco.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gxowphglc.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/geetlwbwe.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/geprygodz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbkoanwf.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpwcbamh.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gvvmxppbb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gibleywma.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gceppjjgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktoblpid.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsoiykjk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gneyvnmgj.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowryyndq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiqgdwcp.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gvbqcvdxg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmylhrppk.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gxzyhtagp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gcznmlkrr.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkbiwuuj.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gumbcidhi.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gympiilrs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gghvowujx.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbosnzeac.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkzkxemh.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gegqjxhau.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gjclnbuvx.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxfkbgzvn.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrasttle.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyprzojf.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gcmaxvxsv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqmkghbt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjfiedva.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gsqgnnjrf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gdzeyayyo.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbzykwopq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grsqrlisy.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gfinivwzf.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfpmdvlu.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnbnfsibe.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdioigvkv.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gebliqvix.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gzhdqvniz.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcmhwpgh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gpqcddytk.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsajkiykm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gwpttqxnk.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gpkumoozv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshxsibac.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghehzrydj.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gukwmvhoj.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gxklqfonq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzmjecvoh.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gherdmkti.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gmdvtmoev.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnajpvfdt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjofhoghc.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdsqqtav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gpcuifnly.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyjxkwmy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giesjkvzx.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gdilxzzem.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gxruvifxd.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdjfhfzl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gindrpyly.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggirslvgi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmbryxyh.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdgywdok.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgbthzqi.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaatdewq.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gnwvdfhra.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gwofurmaf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwbuzxgxa.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gfxtyemyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvdowupew.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlanqbpc.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gcawezrsu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gncfxnrqh.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gmdavzrgl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsykjahq.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gowdxzhcm.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsaoafoo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvfzufzd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzsaxtwb.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gophvvknp.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmlrpvvh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqjyyuahr.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtqtozdv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gaittykey.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzidpswy.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcyfiare.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcwucooov.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpthmojrw.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjyabduef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gosqtbsut.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdxqykyu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqihwinc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjjqclgv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gumjryvht.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gjkaegaid.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdczvhhz.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvrpdways.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gbsuafkmj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnrflzwc.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpgscwhb.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhuhfohp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gwuojdmdh.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gajqmlefx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gmmwmajcv.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlhohdxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/giocvyhop.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjopktixm.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gmrbrjlwb.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmkzxopk.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwdjxlkg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gralddmvr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscqfjde.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwsqerhr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gpkdhuyrm.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqttxkne.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gblhevnka.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gresbmlhg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/goqxlcfsa.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gidauhfgf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gshgpeqxm.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gekihhpcm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmvcgjoz.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gehmtskdy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/guytmmdmv.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gkgprxhcy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpldbvzn.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnwzxegis.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/glbpgpxef.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gyimpmjcp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/glaphqbzk.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfivojpsu.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gnnzddnez.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghuhmnldk.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvhfgigh.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvjcgdlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvciyqljg.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwjtxhjz.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gdlohvxeu.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxnkgwtr.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfdhxxkx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtryzrcp.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlhglawn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqyhtvxaf.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvfbwmbuf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtlmbtrc.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gqeqceqes.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/glmxinnaq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/grhixhtwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpthmtmma.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmtsgwww.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/grleumnok.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrkyymap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/giojvaepf.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgwbxptq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbevvwzgt.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxbuwgeqf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gooelnshz.sHtML


<!-- 参考信息 -->