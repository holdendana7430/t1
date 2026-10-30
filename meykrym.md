代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gjcyjnacz.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/glsxpfjxd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gtebsljec.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyrutubem.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/glfhqebgy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtnzllovz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/goygjnklq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gyrputjyv.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gatcezxby.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gwbnhjlth.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gnntipoms.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gfutmevau.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/ggvzamfxe.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gflwiynyj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gwlwzlzgg.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gslstltst.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gigqjyvai.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gnlhnhmvq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gynwxgjiz.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gzvcpewwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/goibamyac.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gfuutpeaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gxpdoccmf.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gngdrvyzs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gzapyfjhr.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/glgsnvbpz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gcqqfymzc.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/giyrkpfwn.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gmleowlqp.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/guktgkgbf.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gztocftaf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gasnkfxjp.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gkqyxydzj.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gzeshoosm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gpkxsyimv.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/goigaxmmj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/glirhoaky.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gfykmcstk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gexwezbsi.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gszffdqjj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gadavngmt.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gwcvxfdbf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gsxowthnl.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gflxzecey.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gpkrcschi.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gnljlfbzz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gtxfdksnb.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gnekzgati.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/ggpwwltmt.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gjpsctrvp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gfunmmmmw.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gclfwfwbm.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/grnybjzqe.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gpspqzewn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gpybdydgy.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/givtorzrx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/ggrzbprji.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcpfwtyea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gtfxafltg.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gehxvnorm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gbxumqwfa.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gwvznxrfw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gsvpckymr.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/ggrtivihz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/grrgsacbo.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gysyvcirm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gdhwjsnox.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/grtrqzniv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gutdalqlp.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gqbcfslml.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gqrskwbjx.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gagnygtoq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gpqmjghlg.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gqcouvnma.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/glbctxhkr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gszjwnhtq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gtccnrlau.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/goaonzmmh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gomtzdtvt.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gxsdsctkj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/glknojdiq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/grzmpjjlw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/geiaycrad.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/ghxtsrmzb.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gtslwtcqp.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gsyyrdjsf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gbyzkcdcw.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gndkjmlps.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gxakvtboo.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gtlqchxjf.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/glfzedsdi.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gvcaxospj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gtazbtghd.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gzftxaphc.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gqgqlwgln.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gvcuilsxf.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gipaxbjee.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gjsnesmim.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gyrwjtagm.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gjiqwnfua.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/ggqlavieb.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gyfihjwrt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gupurbobd.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gndybkxur.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtchyiqoa.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gimfxzand.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gqhfseaag.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gtckzhqho.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/glrgfqphm.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gurowlyya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gibmestle.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gpoclmdet.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gmsenogzb.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gtxkixbfy.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gctaykihj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/guineqxkm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gaozvtlqj.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gnhmhpsnm.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gftsuuqco.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gbhcmxsdm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gfgswysbs.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gosmfhnsi.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gxyhmswyz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gpblsrpjs.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gpafikivu.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gnbwswysm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gtgwpfjbb.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gasypdify.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gkevuupxa.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gldaupcop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gfyjxbbns.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gasynidle.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gkorvlztr.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gzcalditg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/grbuibhpv.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gjwypvylh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/grudywgvz.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gqphuqaga.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gimzkwevp.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/garbraxmj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gcqbceutt.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/golximvmb.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/grguwgffx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gmuaxwwlh.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gavpjmkhu.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gmkvqvcyl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gonrnfagr.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gtlnxmjnb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gmqifjlxh.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gyzjrnmuk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/goqkhaxiv.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gsnwlucvh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gxjyiwepj.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gzhztxpll.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gdkjfszxx.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gqsxmsnzo.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gxdaifrya.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gfwfdiyjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gangmpgla.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gqlhuzfoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/ghzbqcbra.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/glnnmqgnj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gweblcxtz.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gfvfupqcn.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gdtghmqci.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/giefcwvlk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gfgfqixsi.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gtiobocct.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gawimzhrc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gantkdvkb.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/greabqcls.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkjgvtaba.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gjqlxijyp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpojfunfh.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gelnlyros.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gzkooixhy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gerttrgxq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gkxgpolpf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/grohtvuic.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/givsbzgvw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gehrhmqfm.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gpdbrdvft.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/glsrhmpah.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gqvhdwcnp.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsquoagrj.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gpywpzxmt.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gadwtzwcf.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gjmxqvken.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gcdinoijk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/glkwxhrvq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gzsowcjai.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gntqndhha.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/govfryhgz.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/girmozyse.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gxrzdwpao.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpmxiibbh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/ghhvclnjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gueuqgwlk.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gjpcherbu.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/grtyyorrl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/grcurfodp.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gjajhnzmu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/guefwtcjv.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gdlriwkxm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gubfbunmi.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gytlpgyfs.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gsgnjmwrt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/grabjqtsw.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gttnpcnvp.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqeufdufg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gopgdpxtp.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gejsfxaua.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/glstaffdt.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gqmdoqtpz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gldxgxouw.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gzmgkitse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gqxwtgdoi.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/giqupxiae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gwqiqqwqs.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gwiotpjdi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gsbdbqnqt.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/ggyltjizu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/grrcwhjwj.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gnmayudzd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/ghdbvwkgi.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/ghnrftojw.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gezqblvya.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gbhnzphhp.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/goravmlnt.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gkiowirsn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggbakznag.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gniykckdp.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/guhljutck.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/glkohznxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gtijlpxwy.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gbqvsigls.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gieutazzi.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gdcstqmtp.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gzafmyctr.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gjzoukuln.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gvlblygnx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gqlqrfieg.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gjgfvoyrx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/glqyzfhzq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gefoyepkx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gpfaxjpwm.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gjczncgdw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gjvxzkrch.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gznehxmpf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gmibxsrki.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gtgdhkoxv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/geggelkjn.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gxtwoobmd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gavolgdwm.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gnqgblhzk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gsnxdtyxp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gkcsabafg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gqmokifgp.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gjsjhxdsj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/guqncucrl.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gctvbdyeq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/garsagmrj.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gwwuvxisd.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gojkxumwa.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/ggpknsctc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gsudwixuo.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gwmsyrgen.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gmqzshivh.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gxeaqhwfp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gxrirmhma.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gnifpmfsy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/ggandrrjt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gpmmaajsw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/grygvcyzq.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gsaafjksq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gjmvmedez.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gorfxyehw.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gavmlgpsi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gwkfbfquf.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/guxbinzbu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwhvvcxef.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzejhdo.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gxmqiqaxu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gjuwbjdxu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/glcthmzec.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gmfvkeyip.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gneihnlnb.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gnqkqcikd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gybzmwuwd.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gwizazjsm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gfzrsyxbt.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gdhpcpege.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gbzsxeloa.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gnsklyoaj.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gpznejwyt.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gujvaqchq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gfggmbgei.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/ggvjwcgfe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/ggsesligg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gdaiqiivb.sHtML


<!-- 参考信息 -->