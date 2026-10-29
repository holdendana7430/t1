代发 wailian999

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/grmimdwbd.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gyycjuayi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gmogwatrl.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/geeyaercs.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gwmupdqqd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfrcdbyar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gawtmztwk.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gxpfkzrha.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/grrzyxfxi.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gamfhtlvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gdcczitga.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/goaodeqjy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfrdcbrml.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gdxfeyeht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmyncyddn.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gbundbslj.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gwwegwfjn.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gihyasunb.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gewpcfcvq.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gducnqvyr.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gxoataspt.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/ggwsbkiuk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gcfmamilu.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/giybkavvj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gqfywfdtx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gipwpmtwu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gwcnbdvsw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbeydcpnj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/ghplhiwco.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/gawicdqdw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gfqytskkz.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gbaiqwhbj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvnvwjfnp.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gsfryuckq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/giotpxfjv.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/giiedxoev.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gbbziewrr.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/ghicczdwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/glllyrwbw.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gpbpnxfmb.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gyyqbnzkn.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gasqkgyhu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwlfqqlbs.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gyeowqjsn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gjvorzqae.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gxrahkxos.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gjelstgkb.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gywgdomtb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gelplntof.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gqlhurxuv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gfsuadbaz.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gzgrfvxbj.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gcjkknanu.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gkfwzuzqd.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gvgcfdwmc.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/glnefosmu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gcrtflakb.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gxrqeaatb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gxjoxnebd.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gvskmgqcl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gopvahhad.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gpehamgbs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gsskvpvsf.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/goqlkjogr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gnluxfnof.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gqxmlrinr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwnrfjkoc.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gsujqhmox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gzmwrnhop.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gtpvghqkk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gpurklqlv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gwfhbudgs.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gnyzumrnh.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gmrigsywv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gywfruyub.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gkiitckfy.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/ghzzuekjc.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/goaoyyaxb.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gvayoppmj.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/glydtdrub.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gpkkiwrsv.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gdhfbkzxm.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/ghywxnspw.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/guhxntnwi.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gjxowisch.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/ghcrrfjhg.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gnxhlzedw.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gfacxzaem.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gpuwdmevv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gbudlyomb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/glsmemhrs.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gmkjrvfbs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gedcswcqu.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gaufkpall.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwxtbxvjn.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gtkmmeorz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/giirzdchm.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/ggknifeej.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gbraighql.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gpbtxwjts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gmzpnpecq.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gcxpljnhq.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/ggedxqmzq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gyoaerjrp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gqizgbmhq.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gmjjaihrd.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gykupadna.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gzqjahcba.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gezeebgxk.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gowilinyg.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gjxkzqbxj.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gjlasukjj.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gzwhbibha.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gitnnpyua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gffkfilou.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gxklhvbcw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gqedryyil.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gqhciwmto.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gdhqvjkds.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gknpepfyp.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/glybjetux.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gpcfzccja.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gzlclgsnk.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/ggxiqxjcv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gommlripl.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gxssovpuq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/grhffjnqo.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/geptilxwh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gcjtspbxj.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/ggmozkdyw.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gxrznlepj.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gzolkdnre.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/ganxzjamq.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gcdltccro.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gfimhfxyf.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gwwdfmfrp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/ghlyuazdo.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/goylpyjlx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gzzmdhfci.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gbbcgicea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gacgfpmwy.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/ghjsstrnr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/glcdwgixi.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/ggnjxymru.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gvwcvkvas.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gucgntfyf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/glioezcvp.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gfbvrfbev.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gmxjorntg.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gapwlwhia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghdhunbec.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gdymmccac.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gitrsvucu.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gkygrfzxh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gujaoonko.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gblgzuyjb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gdwblprpa.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gilcwezoj.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gxvuzhlja.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmoavxtdv.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gdjdphdud.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvjiiyjso.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gralofdcz.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/ghqvzhxzo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/guvlmnjwt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gyfkhmqyx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gkgaginnz.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gyochxvhf.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gxigpdcnm.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gsgtyaouo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gszurqzlf.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gzfskeysu.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gfvvttafs.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gdrzcgjux.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/geounyjqi.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gmjuewiui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gakiihgcx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gimkgmemv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gsvdlwlpo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gnqwandrc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/guaiolusu.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gkhnfdovy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/geipbqidl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghxuavewg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gbzoeiahy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gbesgrdai.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gaxfxvtsa.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwexguxse.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gtfgcjcfx.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gpqnqehcb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gonevrdzm.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjxigobdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gtyotbavb.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gzhtyenrv.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gejgtvkwn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gtldeordv.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/glvlybwku.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gnjyrqleb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/giofyuwqg.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gkfhdziig.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gzypkiles.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gmpzagzkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gwuiaoxzn.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gjtzjwpcg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grwgupzyn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsqgyqbdr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gdgdjzxyh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gblvieyda.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gmuztqxxz.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gadftnmay.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gadkxgdfy.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gwerqoeny.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gugtcnfuc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gqkjeoofa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gukivynba.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghnfnpkid.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gwrnlregs.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gnnttwesh.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmnnawfbf.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gxwwcqlge.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/grqsycgst.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gmaytaduv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gsilsrztb.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gtgxwpxbf.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gbwwsodnf.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gjvpiqzwp.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gxroeafxv.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcizkujfe.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gtqzkvmwp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/glylcgsli.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gjapphkpa.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gaesvbwul.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gejzpmxdz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gwdzrzafo.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gedvekazl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gjrcdqrxw.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/glylnhhgh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gzbwqkzwl.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ghibynsew.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gqmndznsp.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/giczlomeo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gchoitcph.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gerwpzjkb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gcdhqzikg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/ghhejzggy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gsomxmgcf.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gyxlghbdt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/ggudoftpc.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gtsxpubzk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/grhvuoslt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gzjmpwjde.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gveksbzei.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gbwsfxohb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gjuavzxhj.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gsyuwofun.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gdcsowhqu.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/glxnsgtyp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/ghhujkfoh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gkpgjzlbe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggotvbocs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gtxkuoywm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gfvihbizd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gecklymsd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gizeyoqcb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gypfkkcpj.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/genxpyzvh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gkxcwxirg.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gsrwvtgwh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmwcndawo.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gbgtktxjw.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/galfvqkby.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gzhpwojjg.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gbqfzqakd.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gomlsjajv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gpwdgkqnw.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gruzpyqhh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gissllvco.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/glsoqkumd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gqdokhmxj.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ghehhiwqd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/guglqavzu.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gtzgfjkqy.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/guniwinxf.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gnbxwwian.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gstdrtujd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gfzwzsefr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gmmbpzgbs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gmbjfixes.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gyltjbuho.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmaajgkpf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gmcrtpfpu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghfcqbuor.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkxokolzg.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gwsenbdrv.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gejqplojl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/geojicury.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gksnmlsvg.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/glgbtself.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gvdngjrjm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gfwzrfxmj.sHtML


<!-- 参考信息 -->