代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gtpftqlhy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/geouijpcy.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gtivnfeqn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gmolonwza.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/ghpsprdde.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gxppiysvu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gdhgtslgj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gthvaroke.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gdxpvcnre.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gebzwlgbx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gfxkaxykj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guqkzpepn.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/ganlefydh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gstykaeih.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gemkhlwth.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gfjszomsi.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gfoinutwq.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gerqsuifg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/guwzohtas.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gydiwybwn.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/goultvfcd.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gvnetdldi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gdeuczlza.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gksyhcskw.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/glltvkkpn.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gizugcpnb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnfwyjzjb.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gwhgfizpi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/glujfxngl.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gerdahipr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/ghobarjwk.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gxiaczqgl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbyijaalc.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gsohttkeu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcaxzzukt.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gxuypalrm.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gyyswmrrl.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gyhkqcndn.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/geklgsyii.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gbrxohwif.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gwntuudah.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gnsdkwblp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/genthpvis.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gcxkfxhbw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grwlkbryv.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gdyeqejpv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gjjhdpjld.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwfezpdzr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ginebzipa.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gxpbozicd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gixivilgx.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gpwlndtbt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/ggreujbun.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gsltqpprl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gizvorbdq.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gyughipue.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/glrnovurs.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gaqctupvo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gyplzckaa.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbsppfgyb.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/glrozamtl.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gligbuvnk.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gclfibswm.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gxoaxceis.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gzxbgffix.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyxbgrfzo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gyxldxzkx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gyjfvmlxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gifnaxfxw.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gdocryubl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gcnatyfqj.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/ghvykypfl.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gvfabcmrb.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gwnvsdtik.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gfuxfyroz.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gvthezruj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gvhbmkfje.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/grtlkibgw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gjxevivaa.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gqoyscrnp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gzglwzzjt.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/guyseeszm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gpphahpwm.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gjzctqjhw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gudtiiwsa.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gqglcwtim.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gdtcoqovf.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gfgrpzclz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gmxjimvcy.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gassfivze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gkeopqkky.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gzzyfdbol.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gjkijjrys.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gwveheeqb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gwlclblgj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gjgqttxjn.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gmyhezqbb.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gflxwbiwv.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/ghnzyyxxf.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gonzthaaw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gajkjfkvq.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gyvtfzcfa.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gtcykotnv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gaaazqqac.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/grhsfqtde.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gkruypzgn.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gyavmirkl.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gewcekxij.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gxlsfvwat.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/ghiufgzdk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gisawzcpq.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gkjogubdt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwrthmzkt.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gyicuqdds.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/giinpcvmw.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/grtgqylib.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gubwhxwoj.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gbbxiovos.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqborpifp.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/ggajrukqp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gefetmayn.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gocckggkq.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gojerbrgt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/giqhvmzur.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gdwaxiqqb.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/galfzhads.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gqfrqbznq.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gtttjuscn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gaqijhsjc.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gcdrxqtfr.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gmcuhaxfh.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/grlzzgacy.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gsbynstdr.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gzflaldbp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gglkotrvk.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gccdmsyvq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/giyzxwhlu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gikazzukc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gaidrduhd.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gswgxmpyl.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/ggknkttnu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gvrwsiqyi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gzljacjmu.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/grxvtyloa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gieowcgwm.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gllfndely.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/glhgyewhf.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gjcdwilvf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gruubrgev.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/ggtjzqvzi.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gcmnjbhun.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gzxmdkoqy.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gzzrosypk.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/goigosapw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gdbchktpt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gmyyohoms.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gtabfzlpj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gzczndzim.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/geapkwayt.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gcvdlznbl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gzjosybka.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gjvcwzkbw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gwsauvhaf.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gntomyraq.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gyojauncu.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gzqeamzba.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gltwlfqhx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gxuoaxcdf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gzzmkldxv.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gewfkrryd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gulbmoauc.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/ggmgzyfeo.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gmlndtffd.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gejvfvgrv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gywlklznm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gzeqikxdg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gvjsxofsl.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gpazzytft.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gxzxyqcjj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsxvifqog.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/ghhpvhofy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwwdowhxd.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gbesyoupa.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gtxwmioxw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gnfgddxbe.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/ggeliaqos.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gjzynedpz.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gkkuocubq.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtllmhlq.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gasjncbrz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gyytmgtod.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/geowotobe.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gahkpijyx.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gvkbohwkr.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gnvytmjlo.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gchyzdrks.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/ghuhgcglt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gjmlzewsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gkujsamiy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gauslehkx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/godnphhsz.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gicdokuwg.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gjqvumvow.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwhpzikvb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gndfcemyo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gotqtvclu.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gudltotue.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcrdgsoap.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/glrmnetyr.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbmbdsz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gpdmwiige.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gmgpemenv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gyjxetkqa.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gmymmgxhx.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gpnhdtpxy.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gpkehqysz.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gjluhlxlr.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gbxugynix.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/goxutpcry.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gatasgzvv.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gdptnkglg.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gctvsfgei.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gsekvzids.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gfmjqwccz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/giyxnuuko.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gntoshedz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gestwwuna.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gzsflxmmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gockkblst.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gxazreegs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gzbolziyr.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gmwghwlka.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gxhndddtd.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gcjrrrdwh.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gofanhwql.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/geduabkno.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gucyegasz.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/guzdceime.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ganhbiwak.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gfkqldpvg.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gdwwgjphp.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gkvcuhppu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gwcgxvrcm.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gwivpdaug.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gdbqcwqfw.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gzzphbndd.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/goqekszrc.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grbuuisvk.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/goxiwiiyk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gzjvomasb.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gkfjjydwk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gsztetjic.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gzzrefgwx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gisbesphd.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gangxjhfw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gzktcefsx.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gdcrbaljb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/getzgyotv.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gihraqtfc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gusxlkjyk.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gtvijwfum.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gzhzsobnr.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gwaxdtaqt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkhjstuls.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/grmngqlul.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gqqlaqymo.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gcbrxxrnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gejjeunfi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghbxxdjcu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gekcjsctr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/ggrpfhuvl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gvptpeode.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gvplslvic.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gwurvxknh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gdhrvrjfg.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gtrxviqar.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gcmoidstu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gvuuyxpxj.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/ghaajfemi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gezlccvao.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gwheeduwv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gzgatbpjo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfpvrmdej.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gmhquqvaq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gjvknfjxs.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gkzsjzkvj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/guskkswih.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gjinvvlwi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gobriusjw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gvwnoyjiu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gmkaerqpr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gqqretmcb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gaqmkngxr.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/ggjsrtzye.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gqnycjamr.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gntydocqr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gwtukprci.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gureqqldu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gidbzbjry.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/guqoqvuvz.sHtML


<!-- 参考信息 -->