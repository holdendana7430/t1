代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2etinoxhh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dgulgkim.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dnrttikm.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2svfwqvmi.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2opywkmit.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2krojeekn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2znqwgdeb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sghrtwdy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jfmeegzb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2woexihng.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2itgngtwi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ozahrnip.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dtvhuxtp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2goscunog.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zmoyqhcl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2maouyace.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ouqbmqju.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2iyshugmi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2gqxeasep.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2scfvbxcg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ohqepvhb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kaplbmcr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vctnkimi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mizyatwb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2akcbrqbf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zksdpdgl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vinuysig.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vjdmdqlg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ljxvcgck.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ytclplsg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cvqdxlry.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2omxatwek.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ubivrhfs.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qjnmwztd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bonnqztr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fckqhxrl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vzxzrbxn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kcubuqrb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zhggftaa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2culwekdk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nrxfumyr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2axtnrxhg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2irewnbqe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cxuwtayy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wiofczwf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fkfewdud.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2lygbrhkn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nfmahqxm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yxompgov.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dzjwrdup.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tovbxmbq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nflnbuap.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qucomwfc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zbsbisdb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2bczsbmae.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2luzoxots.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uhtoagzs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ntbptvcr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqshtzkc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mgixapdz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jqpiehbb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2udivszuq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2txymhkgs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gpchxoji.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2achifnib.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dtxeglss.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhlqmfwz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gbwsqgub.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2zkhgjijo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mxtnlpeq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2myeptgtb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xyeekmga.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iynavpdi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nwbdhymm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xpxajbqu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ywchnaxz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ovrahgje.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2cnwimnho.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2leqvxqfo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pmbulbfe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2egwrhtad.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fgvnzpkg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vloccysp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qyjlhxll.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2emcywwjr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffgilfzy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ijiyiqge.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vfccethv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zcmnhmqe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jquumcls.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gtgdijvo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gntsrgrk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nehmymtz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xthpsiws.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2knmccwbf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vuacetxm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jfbqrzap.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vbrmwbua.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mgtcnibs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kuiayahy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ctgijhkj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gyxnkekr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dxsrzkoj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ijwbudnr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kkhfvwot.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ggmxuari.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zjyxeyqh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2rsyfbvul.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ywrncjid.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lhsagqfa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2urxglije.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zhmkzoxi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2oitqrpxn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zbyyufyz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fmsrofss.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2afheegdh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2swubrmic.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dxrjwopx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bthxbhex.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ygfxioci.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nkyvejpr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qgdsgons.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vhraqilw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukcwdxtv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fjshbpku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikgwbtqj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipdgplfw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2owusoobf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmejeix.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lagnuhwv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cavafugb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ejunmapg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ocisbsja.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2taqzwwuz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ovfbklam.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrrxtc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zrpzbpad.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pdvvghxv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2svidwnrg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2sfvkfkhw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ajiazwie.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2uzfgardk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xvalpxzm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fvcxkruo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2oxlbruyu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fhtbqhse.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vaudtgev.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zterxfbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2sxamdxyz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xgkzgbhc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zznaqwnj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2azronxdo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2immmljnr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xilxizjl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wnfesutv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lejwlmhn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zebulvkg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vrwpqnqv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rdmpsova.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ehwgudrn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2krislavv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ysdllvhv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bybphhiq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2geuajuuk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcfqubi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fsmreqiz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pwhmbqkz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fcyufpfo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sivgpuvi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ilhdijiq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2srhxtbsy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2eugxzqsz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ijpgwpna.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lxdynlbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tqiqigtj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2coxpmqdl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ipkjiebc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2umrcgkcy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2akxcygnd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zzfyrmea.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2rudlxxmq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ybokdytt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2spiimivx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2slveyled.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hzapxtuf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nffssdfa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2eewwajyj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fxpspsck.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qmfkjjgq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vwcabvas.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xhtnczog.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rznqrcwq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dnubvubj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2guwpjnbm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cfpfiynv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tuqvjqfs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nleodbmo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ofvvvuyg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2reybpofy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzmckoym.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tiluxqcs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2slubzrnn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bvuxchxp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qvfhpqws.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hpntkvcs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cqbmdjrs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hwrecuwi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sghnfras.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hkjnuqer.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2atsrfljv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ltwrnqhe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lvyosbrs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vgyauzge.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ggltueyu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2odkzwszw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2gqizvbve.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2emcpjnbe.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eoxhzxsj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2kfssxxtk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2andxngqo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mtwfudrq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vqvcwxre.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tfnvpwpo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2celqffru.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yvlzhctq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkxddsmj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2piznrapp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xjmwhogm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vdmiptul.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nhwuyifh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fnwcnkqm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uwjfvfsu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zuxveorw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cvmqpscd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gorjnncy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xvgnbksf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qlvrsldo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vysahqyl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2iddvxhpw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2acynxzqe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2koposmpj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2yogarnfq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xxdcpbbr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ynrjdilh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2itdsuubq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ozukfzrj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2usbihrga.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zdnzmddk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iehgvrpe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pdqvjsbv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2djmhrbjo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2okcvikns.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ddopdvvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csczdiwt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vijixgci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mthgjlsq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2votrjhqp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xlsqmnad.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2secorrkl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xeihgstr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2lknxlczv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bvpdhtjv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nnxpvmcc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uccllxwb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2srbwtwzw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ccobfeav.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2whlwgmow.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2civlyzcw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sdphlopu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2exmmtoyl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jcyjgwsn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xcujlzzo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rajozuoq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2odwmabkq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2holbtbqr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pfadbkfr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cglfxnuh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mabvbfxd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ytxtimhc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kixrkume.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vdadopwt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2usfoiclk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2soytnjrf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cheuwcmq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ijziyujz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2voujiwtd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2alsufgxm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tgqcpiso.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kigekhxi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oustmpvu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zoutpaau.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mzqznmuu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rbvgqaza.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dhgkaldo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2liwjxqes.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jfyclrpl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xejmiawf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2toweezmy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2aictewqj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iuzaamtj.html


<!-- 参考信息 -->