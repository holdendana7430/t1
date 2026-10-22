代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kdreogig.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2tkzcopti.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2swiozhmu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iqtjnlwt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nekwfmzr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xkftsqvo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ypvqzuty.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oeqtwpcc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ekinsyty.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jkwwyuxz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2dieduoru.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ovlpinny.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2fsivicnv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mpxhfbth.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mowtyuai.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qwzawvif.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ejtfxdde.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2goowhgnq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2eghhsizz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xrabwpqs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fzaddfml.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lxljllzh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nrmebpyy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wvegqazx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2gljnzusj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hadllhoz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kgqcqwaq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rkkfyneq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmvdsuqy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ylqhwvot.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vbjxwldi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ihbmdimx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ysptmrca.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jmupmgbe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qqmthrdg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ngfposcv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dyipborz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vbstqasz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bmfzsdbe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rsrsqdwb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ufhfmhyg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2snwrpynb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2sxxibcgz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qloexlrj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2icqzpvqv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gctxwuyx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2hytmxgss.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2tizevwgo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wvjlewfv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hwrgvlea.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rjwnhgxr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uggesyvy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2upwnwabz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ctucdpeh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hjuehwym.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mnmkbflz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2eovivmeb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zpaigehf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uytbmsii.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2nswkqbrx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oeijmazc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zhzqsipp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ggvtyqip.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jeupltmv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vpsrplwk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbnoav.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lindyqrl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qkxxbsuh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jicmfkas.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hegnfosr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zhmeevly.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ehlgllkv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mvanyjru.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbrirrno.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qdgdfriq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gphaoufr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rwbflxqi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2delkctyt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cwvwkeho.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rirvzvaq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lcaeqqqo.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2scnwlmie.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cokrebjr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jxncgbhi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wwbcvdww.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ceefcosr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vpqlbbef.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2evbazwlr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kbpyxzhn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2haunqbqh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sdwonjpz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qxmcaphe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jkjnvbpu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dazjuoou.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2blnigkkg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wktbbaqh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ulgmfxfz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uwzvfuyo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qwjyrcuj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nyxggneo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dopxvqiz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mtzsyouq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yljorktc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ndzptuvj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgatzs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2odxerlvr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2khljllem.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cchlasdv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hjwdczrf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zmothysu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fdwfzepb.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ukmznarp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2eljiezmp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zptwnctv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gjkdatvm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fltlvhmn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vcjydtnv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2yktqiner.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gpbddnvx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lgqmzxtq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2opcszdve.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jzsrvnwq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvytxpnh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yiczgwsi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sqkmqeqd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2risfdztp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gkivwfkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hradthtq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zzteltxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwddxvfe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kiyyqwoc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jrjrgfto.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2glgnjlhl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kipqtdua.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vmresxjn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ruhgvewj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2sziuzyxn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gsstsyxu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ggjzigao.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oryvpwyf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wxfzpbey.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2puganjuo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sumxiqrx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ltmueyqh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xdgrljja.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2gssztker.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2glmadcjq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qipevfhn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mvwnyusa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bccbhayq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cvycddld.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rvdjrcth.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2yiwbfufl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iikutknc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xhagpzng.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uawkhfqp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iogkkpem.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lqygmioa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2blcpadfy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2edrnvrtl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2enqnlagp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbycnrip.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fzcfktiz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hpnaehca.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ggathqcj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pkqukeeg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xlwctbui.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2atcifkyp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wazglpoe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2eujdujor.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ozlwkzhd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cjugynnp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2arxlojjk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2utywaqkp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xnrkpkxl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cztazoqs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eireelua.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gsynrmmk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zjojrszp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2iqotwjip.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ggzolwdb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2brhrhauq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2icrwgnzo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ohhqgcgf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2emmfhlpx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ctuionzd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cgotdvrc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pyvkxnnq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fbnfvizs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2prmaxvgz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xsdplsjm.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2pttkbpso.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kihlxgzp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nixocpos.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dmwyxdic.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfsazgey.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ptgrmpis.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2guyrcfio.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztpugxpp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vgokaefd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ixbwwckc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2puxfffiw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qrexfaew.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2jmfmbphi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dpoxwnmf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zuabpmdk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2udflpuav.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lnuglbuq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2mynrwsqp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2boqyiqlr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2naknjzox.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zbceuned.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2flrhbtet.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2swyfvvca.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2shaszwkk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zqazwduf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fmzmtgwa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2seegmhel.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocmzjdmv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xfvytalr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ocqllgly.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jjkjcqjo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gozsmoev.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2siahrsvb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qtcdybne.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wydszlrl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hzutzmwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbblnuke.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hpbeivex.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oporjcqn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lrvjdakx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vtubrryh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2egkdneru.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tizedngr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xcjnodjf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2htwjbzbv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qkqgzlzr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vwklvkps.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rbodxlfu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jwomwseo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvmagqus.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cvsneppu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rvujiaku.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2unelswyk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zyykdwrt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iawahrac.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nnyphzue.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2qxjxbgwb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2talfsdqi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2onsoeldy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2llhxcitj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2chkqsutq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hxblikrr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2sdojeqcm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2azaftkkr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qhmwbonc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mzkbzwts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaulkbhx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ifemerkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spmrfpfd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmqmouuh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ofrrkclu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rjjqldza.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tbpqgwcs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ponkiqmi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yjjqilje.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2abarebaq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bhprnlzt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ugdvhjrj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uqqlciva.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2frhcjobq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cbauiutb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pyrdtupf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mvhuxsfc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2anjhfpbs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hwswrtgy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvnvhhgw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fwnpkkmg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fkovwkpx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ghoppsea.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xikrtylv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2scfqvghf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2besfiran.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcgkqtmd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2pdgphsky.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qlaouxbj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uoitneof.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgxoegh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uxvlajpr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jeiljmdf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2guzuduej.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tlesmdew.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2qwfnlquo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnqnwlbl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zsdosing.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2npmsegqr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2phojyeeg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hdtvrovm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qmsnqyia.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cspixrjw.html


<!-- 参考信息 -->