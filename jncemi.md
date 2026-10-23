代发 wailian999

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3welkjami.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cxjhifpi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iddotafh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pckxywzo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kslwhyxu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vbaezxfo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tbnfikgt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dtcfrfwe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pnvwhnhy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sgdecibe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rernppgj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3eutqsbmv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qxemaehz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nlczynll.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jbqaetfw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ycieanid.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3aopqsjpi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xohfszeo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yhvfgyic.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qzgcxtrn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kigitmtm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mzrygmvl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3warabawm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vebxbuxz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yvkklwrl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqgutgsy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zlgvqquv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bekxtmwr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hvqzcknm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gdgdtjsl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nkyptbwl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmwtxqej.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3gucvagdx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lzcsuidy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ljzolopl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hjvjcprl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ylxfkbzp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3phqehbkj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gnnccduo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ultrjmew.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pmwofigf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qelutyvr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3yqervqpp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3flbgodhs.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3crcnxyuu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jyimyoby.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3kgwplgnn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tncchngh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rqvsjglv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tqykmymp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3adhtotxt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xhlcpamh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3njnucpxa.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ayeqkptd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3xxeyiteh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3omxvlrsp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3aprhdyep.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3duwommqv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zhgcipav.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlhoslkp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xyboadiz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cwhgpwqi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ctdfurfo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xfiqgmtt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mpfzmhmp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3akolsygx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3snajzhhk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xvmfvbih.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uglzoifq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vktwipeg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3owbpipfh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mccxkrrb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zcosshrr.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bbiatdfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tnudnffb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dpbbczrm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sslcwkrg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3haiqnrot.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3cxztxrvr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sfszisdv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3oyukbwus.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tipeaknf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ifubfmib.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yrddfkvx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uhsmgwox.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3svahtvhi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3afcgkeza.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ttrmfoql.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ybxikzmd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cewxqian.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ktrdtpti.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3hwpvfhcm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dwzrxsvf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ktestcjf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dcamojio.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qutkrttf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3caemklvv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zatzzhbt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tjakwctm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bzbyuaqj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3niofrwpo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3byfuflqx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vwxymqzb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nisxagmv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mvfiwkqh.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lnycrngg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3glzdapax.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3jyydarkk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nsjlcdcm.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3auppcdbo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3upmyclig.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dyjxrctc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qdlclriz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mnldodtk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wiuszjil.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vkxrzjbb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3poitcvel.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ihwflzup.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wduazsze.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3btwbgtej.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hkhvazwi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wugvzcxj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xccauuiq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ddqmjaif.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mbqwlfhx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3thhdoylr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bsgutckl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qlmtyfzy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bhnalbpt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3riftvazi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3rdqapxvg.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fyammwdf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wrcjcuxp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hcubpnpc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hwrmeegn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jzjcpfmy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3elwqsjpi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3eepyrqws.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fdlfqzuk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3hhcfrvdz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jpdkpbns.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3krtiwjtu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rkllbjoc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gtaszreg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zmpkgvtj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3hgsqhqbw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pofjnyfy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3seghfvih.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tboypayv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qkqfbuvn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fcabhhyz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3avevnsrw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3xojfzbog.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3omzfsgnc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ketnctsb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qkugwicp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ddkxndbg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3whhbjgav.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uzsjmiss.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3oitorhtu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jlcvbpuu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3swytnlma.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3eihcdcol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izwntmas.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3winvbnky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnwfliew.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yaehaazx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qacsjsea.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgphlqfp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sbzfafte.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3luhnkuae.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jbkeuzco.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jhhpdjnn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gzkdqbss.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fhzezxkt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3madppngg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bvzqmpur.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3olnbjtga.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ixeoadvh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nzlxiryl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bjixtexw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rspyrjck.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sfvhxszw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3hchbhmyy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3sietvbhd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3sddcbylw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vbmtqvpe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fznihwnw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mnlipoil.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ycwukwaz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ybdocwoq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bmxamcuo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vaetsloj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yxegzoho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3udhlkvqz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cqzclqmq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xqxiqfii.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3aatoftob.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lbxoyydg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ycyyviua.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kseseruf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnbbxgqf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3xvajlfbs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qxpbfmrc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3uctdqlmk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3owfhdhju.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ubgylchx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pgsiauqi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wjmubpit.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pdnvmvgn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xawqvotc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gxkzsizj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dauudlsa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3manldfcf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wcvllspw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ednqfkqe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3imoydlig.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bjlelyfc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vutdeizt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fyvdbfjf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xvdllije.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tdbsqhrp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imnvkpjz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ciyupzhm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pxynczsp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjlxhmji.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jqwrqihd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nbmwqazp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vgvtareu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hyehcerx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qustmcnz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3otyocfni.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rryyisle.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgrcfdrl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3czbtyrpf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3unskoreh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ulzqxvkz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sixjmpmv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3euybumwm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijgkxfkt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3omflmuut.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3amkvlymi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3huntpljx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3onilavdj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zrhbwfsh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hpsbmpmq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3expbfoib.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dogxaycl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dwjxvnmc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3plfbxyrj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3hyewweus.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bkorcupy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dugyywqv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nmujkckd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xkbwjddy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jjcpchod.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3drnnclag.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bybfpzew.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zevtdjzf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqzuyjme.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3syxkikyl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ulbawfaz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nidxmund.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fxfwckqf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3tdbscjxr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3znzsdqnj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mlhhzalc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jahjhbfs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pssaifnp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nqgybcsf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qykbsxcv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gvjoesxl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aqwlndxq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mofqtpfa.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vchvptro.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jprquyah.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ephbpjtp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rcrnecby.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3linavvjv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qttgyakc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hereawfn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hlbgwtme.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3blsfmhxm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ereadynm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxgegjp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3oslnwsgz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ytufumvf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xwtvtkdq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cmiezdjm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fvcutkls.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ngfsysrl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kwsttmze.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xtiefrqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtdlpkyj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vwllyoco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkgdswkf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oeukkgiu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rzvkbzif.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iizmrgwy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kklqqbiw.html


<!-- 参考信息 -->