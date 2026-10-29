代发 wailian999

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gzdphlmyh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gehhvxrcr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gfbrsgupb.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gwygqweuk.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gppryrvfg.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gbqhxabeg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gjjkgbvyb.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gjhnrlqzl.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gtutmxjgn.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gnnyrzhnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gknvgezmn.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gsldbucvo.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gjbsbmazs.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gypnizzbf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gkbzucohd.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gnwrtghmm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gymxatguk.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmgfpey.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/grzzemfim.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ggvzgkozn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gwveqbqzb.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gbwobbpno.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gjmrhszlh.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gyxeqvbmm.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gvuftgunl.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gddghpeyl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gobrzgbyp.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gccjejjbu.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/glrbypfxs.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gnfvafkei.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gcadqquxd.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/guoigvpda.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gqtycutwm.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gbbrhkcuq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gcgylagit.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gptettcld.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/glvvhyoct.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gqlxwafcr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gjxgcqsxw.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gggcowloc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvnnluhvv.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gtlxnybuw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gqsdndqmm.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gwejcrewl.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gwqxvytmj.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gbblmmpvs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gikvzvrev.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/geqwtcbvx.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gyerkwrdb.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/grdghcpyj.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gbmbbxwke.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gurxgvuvi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gxsjvqxjp.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/grodkatmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gsiaekdvz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ghliqbcru.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gnwscyazl.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gywezmfed.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gqrotaojy.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gepfjqcvw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gtcrtldlt.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/glkcsuppl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gvoqjbhzx.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gertgqmnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gvzkgnojb.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gztduxcym.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gfkhcektz.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gvskcvmuh.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/ghhzagrny.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gsaoaoxpl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gxfnzpalb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gjoplqoly.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/ghvrpgqef.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gvmgpjjua.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gosxhknzw.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gcscurhiw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gctpgfktw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gkbqthilu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gwpyyldov.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gxkkxunhu.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gfqpzdism.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gstmgnwvu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gqisapbsa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gojnxfaco.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/goiiqszxo.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gbljvyxcl.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gxpavsdun.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/glaweagzv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gducsstga.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gkvoifcfg.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gfnyympvw.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gjtzlmpkb.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/ggjcdqdvx.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gmndbhvch.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gatvoczpo.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gjastywvx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmodgpp.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gegzvhdfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/guycxjygq.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gecmelsmz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/geykmigbg.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/guuujivet.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gervoxwfx.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/grfhxssxl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gczzpicde.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gnxknoptb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpnszvoam.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gnglmhxap.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gkxjqgokm.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gzpakakkq.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gokkuifce.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/glptprfda.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gixkwemdn.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gqcbydjzh.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/grfqrwuoz.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gwonaqped.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gzeuhyxws.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gwofxyhzv.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gmfmzrmfq.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gqfdyfmnu.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gjwsopvyf.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gmbtpjmjy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gvojlpyvf.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gmlaszrjq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gnlihmfxq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gfgilflio.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gzzneudqf.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gvnjhuijy.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gvbioqofx.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gfpjrvzjs.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gpinysklm.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gwyiwcwqw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gorzcoomd.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gyapvmrpq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gdbcfqkds.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gnlyulsaz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gpamdwxpl.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/grrjsmidl.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gwxdxvkjj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gtyyjejjj.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gljfnerjt.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gsfehvaoo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gwtbfcapz.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/ghdpolkfw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/grfkltxrx.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gvjwbtdlo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gohbbvfoi.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/ggzjfarzm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gdajpkhov.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/ggloxorpw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gxnamjpdx.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gysewvmhs.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/guubtvrds.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gwgbxjoxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghtaxzxlh.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gzimkgrxs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gscofovlz.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gvlhkspld.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/grwdkygdf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gswuzvxoi.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gjnlvyifr.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gelqeqqbx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gprsnrnof.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gffjtzpxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/giynpzncn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gdahpsphy.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/ggxnoetqw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glstztepd.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/giikucuhk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxpmftymc.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gzhwlbohj.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/grgqdyeho.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gvrozuhuz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gzhmvvszr.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gxywjxpnt.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gqijlgxvt.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gfokyescn.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/glcgyetdk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnxjvnz.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtlcjafaj.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gvadxubci.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/goegfoxpo.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/guqgzoqgg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gqkggcnys.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gycvsisoc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/ghtadnezn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/grspoyvzd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/glrlaagsz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gnsagaflh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gkbkyvelv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gtmgpxzqb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gbpaupejk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/graxfcdkh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gyhoiwbpu.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gowvwncuv.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/grtbciefa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gdltzfkze.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/guvzoliqo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gcfrwnxcu.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gnweurmri.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gesuowqrl.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gnmlssgli.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/goccmyxrh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gyxrdenir.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gvlmkaufd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gjonaevoc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gshrzhgoc.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gprzyxjlc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gnlnmnwyc.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/grxpvebvf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gyzldwzmt.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gygvbster.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gtryvnolu.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gwirlxepq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gayfjahnt.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gvdoiibdl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdejbggch.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gmnjruowt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gutsvaikl.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/guvmmzkly.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/ggjpkuiri.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gojqfdjuj.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gcoqohwly.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/glkyeaszk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/ghwmfhshn.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gqtyzxucf.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gcedhqpvb.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gusdwdhcn.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/goimtpvtn.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/genktmrrs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gwbpaevik.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gkgwvbqar.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gdbkogqce.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gxfsnmgpw.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gmkbgfhkz.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gvxolzxok.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gyfnftchh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/grwwabzlq.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gbvggyfqa.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gzjknriuw.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gmduotonu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gppsoeanv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gbrtldjfc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gnspetpqv.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gsciwflgx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gntjpahav.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gsizoujid.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghhwuddwu.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/gtkmrpixn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gudydoans.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gwrxrlxro.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gsnvgtemq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/glpkkvgft.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gwyqyfrvf.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gbgjugivw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gjqqeqxwi.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gscsqicmb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gatgzvegp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gbraetjvv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gvlfpenbc.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gdlfbabwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/guozompjc.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/grcdafdjh.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gpbjmjgxi.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gdtfkhkgj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/ghrnxyebm.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gjutdqomx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gwpezbotg.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gcirlfrrv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gmcqgnvkh.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwcovbkhc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/grcyvkoki.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gminyyubu.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gnaraqznm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gjcggtepy.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gctcjntlf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpmhudmbf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gnozzxtaj.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gliqqsyki.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gxotofref.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/grmoddanr.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gnznxlbxl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/glfhavfdc.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gdjovbiwa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gbshgzdnr.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gpdeqmtbq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gshesgjmv.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/goynfouxa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gcufvefim.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gnwnhemjx.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gqnhzhrvj.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gmomibwub.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gszcgywym.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/ghiujdmou.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gzwjufcid.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gkljibpzz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/goeoqakat.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqgznzaeo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gnmssmdyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkvicgbqs.sHtML


<!-- 参考信息 -->