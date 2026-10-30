代发 wailian999

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gncueslkn.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbjkhqcx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiysjqko.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gonxadana.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ggezfihmn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizattyiu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwpoclqo.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gciblxdyf.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmygxinj.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gdquvtsdp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcilbucay.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjpxucyv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/guqpozkcc.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdtdwapf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzmsxkdl.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gxpizbvyg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/grnbzdlti.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomczwsqu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/geimtvnew.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/guhgrwcru.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/grhgoocbg.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhwywlsv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrbsqksi.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gfrkfwggx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexrzlcod.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkfcttve.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjswblpgz.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gbsmtcwrd.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gespyubxv.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqthqdqr.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyobcmujp.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbbmyuik.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gcxlujweg.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gqjniupme.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gzbmdjkzb.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gfibuszht.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxbsbfmw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/grsoodusm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gikqyuvid.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggsgrlid.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gewoydkvg.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/glidbjoru.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gykgakjks.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gexmevbdv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gvzbgofuw.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfelhool.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjpifzhp.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuokykmz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gnwnoebio.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzpdfdtv.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdfzmrkyk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaxrtsgr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaiukjdj.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/grzjztztl.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvxnjdiaq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjgzzwjt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/guwpzpsol.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gjzecnuvi.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gklzblhme.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gevuqblne.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbplyfbq.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymxxqilj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gudnjrpdm.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gvtqptcwu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gsckegboh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnrvaezs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gnisrnjfo.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gmalxotpk.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gbgfrawxr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbwekpen.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/goiwhrmfb.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gpyxlgiow.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/ghffobjyu.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlnlehxl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gxzzojbdq.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gfhpyafjo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/ginjxiwjd.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gkcsgelxe.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfihdihm.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxydgzuly.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrecaejn.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gypvlnxsu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpuxmlopi.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/geitkexxf.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gciyhuhaj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gqakquzdb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpxrnkfk.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gekstexki.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzngrev.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gkwaaixua.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggurezreq.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gohebauci.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gdfejfbke.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrmwpjok.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/guflvsgkp.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdllwxshm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyxzajna.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpclwoum.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdrwjkfd.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gdcprfxyx.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeeouqtm.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godegfcqp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gitkdykmr.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gvrlrrfob.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/glygisqus.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gcibebicl.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxuwuqm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/getmucijm.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxigxmshq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyweuvivk.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezviuxwp.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/ghxidqnwm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkhufrjrn.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixapnyaw.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtydzkpix.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gcplbvdus.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gkyclqphr.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gejxnbwau.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgreblft.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcoptuoyn.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwfdgqsq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkpljniu.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkyhimoj.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gyirsjrpy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gfhjwixhb.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gbdciunys.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gxujgpmeb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaxgeqau.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gyzvjzohl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuhmlurl.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyotmkch.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtorcsjrk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwonkgkjn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gisuvaemf.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlnaxhdc.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgocifgk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqwznbpt.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/grvnophpr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytuwgzij.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmtfkdsu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gycdajrrw.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmsoxqte.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpnnkkvxd.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymgrmkok.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gayaeavan.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaswesko.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfdxtvcz.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjvfemonu.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlilqabn.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gshfzgkqj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilxsxqzk.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/guyjnpudu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcozmpglc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqnmaibn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbvszizv.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqjuspnnp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gjfnbxpbz.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gmxizbcag.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgamgsaj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgzaaupz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuhwlkuz.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/goisjdwuf.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdtlrgph.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyouvaen.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqcklnid.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnieevmwf.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gflmriqow.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyaxzaaj.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gyzdvlrcc.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyeqfyvv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gibhaesoc.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/ginnedlwp.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gklfoabzx.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gqsyzxccc.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjfzvslc.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtyjyjtzh.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjucbgugm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxidmyldm.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbhebmov.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/giigzigui.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/geffsporo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttzzgetd.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfwgbao.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtqkpwlhi.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gitsmeqix.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiyncpje.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqjonfeo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeayxqjm.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/ggxtnaugn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsprteruz.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfgzdupyl.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gzxotmmjs.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gclwmbkdd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszyaskot.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvmpuegpz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvkmhygte.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glnqikzyj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gupmocofc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gilmnkbtf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gofpsozwn.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjfjhdft.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gwutsgwtx.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtckzuhj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwddnxhv.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gvuxuusre.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcqplqya.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gpelxzmmk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfdthqox.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxmcnsv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvgylbvu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghfdzeqq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/grzmtkpcl.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfrtetro.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/guwumqkot.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/ggvgouvji.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/guamihzib.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpsuaocm.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvysqpr.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghropzsmx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gfylxntap.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyitvjaey.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gzcgqbenh.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/glytheqwt.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gpidlehws.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfyhynyx.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gebtnjbqs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxwsmqtj.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoxxqypy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gznmavjvf.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyinedcfl.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gexmkswtr.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gyarjniqd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gawuzzqru.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdaqcxpq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucubdma.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grdycoykp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grugxhoqp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcokzlfic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gpqpzxkot.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grmqqmppl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giinmvvrk.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gnsygsgmn.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfpxxqlj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnkfyxyy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gpotgwllc.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjifeidx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/ginfzpcrn.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcwiqcpb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcdarbpk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgclixme.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkceyivxn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpsndxau.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvnwpgmd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gploerwbt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gggjphrtw.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gymvhwunt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwhqbsrn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gnpbgctco.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbrxudpj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gpznimvki.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gpquyuwgq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gzxvblbyg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gzeprkgrl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhbeebee.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gwaoqihxa.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwtrvual.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwgfkuxb.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ghkybhjeg.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gozhsabjr.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmacighcz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdgkofwu.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxaxetir.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxlecicf.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaspkofd.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gnhywiqdg.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gbjztpnas.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gdunzkllb.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxeezuuls.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gztwvfgej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gldusabia.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gblxpworz.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmrvuyqn.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtazcqees.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ganacmbba.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxownhxt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/grkkdqjpf.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gugjkotsu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvurzwpdk.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/ggjseshno.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/guzsbeqei.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/glhtcikwb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmchegzey.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwzyiejin.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glebjrjbj.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfwtbqb.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gmfaqknve.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxoezdem.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvceoobua.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gzpnzkjiv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbntakcn.sHtML


<!-- 参考信息 -->