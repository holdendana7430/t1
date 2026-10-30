代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqbtrpmd.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojxvlrwd.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gnyhijrgp.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxodlgov.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gxjfippvy.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gdwmxmwwc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gzvoxsbrz.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrljrqyy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkjwxbcf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyduvblg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gstyxwqrb.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdkjftfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gieblfkto.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gssymtfwt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpanjosh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsepmbnp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gbunyqfni.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrqrtygj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gotrgyaaq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqegphop.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gtlpqcvcu.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gscvjiktf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gerdwrqmn.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbksusdtd.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdgledal.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaailvqce.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdqzrdbsx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/garyhndgn.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gfohejycx.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gipircmvf.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gjsflzwjs.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/goinealpa.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/ggdodoeaf.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeglrhqm.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqhipicw.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxqfjqxbj.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grwquarvp.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvllckndk.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjaoabst.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gmmcqlvmn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfeqcgss.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gnhxzrjut.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gufjqojnw.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gacawlvrq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwjmmmbjp.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmryxwgbn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweszslbh.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjxbdqji.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gpzkmgxbl.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gauzznsoe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gimtlpqlk.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gqclugeif.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntsmfcud.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzjgicvs.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glrokresh.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gmibiqybs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoiradog.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqspnjku.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaalilbap.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guooumxte.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnjwdgwe.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gssnausdl.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gqxktbphg.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexilvhjk.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gxisuvuts.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyybiwcst.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/ggssgcalf.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gtbitkpmo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/glhxlwkru.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/goejlnzwx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gknvvczjm.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gdqdguvsn.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmlmwhqs.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfccrqdhj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvijjjto.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gyxsvpuud.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gyywrmkmu.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/guqfenxyb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gerxtuuqm.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpiwdkvi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gmfydfsgp.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gskjibxwh.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqehiowqw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gyiewkiac.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/guggayuoj.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwhaofvys.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gcwtyrqos.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrvlpmng.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/glwbkesjg.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gpswjheqs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklmwbeir.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gsgotizky.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/goqgdixbw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqfildh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gezhjours.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvaewkrke.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfekrosv.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gdmuudpmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxwajjnw.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwwpswaw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gsmrmuprc.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsezrmccz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtjfpfyp.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbosbgjj.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gdeaneezr.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gxikophsd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfiffrpng.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqhzwge.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyjwecpy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfakabm.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gzscrncin.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfbwcoack.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gleldbnzc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guanqjnfx.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnopulmx.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsdrifbk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyqukecib.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/goefprtra.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gknfarjto.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gjuicifgh.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduwcfixj.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gsbaguflu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhudznvt.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/glhbbngsj.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaqyspbz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtzzymzu.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gstyoeupt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/glemrezuw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvopqsjq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkneeigl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseajvkwd.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gutcpvefu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gdpohvdxi.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsxpqsup.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqphugmf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmipslzd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrqmbyga.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwdiyssc.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbxeghn.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grcwqprvb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnuavjst.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwymuvmgi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwkosxyz.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gazzwsnma.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gtskpfcfk.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gsoqwbzlz.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/ghpfebmbe.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosdgsma.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gknqpbpfj.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhxpgrxd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdcbrvxjo.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoskifyn.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gduovapnw.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gziepjcmb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gpymasbvz.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrxdgcvl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggqokunyk.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/ganzguolw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gcrtxzqme.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmagwwnjr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdygpjer.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbpogcvx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkksuyiu.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwxcsrff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gakfhvobw.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gperjwsgs.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gzkcskijq.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gohtgkdkv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gqsjdzcux.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gacsjggms.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/geyvnzarb.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnvrzymr.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/grgbbwitj.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmilgtdve.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/golixdfxe.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaaitruhf.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtlinmpck.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqzuxqzd.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghawocvws.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyhqmxtq.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gneekbafs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclnpevkm.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjwzlozxz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gocohnfsf.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjydphvf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/galcfgnec.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/glsnizogv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhhrezgq.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gltovgcck.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjlkyhymv.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gmknfavoy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdunjfwia.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gownkjlou.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gumzgqnbk.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwjctsmv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoadftam.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvigkyufa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnoorbun.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkqjaelem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gedbjhxny.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/ginceqswr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbyppmsa.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzyalatih.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoywvrfl.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gmlfeanwn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyqsfvfo.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdbttfd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxpznlrh.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrvigwwq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/glfsadeag.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gmanzhtvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzlzmyxu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqybryai.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrbtodrb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeyzgrgf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozeqgxif.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/grgdknqsq.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghjsogxid.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaihzvsp.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/grudqmgdb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glntpfvip.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaxkbatoh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gtpmiesme.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gbctbakxc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgdinsjo.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gkfubbccj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvbtlhic.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknysyzqo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gipmbxypq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gbdjasnzu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gsxhkvhst.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/grccayrev.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjasgykkk.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdomskdz.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/glmxindjo.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxksynnj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffetpltj.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvveeejm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gcpldumqm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/godddwkdg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjpgrmei.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geuacgaob.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgowtodj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkrwrxqj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcfgyjwlb.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghblynpti.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhwvlpco.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcacwyti.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidrxcwfe.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gpqrhfirt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxowtofpo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/ganzbtpzf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gfefrhyud.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpprnnvg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gimmuhvsv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyciwztf.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gfubwcqwr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtsplnnpz.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfylbhi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrwqfbpa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpabuqj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmpkfjen.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbzfwnrru.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/ggdokxkct.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gtvafklsz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gykbgnsww.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrcjqmko.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkviyadjq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goweyxykj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiqmmhey.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkrlfnox.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gtrosymsb.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gujuxwydq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gslcefzws.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdseqcg.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspqiqntx.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gctjhqnky.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchdrihtv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrqmnsko.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyssrzlkk.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gnaqnbzeu.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabepyeb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimzdueom.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcoycset.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gzitovgqt.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnopuogym.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gydalgpvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/goinghgpx.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcqgmize.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gbrjlysut.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfbiipd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gnxleomnp.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtryxpmlw.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnnzekkp.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gshnxubds.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gupmtmrri.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjoklkrd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gvlqyytom.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gfczhwcrk.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gwrwozoet.sHtML


<!-- 参考信息 -->