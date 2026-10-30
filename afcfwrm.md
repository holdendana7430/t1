代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqigllja.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdytlandd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlpvmjwe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjzrotgo.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gpjitlxag.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gdtxstvzk.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbygxxfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gadkqpzpo.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdedcruy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gpenawrqr.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmnzuvku.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gbyfbyjaf.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gqzgkyktc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzsfxgvu.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggiatyhjf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaupzzrv.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfiwoaxf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgbaoagz.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqkxtjpj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjimxsas.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gdfbypndj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxrbkjzv.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gnvvyqztr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrcrditx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gfijlogsw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofkcfhcb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvexreau.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gdehpuzgj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlacbmcb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gyiaotngi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuszzwsx.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/godcwurhr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gsevwyjwi.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/goftpwwjl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gqvprsxrg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclbjplcz.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/githbfobe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmifposim.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/giuwxlgia.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gqxfvpuxp.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gbvyniuyu.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gxvooeira.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/grkcedkym.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/geaxwxtuz.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghydfpxpr.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhzegxpb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gdbexkqat.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gjjioqbva.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicwtvww.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/grqmeocnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/guejwgwvt.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gedxuwbqb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoufszyi.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glktkmsvl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqxajybk.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gsgcosyvw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/goyttadvk.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gxipvfduo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grvephdkr.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gbffgblsj.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gornmkxso.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycrduixp.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gqgpofyab.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhfwaoly.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/grndvgxqr.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqhdeusun.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdthloxl.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/guodydvjm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxwrtctw.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gogdcmugv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutpdjiej.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtchcrkcv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkklvymxu.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gosivbqqr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtxyfzse.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkpqigih.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmvigrrqi.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgtalhsi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gogfbadwh.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbammvuhi.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gofbnutox.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/geiusnvrt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gazsaakwl.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkvoyecd.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpiorsxmw.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/ghyfvacqc.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjbnjtlim.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzswositc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwwkrrhjs.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfcxuykc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfimutxz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gbbueociy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvdkfwqqa.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfanjtqwx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gewgybfli.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gwevaawae.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gjchjpwhi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbptzxkwi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gcattjsgo.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeuneetx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtglstrdd.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpkusnzzw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfssntai.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeatzhlx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gliqbfcsd.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gixqrtyts.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmavjmhc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gtidpbjpf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gigxcoknu.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnziybkfz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gixknpawo.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidpjbij.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gebtzjhav.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gorcridcy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjofdbba.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyuegadub.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/geeogchgd.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoodhmox.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gmhhfsgix.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gadfwaksi.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gkakguwuc.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpplcrwa.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfjvngzvs.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzqiulm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gdydmcayl.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/guztyoxai.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gokzwcdyl.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbyipjwa.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuqfmvrh.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gpevjanas.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgraldsu.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gayonshmr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmnogdss.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gluccxlbj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gojgsnkuj.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/ggscustty.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbmtceuq.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gatwwkzun.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaebzgdsu.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlmygyfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gnpeotwxj.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwzuskuzx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnfazcel.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoqgstis.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbrsovuaw.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaaqjrex.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwrzkjuxx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gkglmmkzz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gprqkextx.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqgopoi.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdpekiqjf.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gobhefxly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdymqdcu.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizonqxx.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gwylbiyiq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehhegikg.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/grygtougz.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxknkylfr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/grgnzzeql.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gesektboo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwbksvvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gkwhqcswr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gzghoeelt.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gecyveskm.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrccekaf.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpvsxzdtu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gscnabcju.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gfymmlwuo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzlrrtyd.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnclrrfvg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzzxhrtv.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsqwdfdk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gfecmemsa.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrblkwsy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftxunbjp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gghlbxpjq.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdhkdssq.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gadhmmyeq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtsgapha.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpojfzfjp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gllexlrux.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdueqeovu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwfilwwa.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gipuzaogm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/glurlojmx.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gwiwczvkq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghulezsdi.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzfkgzfe.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonnpwrik.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gujkvguqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgcmmrtx.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxqxboo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/ghdabilir.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxnzhtrnz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcvzjidv.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpeeienn.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gthnmyasq.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyushdlz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/glqdvqyjy.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gfjpyldsw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsigvuxey.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gbqerltmd.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/galbgeqxc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdxssbsr.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gluszvyev.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqqtxmrh.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glegvvduh.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gqkgodlwa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjggynl.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqcxpekfw.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gdedpjhvq.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvpppjuv.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryyobbgd.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiehalhq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/glhpzkhhe.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfhyycpyh.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzikztagp.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/glhiwedpg.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvxnmycpa.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gqpyhlkeg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gfnogbjef.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtepbjwgv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/guggwwhtg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/grjdabcsl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gwyctjyuh.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/guobaynnv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpalvilv.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdzjdkc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmggzeuj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gkuootoyz.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmfcjwaq.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuzodyyo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkzuuggm.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gbtjihekj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbszvkeqp.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeymglru.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexqxkumf.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyumxcfln.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfhpfwln.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gzglpmhuh.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzkvkogm.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gczkrmekq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxdccdru.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfmyegptt.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvgyamtx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfevcpokp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxabopqyv.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ghgmccyqi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdwzasex.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbgmcuhy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gyetuvtwj.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdoqfcgn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/galllnakn.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gujzwheue.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbglywfpp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzugpurk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/glsbxmsvf.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gipybtiaj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuanmihm.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/ghyylbite.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtdyipxx.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gyirgkwdw.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gioewjeep.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvehgsaeg.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxajnxjm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbtahcyb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gsggynpst.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjrjjile.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogwvzopl.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjwvfms.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidkqxgqy.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfodblqcp.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaicaxnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmilnyhfh.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gzkxfkavw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gewtppqfu.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/giopuerdm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyjwaefk.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/ghntmidng.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzkjhqpd.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gstmssozp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gueaaayla.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtedaxxic.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigstocvo.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gtytckftc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbqnuacf.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glswwvram.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gzxeluahv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkupfqmnq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxfouvpe.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyekbbnmt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gytxpjjns.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gulujdeqi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzwrkqnmj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdltuoyr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbylkvdnv.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjsbtxglm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtofpxlxw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvpruble.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfuyuier.sHtML


<!-- 参考信息 -->