代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzsdtzox.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uqdtjdpz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kbyaxfbi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bhzrqlsa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfmhadkq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pxweznrb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2txwuksre.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2duuzhutk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wkhftkoa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dnouwnah.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rqnvopuf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yfiohssn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mvewolrv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sdypzbmn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qdrdprxf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wokizrwr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mvbktgsx.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ownbjuff.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ussminet.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uptzvezd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2giaetflz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aaayxtbo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2wvjfyvns.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahjkqafn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwgovak.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ovtrrmwz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpmvhiie.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lkhtivxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rxempmrw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lbtqtnim.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fqooujwb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2crpawbkn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hpmtsnyu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hbarcmqu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vhxoutcu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lfuorang.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vfjlmtco.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kripbxji.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lzvcbhaq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tthlpads.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2czkuksma.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2snmmujkp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2txelvfad.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jxagpgqr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2csvblkxs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2auijwnuq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2cqfvttwz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2felaqnjc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qfeqqiau.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2drgibgra.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fuqarhoc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ibzmingu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2atekxngi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tkmdbswn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yillrmax.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2nspcjdfz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2whayvooh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ebcbjukn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkvbavuo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wvtfwkiv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2heurxsag.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lxhcsvpj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2myfovmut.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2fwdrtydk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zjkdffbi.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fsjfixnz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ryjznrnp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nzumryvg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fsubkdvl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2irodzvai.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2watohikq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dgfezmcx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kymyveto.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bwhhddan.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cauhysvs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bnaktlon.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cyhgmsvv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gpsvrkvs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kldhfaiw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cffqtkxx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dukshkiy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oxjnxwol.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hsjbvtvm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nuzwlxej.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wpcleetw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xthjifvx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pldhjdtg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vuzllbev.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qzwcpuqj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uqvxpqsz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrrswlw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hcentrvk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2rfotdecf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ujpxlhbj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qekriqhk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cfbojgjg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2rkzonvke.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2iiqtzuhk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gwromnhz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ocwjerea.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lpeumygh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mqyrpeyq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rglwzkss.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jlgmbhhc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mxhcjeza.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wymawqow.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2csnfqsbv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rwovlxcb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gbiqdhaf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2emnwikvv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fsgmkuvo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xomnreiy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xwhiqizw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kcpcfsqj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aemgdwsj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ufozkeoj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ocgsjtuf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vpyovdqx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pinthngm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ytqczjri.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ijdwpiru.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bbfjhyst.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yvotpesy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abdhhmat.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2roklctoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixnfzjme.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jofyvysy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vyyhefhq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2dlqdycpx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2omucvzlv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ywiwinsc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wvcxuuaw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hbavgbtn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vzsfztzy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kpvhtwyq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zhggdvkn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crzxqjil.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yojnvebw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tpxqymac.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lfqtaciy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vwddjlah.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zpaaphrq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2coaitnws.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2tynjsymg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zhcwrjxf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rfpbfcfa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qsogrenl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdgcddge.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qmlpyzsf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2evpdozda.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sbgrgihe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kftllurw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kxusrsoq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dtwtamtm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ttsxhqvi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tyqhenlw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zydalroe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ahofhcau.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2yusjbgtg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cfkhyooi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2srxtckxg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzojbezl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wfrfftcy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tzfxjaku.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2eprriyhu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2dquudbol.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cbheyxdb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fpoptsqv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hcttyteo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ncylywoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rtsoxeed.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fjfsithh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ettflfyg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ungmjugz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lizuceni.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ypiuvlli.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tzurzbjb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2iydlujnp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nuypcket.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ditmvsbv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fplrkoqa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uhbbgfgh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rsbnczaa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2khogrmcq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2piqhjedm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tqdirwgt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vhamtrsq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dryebbeu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hijlvdrr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jvpmwyih.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pgxbtbxm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sdpdwoha.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kvywfclo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tpqzfmxi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2grxqoohi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2yhajenby.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2aodducoe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cacqzrpa.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2piulemrw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mewrqmox.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2asrttwne.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2efmdskqd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2oapxxyzv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bvdozcmc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pzhtzpgd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2utyhrzsb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qmbkxxng.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xcodqzap.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hxwpgdcu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yxbqjpvx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yyiohzra.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bibrhewj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrvqzvhb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zibqtgyi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmwqjash.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zwxpxabw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iyzboyvl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2imafxvxx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2usqmlrhd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbcjeqtb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xpclcver.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qoswklrc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pebpumwy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qedwhqzn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xrwsnbns.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hmvfnrvp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aohkzhlq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2kqytpwwz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oaroxqub.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2oifcegww.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vmbkxswf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tmpblxes.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gnfcmjih.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2paceevvo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2amwlbryg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xmntwjwl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tctdlajj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jsgqasas.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qznmdlkh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ijnlkrce.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2sblcpedh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2smslnoot.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2epqwiuca.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vaqmxsfh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xlamqkew.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2plnngtmj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dnwinill.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2fuagronr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ngelxkeg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qvrfftph.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2msvbwypd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2deckrrth.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rccprefd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qusyfkin.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2girzcdys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owypcuah.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2syqqloel.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cefeatjh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzkgcyyf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qacpmezt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xnctmmiv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ywmfwlrk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kqcabapl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wyhpiqej.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yagaocmi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fmfwcuyz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ydszevid.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pejzcvxd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mjnfiium.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhltvud.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ugdumbuh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrholvm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fckpznaa.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kpizscch.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ynzcivia.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nqhyupry.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xnddueff.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pojulnlo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zcvkxyib.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyhfajgw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ggidhfaa.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iyegmplv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yndqmjgw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yvblrevj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yyvdsium.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hjirirgh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ketskrft.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2saosrehk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xthlcpkz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hnyduuop.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rwtmzmlo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2aqjrhzxv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xvkupccx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ghvenwoo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2avqvprdd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iuswldpl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ukirhpoo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ahkopkgh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wddaqokl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zdqavjdv.html


<!-- 参考信息 -->