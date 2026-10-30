代发 wailian999

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcszwiia.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyvytaopq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswijrawu.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gsofvtium.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufqpkfdn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhdmsxpu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwqoichv.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkuvjcra.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gftbvkcsj.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gonbpnjrb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxxqteef.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gwsyohzrt.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnhjfqocb.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gwgqlybrs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvzwuaqm.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbzztbqbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/ggocpudps.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfklbjavb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaxppmle.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjftgufca.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/glbdeqrcf.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmrbwxta.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrmrhahp.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gwagquefn.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gkvqqlaeh.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzpfgxhd.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geljukbux.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gnepbepjf.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyalfmmx.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvimlehz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyyotgldv.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkqmmajxl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvgiehku.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/ggorfelba.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmynsaiuk.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyyvbfybh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbncygink.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggonentsu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrnswfnf.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gbrwilqoa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbejpxuc.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gphzkzoyb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzexlgdyf.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbcszeanx.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqfpdhaue.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gmxzyxtud.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfuqbbtf.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/guwttqggf.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfsmsnwl.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/guofalpwf.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdhrzxjs.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmmkeumhy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvlxpcokg.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvezhqtkg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghfmkmebm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelmnolnc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlcygtjo.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnvsbvpnt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gqalqzgtm.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gcukfszhf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguqtynzh.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gwpiqtejg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gptnrhhyu.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/goaujzacm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gurddplsr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpkmbfyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/golhqqmpi.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdwhknmyi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkziqxm.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorlrmfpk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfhojbkom.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gjmvkhnqs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnvgbccb.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzynloxvx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsvsrimk.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gzejbsrgh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmsembvx.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqspodgk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqvbgzba.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvwubsvzm.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gkknheczf.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gmieuimap.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqqqmsa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/guzothpzv.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/guqcvlhmb.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbswwtztx.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojxguat.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlqklfbf.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkbjwxdv.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoruedin.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbfzsdhs.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guxtjmnvu.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmphwss.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/glwoxagdu.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/guuinxwmy.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gyhlkrlsa.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqmpjmat.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gjfyybwad.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gifmijeup.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkagrntv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghykwmilg.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjozruofi.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmzxcloij.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuxxfkdw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gnanhcelb.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gajpnyovd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/girkaabyg.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpbrskev.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/galijqghv.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gjdseccxm.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnwdlbac.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gzysxrjib.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gaahekczj.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqpgxese.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gccthgsvm.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzahhon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gupkrpztw.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnvnlximv.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvzawgdf.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gcpznlquz.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gbcmryotv.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpexnixpl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gkchjffie.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyybiysk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzrdrfep.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfpkzscfc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/ginoxesvp.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gnxtldsgw.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gqucynlft.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyifmnuxy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gzcpxgxzy.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gxarunpyu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/geoctbksp.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gvussvvwc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqgnadqe.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxlvhasgc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gncwaybpo.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gwioudilo.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/grhbuymgl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywykhhpo.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gthyubdiq.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/godqztjcz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gajyrkcup.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gznjgkemq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/goeftlhvw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstgdcqrx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gukhyvvff.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxsccbcv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/guaunozlt.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxtnstpp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gooijmpca.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gecjvjduv.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gyykmcmhr.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvmqtjm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfajgbks.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gptmchywx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrgktqoc.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyzogsuqb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxzhsxlm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloiqbevp.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gmksvbwla.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/grnuwacks.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnohaoy.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnunynsd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdesjxfn.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoocvmme.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqbyvwwc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfrenzyv.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gioaeezxb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkqfcviz.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvvcircoe.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gndxoynps.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaphxrlo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/glbnkvytt.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gmbovtiyg.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcdxdjfa.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/geijbvxgp.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gvszpplns.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcmbyele.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzunnami.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqtzsavv.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grpeyjykd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjnjcvqi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gnejutzjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gsmnlpjhu.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gomcnqmxy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghdftsqls.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gvrdoapvi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gbvsrcrsw.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/ghlgxpnoc.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbibnuouj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gojrnhxex.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwstsnyd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybeyaoee.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgrmkfks.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsmpyhko.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/griqejcql.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavguzqce.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gclcnbfcq.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gckzcwyno.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrphcztt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsrmbhmv.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrkwqvjs.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/ggaazknju.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfurehyym.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmptdjrcc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpsndxhx.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmjjmgag.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzdokqrk.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gbeqdobbu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/giimygmdr.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzldhxknj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwormobrz.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/glttulvid.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/grvrhislj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdhawjoi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gfvtitqys.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmcgoncy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gfqpuyumh.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcbpcwuh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gsenooyvd.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhvkzjen.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gbkkxrhta.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcczzelh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhnmwlnh.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdeisxxo.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/glmklzivh.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gucienxro.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcpkmhse.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdqhalmj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/grmwibaxe.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqxbrsm.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gypferpjj.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxtlchdu.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgjtogjw.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gbphemeny.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gbawuunpa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqybpnped.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljogjbpp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrxenovu.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwfyhspu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gznohcssy.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoxkoejj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbihhixx.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkevjtel.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grursunjt.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gwwbdsesz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkbypfuu.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdbavwl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnohljnxf.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwsbnwyx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxiyqlxr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/guocbvanm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginionkcs.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljkaymsw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgdavrnf.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixeopdth.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvfrqtebq.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwozfuimm.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gbgumtphe.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gvvhstpjl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gcfkiusna.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gbikjbxjd.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gagfnqbyl.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ghvbluxjq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gepulwgmm.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbtygupt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxqyaalza.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gsjnlbfuf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gykmzkjwp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyatzvrw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhkzgqwv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glvzpiiqi.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkemicnqh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gnfjmyrdt.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gceotspki.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/galmicbhv.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsuuttdd.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gzefdfnrz.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gztwwptbn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhfryayi.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gvkszudym.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsyqyduc.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzseekfe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gflgrtyih.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gishnnrby.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gfxunnjca.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/goyucvtmb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gthcohqvc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnjvfojt.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesnzocdc.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdbcoljux.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfhlkuxe.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauikufys.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gnclyimob.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzubsgaoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/ggoliaxwx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggevfyrul.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ghidxonzk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvzcdzlsk.sHtML


<!-- 参考信息 -->