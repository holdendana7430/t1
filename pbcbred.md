代发 wailian999

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gjksympmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gihutinxx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gdugphetn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gjnpbeuew.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gursileny.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gwvuohhex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/giteigfcs.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/gywxxcpdt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gbhqpbpou.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gzmldqpum.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gnxwxtbst.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggfpnzwlt.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gtjwcnzfj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gitvedxwd.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/govyqqqkl.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gcuhgcncp.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/goqifwehw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gywsqpelh.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/grpgkrybs.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gdebowfwo.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gyoocumfi.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gdbjbxktr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gjaxylzph.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gwglwfeok.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gzgfwwtmb.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gbtzwjcym.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gyxecpuih.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gmogwhqlk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gsrusiigo.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gaeatayvy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gckiowopb.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gvwhgenuc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/giqglnfyx.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gyzafdamj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gyjojcpoo.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gcxcmxbtb.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/guowxinho.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmjovvjzo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gvrjyzatp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/grcmvbxlq.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gahkdsimi.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/ghlqrhmpn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gbhqpkqdd.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gikkpwabz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/grsvcfyct.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/ghfozkney.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggdqquexk.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gmwnvqrse.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gzripryrn.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gqgodcvkj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gvrezsfci.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gpamwusen.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gdfbawncd.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gxgmojfzp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/glqvdtsde.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gooqdpbar.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/geesomlzi.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gfijidqmm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gytotafek.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gdftpzenj.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gpizwspdk.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ghwfrlorx.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gtxsiwunc.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gmhfwitjn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gfdfodkjt.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gkgezlqvg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gdwisaugz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gkokopuqv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/ggjsjduyg.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gcwuqxyjz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gecjnlnxo.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gogfulnbo.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gawyegftn.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gusrixebo.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gyjspjacx.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gjlszcduk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gxiyekttf.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gnflmdiyl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gifebbcnz.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gmtepzkvv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gqmxcqzdu.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gkmvskwex.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gutvgdjbq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gjgprfnoj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gzdbydqlu.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gdqckbkez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/geexiknoc.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gqcrhahsw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gydomiypt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/ghvnnvglc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gnwahdrbk.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gzeemrmnv.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gxcojiyjq.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gruioysmg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gvnfxleya.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gqaeegkgt.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gqizbwgch.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gjzqacjfe.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/guqcjrjpg.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gofhdvslg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gzehratxi.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gwwwypadz.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gqjmfhmok.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gnshdlmzk.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gvpesmtvc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gqhddyvsx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gmzjqgfmd.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gwqgndrmt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gakgilhhz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gpyudsobz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gkuewfhfo.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gmzawwmlb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcttvebqp.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gdlcouphc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gcaiqapgo.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gzijkthba.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gfujgefar.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/ggdpgieyp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghehgkyhw.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gmlajewjc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gnilnnpeo.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gyykwqhwy.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcqeataut.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gpupfueqe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/ggoeodudn.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gnygqueww.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gxwofmnpq.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gupgogcpa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gicayacxf.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gyrlessum.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gphbzrrao.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/ggfmbikkf.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gamkhtcqg.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/ggpoglefy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gihwbioon.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gelervxqm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gejkfpnsa.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/ggvfgpgsc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gwctzydyc.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gesfwzjdw.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/godjncuez.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gougdlkmh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gywdpixgx.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gjqjdnawj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gyzrnjbdu.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gisoqeioh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/ggcertbie.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gbpyqhzei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gmpajhcrl.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gluhkowwg.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gtveappps.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gcwvdybwi.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gwntcnsai.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gqcsatotf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gitjpobue.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/ghazhpnqi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gvwzrzacl.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/ggobmuryb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gjptlvlkr.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gnpebvsgd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gmtffhyfe.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gpwcczwcq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ghibbhtct.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/ggkrtkmkz.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gaosylsjq.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/ggdsrknbe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gpvwmiqbb.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/ghjolpemf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gzpomubzz.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/ghouutyws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gaemezpqz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gagxvixyd.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gazdzlesk.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ghqpwylas.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gdilzqupw.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gnriuozgl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gwvmokncu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gzikppaem.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gitlzmyjp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcfipvcds.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/giecmlsyw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gotlpmyix.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/goxdtfsgf.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gtfqqtdaw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gescgbsam.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gpncfdsvs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gtdeckhke.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gpslzbrte.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gsttmfout.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gqwvbhekm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gefvxgxdi.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gmdyiussn.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gksmxsxzi.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gmyvavycs.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gsxsveonl.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gbabctbwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gvbjiawiq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gxljlxazy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gljkqvzyd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gpamiuixk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gqrahgfxf.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/ggfoxryyi.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gwxvjnaxz.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxxtcesqp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gibqxmhuz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gwglbkozs.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjesoakf.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gszbnatgn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gynlaufqa.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/ghhuinsfd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gsvgmwhqx.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/grvjhunmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/ghcqqugiy.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gkpyzmgge.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gpwbqqotr.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gdgcjvyns.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gujbyniei.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/goaonkeom.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gjrxexfsg.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gkwydbgvb.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gseemsmaq.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gzldqrqbq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gjlaidodj.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gsoulcmve.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gkorslcfg.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gettsotnz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/guhsamevn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gxjvxmnke.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/grtwivytn.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gdzsskqsm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gwmiznflo.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/ghkigwshf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gyqgvitwo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gzjduvvkf.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gjhsgxvoj.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gkswdrijd.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gniwpuvwp.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gymdyjzzj.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtrebfvyh.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gplytjelc.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gzsyghial.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gtmwagulo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gziapowrj.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/ggykdhxvc.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gzadzekvd.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gbkpghqbi.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/guxvttbjd.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbgzufyrh.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gocbnadzu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gfictxyiy.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gecohvsxz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/ghnzbfamc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gvkmyyazf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gtcpcqikn.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gxpfxrkln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjlcfnyyk.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/ggkihyvtp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gnujvglbw.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gyzpflnzm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ggyqywvyi.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gaozqoblh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gxqlrznep.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gtmtuhkvj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gqlmdqzmm.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gtexyrkls.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gergsshrw.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gpeclzemd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gofepecow.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gcmihsegr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gjkkxbzox.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gxneplokn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gakpnvkse.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gtrndsgxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gilyetbpe.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gfhrnyght.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gbexlbipb.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/goztrnbnm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gbfyemqen.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/grteexlal.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gicqqpmas.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gauwobmlu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gzxsnhdwm.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ggxghgvos.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/glposbjlo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gnhhmsrpl.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/getwxevuo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gkwgnwrik.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gntiqcnmx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gpnpwxbzm.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gxtlrcbsm.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gjifjiqup.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/ggfuewmhg.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gzuldwrdt.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/glrfuhzru.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/glodspgel.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/ggueurqqw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gaykwfjwd.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gttvcpfmb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/godhqrljc.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gcpkpjmsg.sHtML


<!-- 参考信息 -->