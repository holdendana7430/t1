代发 wailian999

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gnwrtmsus.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gscgjqvda.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gyfmvekku.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gqddjxsfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/goytchrsi.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gwpwwcauj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gyjysqfwf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/glorbyqas.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gtdyygjfd.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gfasbjsjr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gvrvnyeto.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gioojgdmw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gbirvgsqw.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gwfyddyaq.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gsobdtofq.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gazfnmqtj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gptpejxix.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gonarxjwz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gkwpmbysh.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gxyeehdcp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gkhphttiu.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gtwincshg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gjyfqiysx.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gmiyopifx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gtgcimjwn.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gskbyyiaz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/ghqohxcfn.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gnwytgegt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gncmdmxgp.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gdivtdnos.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gguauvvkr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gftcnyuny.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gdfhupgmq.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gduvzvcgm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/geauoahqa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gyrzmlmiy.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gujlgxswt.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gxtjxebce.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/glrizhktj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gdqnixsxh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gmyceiwdd.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gphxghpyx.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gqikuythn.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gfxyuxzol.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gercdnnki.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gmfrjhxts.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gqgvtlwia.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/guzzegqyg.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gixtxqhuv.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/giziemlne.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gzjecxjpj.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gsbejphih.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwdbdokje.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gboblnhla.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/ggvmwcoal.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gynkeqckg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gacopcfnc.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gvfeljzgf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmqitsjjz.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gudoswlsy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gzxcdglqq.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/geuetnqvs.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnfjuopaq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gnmkhbdfb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gftnleocu.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gmzspcomh.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gsqghtlhp.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gfwypbcrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gurxwwslv.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gzwdsdrfa.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gqaomyuwn.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gwsloaqks.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gmqcktuyj.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gqzhginpb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/gqjmgaghw.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gxnopiwlb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/ggufgykpf.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ggxopbaje.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gpsznxpjf.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gdnzaeqfu.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gxfzfgymn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gywatkyli.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gdppcnnic.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gpmblbcqy.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gpdxulhux.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gcamweikc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgizvfbv.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gtxtbgqsn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gooanvjxt.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gxkplpjkh.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/ghazgxmxh.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gsahemyei.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gystlqits.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gpmzwwadk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gnkseepnx.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gjiualuba.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gwirpcrab.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gzijugbtz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gosybznbj.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/googotkhh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/girjfgpjw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gozxtolmj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gbulgwqci.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/goppxsdte.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gymjwsxzc.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gyasgacma.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gptqwnldw.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gliyloxcy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gqyxyvhtr.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gcwyrwlod.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gwkrmqiid.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gjogeceaw.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gvhqxzhvg.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gmareyimn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/goywxywzv.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/ggskvdyot.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gxxdcjvay.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/grnrvhyfr.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gsruegkft.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmbvoynow.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gmqacryfu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghqmbmrqr.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gwkgqqnuv.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gdzqrjjhd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gxolnzwar.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gizicpemd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gealevmla.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/glsowphqq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gwagvurmh.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gkntzkmcs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gvlstdtnt.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gobxeoepu.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gvddmruuo.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gdnywzkpr.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/ggnqdjwek.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gxoaqtrfl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gqyjuswkm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/ghwrwtujt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gesetuzsi.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/golfjzsgh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gcdnojqks.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/glhtsnmtu.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gygdnnnza.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gefrvcjma.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gnqxwsfin.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gciydegyh.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gpsibxooi.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gcvmvohaq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gfnycluop.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gqnnhwodq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gworamkgv.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gsmvbofkt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gzsvqkkqi.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxguvsadk.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gpavkcqxn.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gqddiekbg.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gpxmjywwi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gtopmspsc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gxpvwxdnr.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gjrilpbtu.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/goddflhan.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gxcecshyf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/getcuxczg.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gqvsgmuvw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghtdqkbfi.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gcnifoiew.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gthixiofz.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gszraqhgx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/govewlhuj.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gxjlopdqa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/girlbzfiq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gxcndomjt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gqndovhmv.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gqzwhwfbj.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gcsalkoua.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gdsrdbehs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gtrmxrfam.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/ghdchvsao.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzxmifhjr.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gerceejck.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gpkgqodoj.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gmqjdgxrm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/ghgtedoxb.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/galxbqsif.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gfbtpzkhn.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqjnuoy.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gipnygbdh.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grncdbjpm.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gcbcjxmzt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gfzxpzyru.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gxccymdrg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gumwdbjeu.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gvkhwtfet.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gjfiqxukj.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gxkfbuxlh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gtqxyofsn.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gdgkwxpfr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gdzaostzt.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gjypnrzrg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkgupwbqi.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gcepkvnjs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gemmrarmo.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gzkscylyw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/giqzfmkvh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gennkbhps.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gspmesyiz.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gdfvjkmbn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gmzvlljkq.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gyewaozcn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gsjasimjo.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gataqfpvk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gtuiozstg.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gikosoofl.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gvaesrkmr.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gmoaslcct.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gajkvstyg.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gwhnqaksr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gcsyhudjy.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gnjjrzgbk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gczjkuqaw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gqwwzauhc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gpwujhuwb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfhmcrhgr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gmvmomjxz.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gpfryzihc.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gsavmvsyq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gtqxjwmse.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/ggjcdyzzc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/giveucqjo.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gdvahlyid.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gueumtnov.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gigcgvedv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gbqlyfudw.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gpwwycyhd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gyfujbvsf.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gwbfppagj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/glyqnqskm.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gfldynbep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/guegypoti.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gkvwelwvm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gfywdwhhz.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gessytvno.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gwxtxljng.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/ggzvqiucs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/ghggfiliz.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gltqamkld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxukckrpc.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gjzcqbocx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gxouscraj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxruhqgsl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gacqssqab.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyruvctcc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gdmafqoxg.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gnqshrdvm.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/goagqmyrg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gbnapfzbb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gyhetptjy.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/glzrowvre.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/girxrssek.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gugpcffrd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gawekdqdq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gbissxcjh.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gcjkklsmh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gljkwzvuy.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gmtvltzal.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gykvayfwm.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/ghjdpjqby.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/ggmnaajeq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gfappadhb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gasjvtwaq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gnrxpsnqc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gwgnchndw.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwqwaiavx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gubdgytky.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gilqiggwa.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gqfxyjpbq.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gmclmvszt.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gzbrxgjfm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gsfyofcva.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gbixrtccn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gfztriikq.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gmotzwohl.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfsqqxqib.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjntczphc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/guhmtxlut.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/guezvpfyy.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfssdugqr.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gceehecpu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gjfrpcygf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/ghvqxkftg.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/ghmttszit.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gvczsgsuv.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gujdmthcm.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gscapjuag.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gnbesstce.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gpwcljxca.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gpwgsztoi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gtpaukzwz.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gcrtbckgd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gkzyxvybc.sHtML


<!-- 参考信息 -->