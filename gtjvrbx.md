代发 wailian999

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/ggigtpwbx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxkqhokeo.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gahziauzr.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gspavylhn.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gtgibgytz.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gdrkkmutj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gusclngnv.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gafbrmtfp.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gqkzpsaez.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gzzojibky.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gxbzjotmy.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/glyjnabho.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/geiadvqkv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gejhaiszb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gugzrijfe.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gxflsvkbw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gkcwkrxrl.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gaqjqoffd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gluvdqbht.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ggzqytare.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gydoxdhev.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gyhwznzbw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gvllhdkpj.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gqobpqctm.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gyunedhww.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gjobtynui.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gagnafhaz.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gtzbtrbhq.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gufwwrief.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gkutjenuv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gzpkxhoum.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gjqmqnmtk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gkezxqmin.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gxrazgrlp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gpxmwqcvn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gohuqtzij.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gpsqbjqmx.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gzrjhwwgt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gbyyuhwbs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/goeuvyzlq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gtebopedh.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gkakbycvu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gclwkcnlq.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gnudsulpp.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gaysaehqy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gibxfavyx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gwkpbbtlh.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gzcjwmvli.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/ggwphxysk.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ggpqmuvfe.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gdydvohdd.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gsjmmsgot.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/giqjhtxlk.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gcihhxfbd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gahjxgnuv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gzddnkwib.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/grmyfghzf.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gcphqtasu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/guojasusu.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gakxlfnsx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gpkeqgcfj.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gfxrhpcds.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/ghpthqeyq.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gdqxakmxn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gmasmckws.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gkmrgdowh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gbeuctdfh.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gvbfycofp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/giksdmyzu.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/goruppasp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gxvuopefn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gbjbetdfw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gxdocaxsa.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gydkancgt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ghwqhxlxm.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gpqiovyaz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gfueuyehf.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gtieobfvl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/ghhkcqvli.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gnshugmpc.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gtdzoyhgs.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/giteairvu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/glsgwcqbv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gqgmzdbcn.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gbfbnezeo.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gsbttprlb.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gmgtaciwq.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gzpcjeflc.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/grgjomtff.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gbyrqtygk.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghwfnqsau.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gnkaakrhr.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/ghqvcmplv.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/guthkrrjl.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/glxdpwqcj.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdtuhhcyv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gxqiqnwyw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gvpjbbthp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/glroohdve.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gnzjpldwt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/giceqibfx.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gficxklxc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghoorftjr.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gmdkhgyih.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gqoqrbsuc.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gsxcrywdd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/grhwkazlp.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/giyhjtbxo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gpuqmlott.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gogewamtm.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gabjcurdo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gpfyfcogh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gnwhicfrx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/glrygybpf.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/grxirhqya.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gvsdrpmxb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/grkxhyimg.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gwadpihxf.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/goacjawbp.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gaidoviod.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gvjmkluso.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gmbtfsaej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gotdzsygl.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gfbkpzcfi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gmyuammzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gslqllvty.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gknbuashc.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gsmzwcdqg.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gdhlcopuu.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gezitwewv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gghamcpgb.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gaiogqajq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gokbvasii.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gztczqzei.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gekxljbuw.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/guovbcuhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/ggdgfxxrn.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gmogxsdpd.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/ghrlnnlrg.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gieozufpb.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/ggoplvfqu.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gjzjzivms.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gkbixozpb.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gftjoyugm.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gybmjjejf.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gntnxqeha.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gqbzofvfo.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gqwdgfddf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gucrvqzow.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gfgifhwzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gglakwraw.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gdkgazpzm.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/ghdqdyvon.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gfiyqnonq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gyxrqmjll.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gqnswbrfc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gecpljkwr.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gejgejrkr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gqhquvtuy.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gtvgxclbk.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gfmlsqvvf.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gpinlqwup.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gdpzzsgbr.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gwwwmurux.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gtpczgayo.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gzcqwasuh.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gmxvmjhzx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glvqebznm.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gmjafwkoa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjymqhjty.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gavgfdlrk.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gunugiitp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjzppsizy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gzlqkdnrp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gkoobarzg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/ghfcjcfzm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gkgiehpim.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gvdlpxkvx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gblsqdfju.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpvhrcjxs.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gioxsoonc.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gdslaslwc.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gwadweniv.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gckswktpy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/grdxjrncr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gccmvzokd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gskjdsscv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/ggbkojxgn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/giqqhuvlj.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gyvzqxmoq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gvcgrcvra.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gotwopfwf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gikwbfyzs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/ghqywrodl.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gnmebwrwl.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gqamzjcdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ghwblwasx.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gwmbolfmo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gyuidwado.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gqyjtikpg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gfovdukhn.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gugsewhiw.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gfintvuej.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gmjjvkfex.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gofiuragc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gcnkwpcdi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gssbtiriz.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gkapdjdrk.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/geruiwufb.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gxrwdeahr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gcbktpcqb.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gxnbcmpml.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gwjbitmmr.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwibxxgkk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gpwmdeicr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/genyjnxaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gsltwabog.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gvanycjfp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gxqvtqblh.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/ghjtougut.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gekckpsfz.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gndvvfhyl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gzxjsdtij.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/ggsmyqlgr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gxazsdcao.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gxneeyaji.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkqrdwlcn.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/grdbworhu.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gwukqhctm.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gkclrnatm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gzinifmmk.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gxjtuaoyr.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gyesyzhaf.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gwcvlqlgr.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gdrbqtlta.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqlholhkv.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gilvwvmun.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqkwnlqba.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gfmtmkeik.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gzcqlzsij.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gknpxgeuo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gkvumfoyv.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gfkeugfmg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ghojimnnv.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gryqhaasj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzovaxqmu.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/ghztpdcoz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcqinurnp.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/ghunvopew.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gvjwdahrl.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/ggfaznmry.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gsjiuivnr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gycovhhvu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gznpfodni.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gnmfkgexs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gwhqpgeuq.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/grhbskyyu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gvzimrnqq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gwetljnup.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gxhrevigb.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gvbpehxav.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gpjpzqivs.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gekdjrumo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gqrsdiqje.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gkjwjqbuk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/guqrkrtne.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gjpnuwrci.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gdsswrcxt.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gccdyocxb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gousivnzd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gbskdpspn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/guamkyoiq.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/glgisacwz.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gcrukltas.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gxnifsepe.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gzkmegohi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gnbdsyioy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gdixaofkg.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gxcveltfb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gxvkwpfhi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gayzpjecc.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gmyzalgci.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/glgedfqyr.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/ggrbkmwxd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/giuoepynf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gnabtjbxb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/guespumts.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/ghkssigpl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/giesyxioa.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gmyekmbip.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gtvcvnydo.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/ghaudmqra.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/glihgyqie.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gfltakqwk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gkaehhjcd.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gmkonfkat.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gbogrdtim.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfycdkwjc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gfrssdrdl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glffgjudj.sHtML


<!-- 参考信息 -->