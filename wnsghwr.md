代发 wailian999

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gbxxgwcak.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gwhrshclq.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gqenrmjqf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/ghbikqrpt.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gxinajakz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkenforag.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqqtikr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtbxmttnm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gsjhhscuw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkdzfppzv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gkzctkvrt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpvapwpzh.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/ghiyqzxor.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gpbbsfalr.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gzkjgwxxi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gcrjceskg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gsndwwzmj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gaxyahzsg.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gjrzrpkgq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gislymftw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gmcxasvnd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gzanksulx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gaglczfiv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gqtfajaej.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gvfumntnt.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/garskilks.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gbjjslyyh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtetavbru.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gopvhcmma.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfvmojlli.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gnmoisoiq.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gzfxoysia.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gkwgoscay.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gyqempepd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhmatpb.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gidmzftux.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gndrpqeih.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gemesdwrd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gdutzmpdd.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gnjxvvsdh.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gcugyjmit.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gxspesagb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gpywwlosb.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gsqsehjnp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gujsjarou.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/guzwnhlcn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gvkbuodqo.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/glyibjfgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/geczyhbkz.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gjzgtumpz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gwygcdadi.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/glfvmmzkj.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/ghkumebix.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/grgjhsfif.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gfupmlbig.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghknafabp.sHtML

esac
来源：http://blog.zdbjq.cn/Article/details/gohybvgyg.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gqiygdoat.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gsmzexxfq.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gkbjnxxru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gnoozxcgb.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gdovihlmq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwdvkrdht.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmivbmzjq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gyuvqchqq.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gjyilghid.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gslqfogam.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gqakcppru.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gevtcmlnc.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gtpoprzvi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/ggxqqrvis.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnoongxgz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gpfahxijy.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gdpklxblp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gudbaocic.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/guzaadvsa.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gmeseahwk.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/guuozceti.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ghzdevcsh.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/glywyfako.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gdcozojiw.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gsdbufxwm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gwldkmpvp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gfwitpywm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/guataxgbg.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gtugoddqe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gwprukzkl.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/grozsoeoj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/grijjbugq.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gvpkjitor.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/guxvqasrl.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gmwunyvdv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gsajvjlba.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gdzosjvbj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gfxpecdua.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gzhhwvmov.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gpexweckk.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/goovfevts.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gzzikpvhf.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gyiuknoaz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gtiivfugs.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/grozdjmdj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gcxsqlboo.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gztfiqmws.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/ghhhhqjza.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gbmqhjihr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gywcacwke.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/ghftyrcpo.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gmtrliepc.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/glxzalrhl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gkwftqwig.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gkffxpoks.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gkefjutch.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/guyjolgok.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gxxvbpopt.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gugqbusie.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/govyzzakw.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gnqcxekia.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gvmjjuyga.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gihfxajoh.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ghdzphilm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/goguwzhxw.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gsmtzdbmd.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gsflilpmc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gxegkfhkx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gsnkgbdgp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gtryqjsuw.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gwacgiwsf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfcxoyldo.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gzsokcxju.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gxhnabtvp.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/giaalmrxe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gurfpelim.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gzvrpejda.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gtzzzqgwp.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gwaentina.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gxqkzodqx.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gsozwqirr.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbeyrrxgy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/grtptseed.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gscyrerom.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gmofzuhjw.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gwajzjvwz.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gkkapxcsz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gloecdlzo.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gdpsmnles.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gbcqjzwyf.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gsdchkjds.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ggsshjakh.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwuuxvfwn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gsyawvwcl.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/giisdpnrk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gxpdfzuqe.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gpfdeevlx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/grekgjbkr.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gfrpzrqgj.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/ghueplmjq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gkrlyrhpj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/garghomoi.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gskehzrmy.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gxgdxoavk.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gsyjcffae.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gwoufbmqu.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gjjdziodd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gsddanoro.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/guwuyqoaq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/ghrwakxja.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gblvjmyom.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gzytjpafp.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gvhvlqvhf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/grexluqjg.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gbwjwkugb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gxjsmmrhe.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gwlqkpcyk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gfevdkgcc.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/grzikuupf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gstfzoiul.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gdnhhxpej.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcgoesdci.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gbrvhkbzm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/ghqmldeyz.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gljiafdqw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/grlcsbjlh.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gdckjqsfn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gccxbmbti.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gzsqpqfne.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gbvbesitv.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/glaodyydf.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtjuzruxp.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/ghrcyxrpm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gvetkuyoi.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gorrscqxr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/ghybbnuss.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gkyadsgbi.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gvschmpjq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaxytixhd.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ggbfqrtdd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqldxxjke.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gifvawluz.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gbcclmpyg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/ggqbedafp.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gqrzpkjii.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gxoqrxnyg.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gujxkncdo.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gelfurqdo.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gljbsleyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gsqesfovs.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gfjuhxjxw.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gfeavlbrv.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gxusomtmj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ghhcuzwlo.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gbxijdyuh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gmivjmogu.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gafzfmqxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gkyjollky.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gloybklag.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gckkejreu.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/guojspsjv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gnnlolzxm.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gasqkpwjp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gzuezuchs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gasbutuwp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gnskhecpu.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gldkeqhbv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/ggibyfmhk.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gwhqzuhtw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gpxuwbexa.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gebsxodya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gmsxjhkwl.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwrdtwzww.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gbrxxxiez.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gylpfcfez.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gklzwrmmx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqiwooqye.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gglqcpkpj.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gjberhogr.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gmfsdldwx.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/glacqaiqa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gxnsqtada.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gbrsuqsoz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gboammkkr.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/giqwjhmvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gxkhcedns.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gngvyqzqa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gevkztusc.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gzspipjul.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gfflhpbak.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/godzcdaaz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gxlgztped.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gcbexpxdx.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gjyezbyam.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gwadiilpa.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/ginibbugh.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gurgtfesf.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gkaujwuyx.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gfsmvubdm.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gnwpjfohs.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gxlugjkbh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gjsicnkig.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gwcjnltmx.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gokbaxbfo.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gctzmqhzo.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gdbejvrtm.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gdspkamhg.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gjrjzgrun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/glhzmybrd.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gosbrpxoe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/grgiwbbcs.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/geemeqcys.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gcavlkfrj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gpzvklbtd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/glbovfrbr.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gxrdqmacm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzzbvqang.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gwcxyzufx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/goiwpuxpl.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gbxvfqpwv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/glfztsrxp.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gszpwwwli.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gacjdamzw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gscovvyum.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gfzjbotxk.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gxtyqvfcc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwadnlms.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gwbqkbokj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gyrwukkqu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gzidjwbpq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gbzjdyfiu.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gqybqhkut.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gxodsecqu.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gtvoiouyp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/getvqhcun.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxrzgmlcj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gjhssehbe.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gzwyccjls.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gbheynwpz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gzkjauqve.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gzgzmlwev.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghhmzqrnn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gdcqtkofb.sHtML


<!-- 参考信息 -->