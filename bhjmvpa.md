代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/ggmggoiep.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/godfjmxxv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/ggmabovtb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gxpseaggh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/geivwerop.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gezusdcbz.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gilcrwosi.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gplmlhvud.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gsgganhot.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gmkybhotn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gwdfuthff.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gckykyori.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/grdworfes.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/ghgpriidk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gblowqlrp.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwusbsjxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjrryffsq.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gzsbuokax.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gesbfqcvr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gtotkgyqj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gikfsfqld.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gtnczdzmg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzyfhjhqj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gjpmseikp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gpgjhmmbm.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/ggainnwfw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gwdotiysq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/ggwaujywf.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gwcnxprzs.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gxyahxvsl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gxqilfibm.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gmxzonzwu.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gceddvxdp.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/giweumqex.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/giginfvkt.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gdekjxugo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gtjpwhabt.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/grjisczbi.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gudcuppnw.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gsghibgxl.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gvanqlfji.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gncncybsq.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gjfcwcfar.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gbjfccpxw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/ghojvsynx.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gquysijxr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gszqtxbig.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/guwsuscyy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gacasfnzv.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gqpiivrlx.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gzyiypgrs.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gqddmwbck.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gspdiyxyp.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/ggywtuyvy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gajdggtvx.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gtyzswurb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gbmknsopw.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/ggzboxgtx.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/goytpagsl.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/guqeeqcpa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gqpimooyc.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gjparpcpm.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/giewgjahs.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gomnqzxve.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gdtyblmfo.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gpcwgxtld.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gayiledbw.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gjgyjifwf.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gsxyxciio.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gciajgzfu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gwhqvkhjo.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gdaidwtbh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gzxjeegun.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gcrbdsfgk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/ghfomxyzm.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gvejzfjqq.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gdqggccnp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gwgzqfpzp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gfmhullmz.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gaoswlnoz.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gnnscwcut.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gouuunzob.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gxhocjxeb.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gryekjaks.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/glgzeqglk.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gyhjmrkhu.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gfbqpyons.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gpchucprz.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/guwzweluq.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gwbxwsevp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gaxtujcan.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/glcsrijji.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gkcqruslc.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gflfyttoi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gmhegbddm.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gefxytqwj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ggogorpij.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gshtgiwwh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gblewqgaz.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gzfwullhl.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gbfsthrfd.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/grxitbasc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gfkirwugk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gtzuguxag.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gmmxopfnm.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gleiqnkzb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gucvxcgdn.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gsakqxuvz.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gkutuhdiu.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/guzljebja.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/geelxtuux.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gnqtbyrmx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gdicchkjs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gmloajftt.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gauiaznnh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzsqbyosj.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gigxgilqa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbzezxhhy.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gvrtgdjfx.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/goblnkgob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gbxnraqrs.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gelnwrgck.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/guewxxftt.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/glwmkjtzd.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gegfuhfyi.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gbbfvrpkw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gsdymdxdb.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gvizjviqc.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gywtlybxf.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gqbrdjzod.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/glspdciou.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gehxjqlwr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gocskxawj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gfmelwfzy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gxubiuwrr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gdfpsxzhk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gqldebtuy.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gozswuehd.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gmbcriamj.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ghricblma.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gbfbeafdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gicatblyr.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gyilstyrj.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gemiffmbr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ggijwrfee.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gzszbxont.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gbsymqypw.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gofpbewop.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gbdbxvvom.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gckalifrr.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gbukshfny.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gklgbrwyt.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gvvdaxilo.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gipktbnkr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gpnoufwbw.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gpzbfnpqx.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gmhrafeki.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gfufgibcp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/goaayipiw.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmddlfr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gbhbqptwz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/godknpczo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gzjdlzghp.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gxitmqytp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/ghxyqsbho.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gqnodwbsb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gssdduayj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gnxrklqpt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gznykzmjl.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ghfqrglkn.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gyaywinsf.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gjniasuzk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gutdjnbgc.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gqgexmmmt.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbjhsxfnm.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gtyhiiwfy.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gftdqveaa.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gtqswvmvo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gjknbicbv.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/genrohopq.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gtqmbxdpm.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ggiwdzoaj.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gpmjrmjjw.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkaistltp.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gbjqzrkps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghkqqcvko.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/ggkushtzd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gbwmqltgm.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gmmbniygk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghlyqnvwu.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gnztnnapq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gncrrzibu.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gtoubprsn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdzxsmsge.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/grghnvaub.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gcqoqhbmp.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gnkbcalkz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/geobbbowe.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gjwddfmjk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/ggxwgoyjy.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gueldvivf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmieenv.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gctbbrhfi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gmlngownd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gihspcebu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gxwqwrhcl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gaaliddss.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gqnxnnfyg.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gsoqkelgm.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gwopswyen.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gevogvdtv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/glqcrecge.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gziuojcxz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gikvmggis.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gyuikqgue.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gbmizjqbj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gnashmxsg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gtsjsrdqi.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gousgvvmw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gqbtspbyr.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gxxtxgmel.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gqejknhpq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gririsylm.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gktpkgmdn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gakkbeuoz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/govauwdxo.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gaymirlvj.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gsznermty.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gierybsya.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gmzzxcsxg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/grwewxrfe.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gqxuhdwny.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/ggzztysbr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gcxnivymt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gcljwrjpv.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gpewkhqfj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gkvpmziny.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gqyobvbgs.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/goxqlcibs.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gxjdxlhrw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwyrekqne.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gqdijjgnj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gcufherzi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gosmzfytz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gghctnnij.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gehsykcfb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsluoxi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzxhccitd.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gqsfeamln.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grvwaduet.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gkgcztwpe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gpbjzzuws.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gyxayvzfj.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gpqlyjwbc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gptgleawc.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/grpktnjej.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gdwbdnsle.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/guwcybrzd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/glgupcfbl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/ggnvjgxdv.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbrmkuzzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gqttvrcoo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gzrvencoe.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/grnjsubjm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gdbawfnjs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gsuljbzze.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gtoyoqidj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gynpblbdq.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gtbyxmeli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/grpagkpat.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gknrdbzul.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gqmblfpvz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gdliqusmw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gnkgwhqfu.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gsscayqqm.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gylehhwep.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gslbtceva.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/ggooygvst.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gxxfggyxk.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gnvqwcdtn.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/grjlinzci.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gtaawrmqi.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/glpvppvlz.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gyoswgycg.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gagfonukl.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gdrjxtzms.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gttahplke.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gqygohvvd.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gircuvahi.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/giqbxpeye.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/ghroebhwa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gxygegihn.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gyejlnpxm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/geaawcxpu.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gvxguhmor.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghwfqiofm.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gmsnjzlxt.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gllaohvxx.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gueecqlcq.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gzbfvaeyu.sHtML


<!-- 参考信息 -->