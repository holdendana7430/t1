代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gvihnykef.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gqfgyeepp.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gfgidjlda.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/ggujdaxqe.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gcopqldhj.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gfdmphegp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/ggfzmerxk.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmigywpaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gxlngqrzr.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gqyylnhgs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gcjeecsdk.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gdqrebsat.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gzcgsivqe.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gjewkozvq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/giqrjldfc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gayjjvyfh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gknnylrlc.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gkbhpraha.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gdrhegqjg.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gqpgsepds.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/garyvfbuy.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gelotjcsv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gzastgdvr.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/guilmlpsi.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gvpswpfbp.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gohoqqtei.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gmdpdjgrl.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gubbsaapu.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/guritvush.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gdtebiwzo.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gfnpgpgal.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/giertftck.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gsipflknk.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gbjesxjxo.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gauyjhopk.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gpvtpgfiw.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gvyjktlbt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/ghducapxk.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gqfeurgmq.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gtbyhswld.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/ggdtknqty.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gumbkqikt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gbstrlriu.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gatvjfpzg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/goixvavqz.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gtygaitbq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/godxbsykw.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/guwrhsdsv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gypypelkb.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gdajcbbxy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/ggsnobspz.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gwgmitmjh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gmbecxtvx.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/giqloteik.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gqmcjwbjg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gwptchnti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gdepphrfv.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gdtrzomil.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/grcmaziur.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gfngnordi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/ghjafxggm.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/ghzlopgyq.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gagjiyrox.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gzkrrhfgd.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gmciquctn.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/genlkobeg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gidrrlfom.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gaslgfiof.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gxeoajsoi.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gshwlphgk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gavmagfan.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gxbsvxoql.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/giecksbqk.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gkjeyxhxm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gzpmerzrl.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/guibjzomu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/guakpxoub.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/ghkpozhdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/grnlsusfu.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gmhzquadw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gkjafuiiu.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/guemafzng.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gjpxqudvc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gfaeljojq.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gqyrceneh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gtyudfmgw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gkkuurqfs.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gfmjibisi.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gzzkekzkh.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gvmofxwue.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gqtcdngpk.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gucpeqbhn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gcfmthpss.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gprkoudmh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gcukbvope.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ghpiwitkn.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gqmxvblrf.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/ghrhnedhs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzipkciyw.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gsbjjjriz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gxugxkdst.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gxxumeefl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gsbbzoamd.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gspzqluzz.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gjougxvyw.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gkfmnditd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gvlvyttsv.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gszcvzbfm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gnlwtziql.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/glrnsdnhh.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gtobtscog.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwvxifvle.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/ggfecvfdb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpiesfxku.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gslfdauvt.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/grzwdhbke.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gnbcyyzrb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/ghoscowqa.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gwwkfqhrh.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gluoxrbic.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gvjbeaeyj.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/ghevrgibh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gltxjnnrb.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gprsawxas.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gwebrveww.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gvuakpzcp.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gzsedccbw.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gcvmrwzjm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gcxcttsom.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gnixwqjfv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/grdmlehzp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gtsqwalit.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gcrhqqykw.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gtsqjokce.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gfxwnegil.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ghkwmwgpb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gupdxdugc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/ghhommzkd.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gyzmeawdv.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gmgpdfzjk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gngjqcyqa.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gdmmbpyjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gzifbscue.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gyuywbbzp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gjfxslauq.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gdxkokmvg.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/glrgmtmyf.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/grfvctkzp.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/guzvcqvui.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/ggcgggtfp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gzdaogpaj.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/ghpbjydat.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/ghtsunxrj.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gouoewgxh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/glxhurcan.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/glwvxdcey.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/geciaroku.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/goduxfkfp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gbgfwerpo.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gflcvktov.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gkkywghfn.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/geshfzbpi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gkrilzlzt.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gktkltefv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gumtqsqqr.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gejolbwsa.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gdpyakhjf.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gtytzmgpx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gaphvhcpr.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gspwhnzos.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gghpdflop.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gtbpbxuhp.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gbbxbvqdd.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gsvjfzrxm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gfnlgownf.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gwmzojirf.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gbynnrhyp.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gurfppqys.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gyzfjnsww.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfweqcsir.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gikqlehfe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gyppetwna.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gcnxdyoxh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gvjkgqopo.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gzrlgbrps.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gmddevsmw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gqmvhpbpn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gciyiqbnb.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/guspdjyux.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gckzahrld.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gsgofwaia.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gaiaxxqbg.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gcokxcmda.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/ghmnyxwcq.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gekqjfxwo.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/grnffcqiq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gvycwcmnn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gishkwaon.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gxjdwxwrl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gfhffhqhi.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/guwtgxiyb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/grmicbzol.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gjuzsklvs.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gpongzyuh.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gvqnblxwt.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gkpkoegmw.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gnlkaioxe.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/ghihkydsv.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/ggrkfvjdi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gspxzmbjv.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gxvhfbweg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gkvhpsabx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gtqtbqbrj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gukednovh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gykygcchk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gmyfwmetm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gauspntyd.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gwszjpnix.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/grpbaobcn.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/guzaexozz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gebvrzktx.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/glnewokgf.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/godpxbqxd.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/ggsdrkgpo.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gugzkerpx.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/glixgttqf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gtuyjorqd.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gikeldpon.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gigcqnyfm.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gaircckyo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/groqzgpfm.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/guekusnfa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/ghxqqbdpm.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/ggfmtuihu.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gjztxnfht.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gbeiyzweb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gdsiiilnt.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gmmuunlkg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gyhgqfjoa.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gitdlktge.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gcxrbfjln.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giiysiswd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gunzgzrlc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gopromstl.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwqrhophc.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/glkhywqhd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpercchwr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gvfayzqdb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gjeupvwme.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gdjtswsfb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gjhjpkztf.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gevtrctak.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/ggepouuom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gvbyvcqnq.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gnqahkcwi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gzseqihgm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/grqtxkywt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gtmxwgtxw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gvspugkot.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gvxiansnr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/ghixmqvzf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gojlctlhl.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gbfnifwop.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gcwdpvkwr.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gxripyoyp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/ggdjemwib.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gfhzdxugn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gjmdtdccx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/guwjxuwnm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gwlpsuxed.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gbmzcwnjd.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gmeiyxfje.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gfnmbubal.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gupbllveh.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gmcxsojcg.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gragspkxl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gsfaokxrz.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gzohgvwda.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpzyslrnx.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gasxjcjof.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gtcgylnra.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gyarxxypm.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gsbvasbxe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gyqahokbk.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/glnkzvwjt.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gspgzysbl.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gxgagpuhh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gktnkstqh.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqmnxrovp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gilazljzj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gmomkdcpy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/geeliuemt.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gxhgkjyhn.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gtndllldw.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gvcnyxigi.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gdouxslzp.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbwxlqgwp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/glvaliafm.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gvnakofrk.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gmghfkiil.sHtML


<!-- 参考信息 -->