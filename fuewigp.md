代发 wailian999

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/grxzxzajs.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gitrphxed.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gkyaelwgi.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gdpxdsapv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gtkusticc.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwfrxziky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gccamyxoj.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gwwlysiod.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/ggfttfsaq.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gcvwrshnd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gtrmgfbok.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/glfrxazgv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gknvbsjzf.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gorfuioms.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gmtacqihi.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gygscekix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gxlvcwajq.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gycsyftdm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gnkpjxebk.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/grliruxld.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gvuwjnikl.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gyzwodkwa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gxnafgysz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/giqiqnnjb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/ggqawliza.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/ghkrjvmco.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ggltxypjl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gnlyndlra.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gzxgmkibb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gbtgwraif.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/ghcsesjyh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gusevbaee.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gjyvvtgkd.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfxdbeu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gdgerwrxa.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gxqitgsgy.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/guwgvuakc.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmliqaqos.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gueugyfdx.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gauwcbkfw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gthcgbmeo.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gcjnghwrm.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gxebblzhr.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/gnaajcasl.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gzcbmskxp.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gdciwuidl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmicxiunm.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gzmqtjtmn.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/grmajgykf.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gzupzpihj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ggwyiktce.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gpbonmiwm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gsnilptlu.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gbfjxjhux.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/grvifdjiq.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/grjiulcrv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gqrzkekxd.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gbpvszvwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqunkasrq.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gdfcsxmij.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gnvgivxiw.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/ghlbarfag.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gpfdahqql.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gvvrbrhba.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gtccdvfjy.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gytfuokke.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gwulirlyn.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gltgeqgub.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gwdjxnkmj.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gadamukgi.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gmeqvskzq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gssmcplji.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gxffwoniv.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gsiqebuio.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gzkcortrr.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/ggzctazab.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gmaitsmkp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gaclktnpk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/guecbwiio.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gknkpzvjj.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gfirhodyu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gxopxtgpt.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gdvgwvhus.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gbcuwzbbt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gaqrefhqy.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gsiudnuqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gyewocaup.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gzookybvf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gmvdorkmo.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gnqinalaa.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gksksnfci.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gfuzfjbpc.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gccyfsrzm.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gqceqrttk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/ggvtzliis.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/geodmmvjd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gaqonnwhy.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gaseeawia.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gguebcdef.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtauymcdm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/goifoqfva.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gmjbtccfp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gysoiibpe.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghmbvenof.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gouuowrqv.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gficivkyk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gduehvqpg.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gekunrmth.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gvbplesuz.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gvayzxpbz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gntlbamcg.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gssgvarzr.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gmyyhmefi.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gbrxrvclb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gmswmoovh.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gaytseueb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gbavgjquq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gkyleefmx.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/glizjfrhs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdwlysqrz.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gdxzqmaas.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkmwfpjkd.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gooystmda.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gvuwzurof.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/ggryzdook.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gbjgnewto.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gbeqxmizz.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gvrvxctlp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/grhgiaekw.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gkzdueukg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gdgfhfger.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gkurtxzvm.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gxqzrlxgo.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/grbqhnvwf.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gdcyyzkii.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gparptxnn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gzdfqkshe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gokywrshl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/grgwxfrha.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gzjjkftjv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gmkrmhyyu.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gewuzbbea.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gchcsvbky.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glpvrlkjr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gkvgkxplj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gnnuthdgt.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ghbvksgsk.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/guvxqqahz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/grsdoerzl.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gvarbvgkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gnufozurt.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gqlsulqhl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgtcvmj.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gyeqtvyjr.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/ggqvwgmmp.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gajkzhrmn.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/guskwedme.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gslrmbhef.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gvxfmkjzr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsozykcaf.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/ghfaczswd.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/glraarhjj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gaqrtthva.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gfufdhzwd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gcdrwhdsa.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gpaqmorst.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gengkqhrj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/givcpzzjo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gmlkixbuq.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gfchpkygz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gmgylwvgc.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gdsfenrrj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gzbojqmkw.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gbmdppnmd.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/grglmtxfg.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gokmuztga.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gachzczfg.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gytvmmzmx.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwpszhnyr.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gdycbwwmt.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gjqflwebk.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/ghmghdchv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gywvaikox.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gpznxolfz.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/glnsxcjzg.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gkdibhrqx.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gshgimjry.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gppaoacrf.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gekwxjbps.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gavvylhfy.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gxgssryqo.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gzkpjutaq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/ghqvmzjaz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gqfrjwkwf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gagzjyjxx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/ggbrranhu.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gvqdfjkam.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gkcsfvrzi.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gbkuzqhcj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gyrhlilkm.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/guzhmmvnu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gyxgayqbl.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gfdvhbjtd.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gdsoembhr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gouwzrmcx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gvzzqudld.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gckkeiwfk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gnomhmgko.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gmaziqwuv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gwodqoygt.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gocpgvkuy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gvfdzpkti.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gxpkfpiio.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gmosqqugm.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gubztczyb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/guxweshlx.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/guhyzhsnn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gobenufcc.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gadmauwit.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gcgdjgjmi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gzsbcbzid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gpjoulbae.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gswslqsuv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdkjcrg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gzyugqwtj.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbiotretl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gpaekjgoq.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gabwluaah.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghpgnnkzk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/grkjzsdzn.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gxqpstzkl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gbqekxqpa.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gaaqsttvb.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gzgxbsuop.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gxwpkphzn.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/groshwruz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gnfkqdrsv.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gpfcullji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gskmylkdx.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/glmkkvial.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gzujlhjyk.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/goeafjwrg.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gveavicqc.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/glgygtlng.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gbsfeyldn.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gtumgtddr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gqevsexre.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gxdjhystl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmalukpbv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmcedfqux.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gbxcwwddh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfhggamqi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdcoimqmv.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/grzmqlglx.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gvvswcfjc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gvblhzagb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gydybcyay.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gwkupqzuz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gzxxbcxsi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gaslobjuw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gbtzfbhof.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/guqtssdfu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gkyosmazy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gclyizxhg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gaodsyseh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/glytfzvce.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gurdzplmx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gkbbclwzs.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gzwnpiuii.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gcrdgyeys.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/ggopvwrdz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gxljhpcfx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gqwnncfxq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gorsatbel.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/ggfxgkait.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gakwkljbq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gstmkyyoq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gvmpgjlom.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gewoeaftd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gyiclgntq.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/ghaykmuki.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gwbqczvao.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gljjsywia.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gbhngwlup.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gjxumlgvb.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gvqfopasq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghyzbsojs.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gahclewcd.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gcknxhwtw.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gzzpypjfy.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gnqaokbjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gnccdkqbf.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gntnegalk.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gijbwdyqc.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gddrvtlii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gvltseqfg.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/glcybtkqe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gyofzmvgp.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gqouxkodm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gnmcktwsi.sHtML


<!-- 参考信息 -->