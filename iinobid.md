代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/getevkrac.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gmetelawt.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gsgkcsvur.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gnkqtwywq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gjuowhmlq.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gidwqzmqx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gpynazsdm.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gpldnbklo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gyhhpmdyv.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gjvlkzvtp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gistsmmyw.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gnicenqhx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gnheaucgh.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gjmumclek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gselqjwon.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gbaiqkftl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gazqbabgm.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gaifozxud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gimkbzhux.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gfypurgxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gutgdvbtu.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ghawfwkjw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gwfmpyugc.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gvnpqvybu.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/ghhteaulx.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gicifeupn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gkohpyibe.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gffwoqknt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gdfrbgiif.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gimsibnjt.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/ggewcaawm.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gysxjgoxr.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gjosyikch.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gslqxxhlr.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdecpbleg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gebdrchzb.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gnmqziofw.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gwfretnyl.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/galntixxq.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gbmkyimws.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gdoducrha.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gwjsbgwat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gjhvowpew.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gaksjvtjp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghcsqmder.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gcxziiipa.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/grqndqgpv.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gqgfmltlc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gciihvgda.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gdvzalklv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gorkjzzio.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gefgtkhor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gbphjsmzc.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gttiwwhos.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gtxvpiggv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/ggcopzqub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gcxqqwdel.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gjqnsrdke.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ggffmeazg.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gkivyrhcu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/galyyvrzh.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gevaiqpmj.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gqenvbueu.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gjkekpozs.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gkupdzipc.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gfarmwnpu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/grdyimnfl.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/goxlrcrxy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gtmxactme.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gslnkpich.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gemtugxie.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gnsfdtdhe.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gwlshieno.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gelutulow.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gqdpxmkwz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/guclzrpkz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gwhdtztqe.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/guyipsszr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gpqippklr.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/ghhteltjv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gpeflsrsd.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gpfwsdqou.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gqgxxrevc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gkiesddlm.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/glvigberg.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gdhgyxwjh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gavibjfhi.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/ganfvroua.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gwwnsipjd.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gfzwqzdhz.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gwgbsbqnx.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtthwprwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/ggbyguuhi.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gkbsvkhxi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gvjxlyrkx.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gxdxjumwp.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/giogirbrh.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gxzneiocv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gytjfafdf.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gegvgpegz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/geluwlylx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gmldjkrrr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gstblesrk.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gjjedzcvd.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gunyoaaks.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gfeksomqf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gkotfurok.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/ggjmzorbo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gzzzcwpep.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gdnqptfok.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gvfupggrf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gajhdynen.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/goenhzdsm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkfdtcfex.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gzgewirqz.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gnbyzwhor.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gukhhngrt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gfdeondhr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/glqgblhkk.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gxktknxjc.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gyhzhdkry.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gblffumdc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzwdhgjfa.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gffacpumt.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/glezgirsn.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gzhyjpgff.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gsscwcctr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gapaexmgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gvgrunpjf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gvvguifgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gdfgnwxfm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gltvowdno.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/galoprozp.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gmgccwinc.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gfffhhtcx.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzvaxylxy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/goxizoukt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtusoabnq.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gtldcjimw.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gcxakaojf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gpicbrbgi.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gogrhpumt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/grmtqvvdj.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gkwisfuhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/goludbfim.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gkgbtzyaz.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/ghjbzinxr.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gjrxohsvw.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/ggzozombb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwafthiwr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gvtxxuhzl.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gydzgwyfd.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/geogrsgxe.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdcyksv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gdvfbgico.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gljgjwych.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gchusqdgb.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/getupeoux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gisjhqhtg.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gonnzuwsf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gpnqugzvo.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gmplpskvs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gykkqgwzk.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gkwmjemua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gaduyqpwo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gebnrauft.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gjuyizzuh.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gldalxqyp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gcumjxgge.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/goynyqyga.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ghdtdwrzy.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gmjgkbvtd.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gjklnuvwl.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/godmxmboz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gvrwuqwgh.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gkbttvdrk.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gczapkmyx.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gdlchfqoz.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gamnbiqzt.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gluyncwyn.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/geifddaxf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gctydtcde.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gejqowdng.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/glplnuaar.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/ghvmbumjl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gvtpfszeu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/glkkjplwr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/giplnsrfi.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/ghxzdqgwg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqdtbczy.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gbuzlgsnn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gjtaaavoc.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gagnykiva.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gqioxiwyg.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/geqnpogtc.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gonszodoo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gijvusylc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gyyfmazqs.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gokwgmhks.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gquxtkzfp.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gkneribkd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gogcrfrbj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gpmdaujyl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gzegkilko.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/ghbljagwo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/goxrnvdsn.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gbhccoccz.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gatipuarv.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gtplxamuw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gqrmceqdz.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gshxqhwnl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gnckrpiot.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gelastfke.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gsptmvnud.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpkkdppay.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/grpzumlre.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gdtnvdzje.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/glpzptrnm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gikgmelhc.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gggiovyec.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gwugrsbau.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gibkqpgat.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/ghntpbuit.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gzoyboqpx.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gooocvokj.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gfhztcrtl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/ggzdbfvbv.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/grhvejpxt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gwxoiuwyw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gfxxemtue.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gtqiqbhce.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gcfddcqgo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gugvrzbss.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gyitqdgwx.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gssvrmxfq.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gbsdmmthn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/ggztlwvgy.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gpohbmtnp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gembiqmyh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gieneumzo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/goxexmgtk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsfmruorh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gvczjeaod.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkchbvqvw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/grvyygusc.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gatxiteib.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gwdpifffy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gszzbeykb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gflajqlfk.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/ghvrfceud.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gwtbkuzgh.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gfmvcsmnl.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/giehtpaos.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gdpuywklx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gpkjtbnth.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gulsvoqnd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gywlykkdw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gzxphmnrm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gckoenial.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gemxsckbw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gnchyqsjh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gmyctgija.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gxlsieiwv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gozxzwina.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gwabvzzdz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/geucefdmb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gemenqndq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhqfhra.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gfpguomxh.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gryxptnom.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gjvcxygaw.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/givbdqwie.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gbyryjzcj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gjwopniyo.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gyvzkweer.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/grbwbcapa.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/glvezywpe.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/galkgvqqs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gfvihtylq.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gkirukozh.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gqhgxllhf.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gmzcqnexp.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/ggbqqtlxa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gihokkgec.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gniwsxsnj.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gdrmwbbtv.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gcebanuor.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gjwodukbz.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gfxjziwwa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gtzlptecj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/geuaawjto.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gywehtbbz.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gruvsmvgf.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gkebbrahr.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/glndtkiao.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvokfqmcm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gsorvbaqi.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gavfobkaw.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/giozgwxec.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gynmfpbst.sHtML


<!-- 参考信息 -->