代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lxvehqap.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lgzypoks.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ijrfocnv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2islqmllc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xinkpxvt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mmompquo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2zzojglyg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cfmmdjpa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ykslluck.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ibfpgtps.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkncpffr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jyfhzspj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptcbcpsz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wlfrtafv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2awjcyuae.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bsqlolha.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2owjnwnhy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2oqoqipau.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dyukfdwn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrfwvoih.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pqfsvfvz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gcgurljd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qttbjjjj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tkzmtigu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oscghudd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2atpympbp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rirogjvx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2umxgbrrr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cwzoveiu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2xefbjdxs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2luttvbrh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gstgkxrt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2alqmctpn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2haijgjoj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gmdehspx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tbjifyyo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zvkgpfaq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2eaxnaoxi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rtrzeejv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gjfharos.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2eyqxeuoc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2okfoxovs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vkecqctx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hjviblkw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pjouyyci.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2prwxfkrr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2frzoplvj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kziibbpr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vimubxeo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ytqpcnms.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mqaywucy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fffwdiyp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fotcvjnr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2snrxpvwx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gjqdligb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iaamdfdl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ztwzovtw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2edpjucar.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pipcbabl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ztqvqcgf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ismevwiy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ueaxfsac.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nsbkqmav.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zjrtnnzu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2swgijtzx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2shyahfov.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tbcqftka.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2svfmxaov.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rcakyjcl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwjkutqn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bbxqesge.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gprtwewz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2aodxyxut.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rkitgoye.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2iuziqzhx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ghmzwiru.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rsilcsdz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnnqwzdf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hwpioswb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yygclwft.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qdkrhxsz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2thkwlpiv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2upoxmfvs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bhzghine.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2umoalfyz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xghcbara.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mubfcaxe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xktyhvha.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kdtqcolg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zbapfwow.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gxsedood.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2inqibimq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qpeajrru.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qgbuajef.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rwoxhztv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mehdcutj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iipixevu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vevdnsnu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqqqyjvd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qoozpzxk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bswidadt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nufqoads.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2whnnbson.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mbgwjmmd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lnvaxbya.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xbzvorrf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kjswccsz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zjrmzngq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lrgtpiwc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ajjuyflr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2owifqwcj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ohwfrxzj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wboebuzz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hukremok.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pvwpascf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zckccrpe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vuwqpksl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uwlzjkrq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iiuionkm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jppbfown.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dwlxcglq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fsjekxdr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vuwogweh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtnpxtmx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2egqfyjfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2roolmvui.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2axxahxdl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mprngkmj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2teaxbwcp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pdcpgqri.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hdxtxpcb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xusazbkl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2uzcrkfve.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nujnvwkj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wlbzxszn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cnybsngp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sebqdkgk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2caiylcid.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fdxbzpvx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rloeqglc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dsdcopyi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dqishihc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jmdegtpc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2zaaloadj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pxqbtgad.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wxcafuat.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2pzhpqjxn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dkjqegxk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hcacyivs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zlcpmjjh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iycsgzbq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ostedzzr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vrbqeoke.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ihzrkvnc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2huzmrxbd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zdrmresn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2aweclzep.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cafrgvrw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2gjwdbblw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vpafxbtx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zjxwvzqe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vatdnkum.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ursdqcjg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vflusfnx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2btyalukz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bknnaqqo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2utptbkuc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gdgzdumh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pveuampl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rjkkmgoz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ogehztiy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xjwehuyy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sqvzhbsl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vlcitmcq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jgjgrhgy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ikvjcxkq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2laalwpjb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2hlvuvcdt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2usygfddd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2disvzhiz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fvrjybvs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qhncjbdg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpfgfqds.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhapeocj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2avpgrxfr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxbfmajp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dmmutlub.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fmbltdso.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eavxdeqa.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hiqfcspx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ajskslbd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2satciiaj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ksmamacu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcuwajo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zquasgrt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2iuuyvfdq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mhvkasgt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2voiehgos.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2mwzcttpn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ajtqfaey.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ihqivear.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2loszhssm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xfykghtg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yfxpinlo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sdylbkev.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2amvnecxq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rvkpmnhb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bskvvnbs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zerradfh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bxnfqytp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pqfhfadi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jdijuyaz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ltpwandv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2icpbgdvv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ixhasvdn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jfpzdtrx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2spkbwqfm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pgclkusd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hfycmrxj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xouomgjh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mytydrif.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2wqaqtbkq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2apqruhlq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2woblblpx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ecclmptj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ztulqojo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgpaqmqh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nxlvlslc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fyzhvouv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlbjcnnz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yajahdat.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wpjwrrpq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ysxhqgcr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2qawbuvys.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jkpautig.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cdymswad.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2obrmdbjf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ejltudha.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zwtfbcbf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uijziscm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hferfixp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mvbzhagh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2dqorioxd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kmxkguel.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwpbnkmr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2eivhcmyi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wrdvglrx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2wflzzipo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fgudrjct.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ycrpkxyy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jbfpojvq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oybjmasl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aejowmcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjjpvmoh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bafvxmnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzmftvtb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjytfoer.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hchrgfmr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nytabsqu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2itwlrarl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2omlkqudf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vimlyqlo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ezxbgzlo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mybdowpr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sfjxmvjx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xprhkcpj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ggmzbaue.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mnmemwsa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fpvsbjwu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vjakiitv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qhzzqswv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ahsuxgns.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2waytiwfq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2mdzvelkt.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxqheuvg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kdzrdbtc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ydbejovx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jljqhkri.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lxwgprgk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kobrrlrz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fmisqyme.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2klteiawv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iariwdjv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dxvjmbej.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hbbsqmqz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xmmahemr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rlplllme.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2orjmpraz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pumuvamz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2onkdudtu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nuhddrac.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nlladqvo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bbwbsweb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xjvaaded.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nrslxxxk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2treemwhs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wkeegapw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2udpkbngk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2lerchvbh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mccmoxoq.html


<!-- 参考信息 -->