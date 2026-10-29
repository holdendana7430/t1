代发 wailian999

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/glhyojmjf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gulggowpw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsmuhkf.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gpzzeakba.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gmadxpfho.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gljblawio.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gnvyukbzs.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gaubjkynx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gpnnbegyy.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gkrjvzqrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gdvhcnemp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gngbouact.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqtruboda.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gemveabdu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gzsfqjwdc.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gtrrxrdmf.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/glhblbyel.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gcauezcnn.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gogwnvqmj.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gqrqbtsmo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjrkcqxcr.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/godphjvoj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gdbtkitwy.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gmgbrzcoj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gcuywqytc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gqsyegkiz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvzugfeqp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/giijjdoyj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gotvvtlsl.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gutcwxokb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gymnignmk.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gchawfkjq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gmnsneuqq.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gyswpkhcw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gzprfreao.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gofifmang.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gbnwnnuja.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gaorisnza.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/geunppdai.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gmgfeqnam.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gxfamadho.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gtxqoityg.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gkwkjcwge.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gfpdhhfgc.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gkegspcdb.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/goicujbim.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnlvcwkdu.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gvsbwkbso.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gtfhkhihs.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gzjueawsx.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gixkmqjrn.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gjnrlqyek.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gftzzgnhs.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gbhhpifoa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/giuuwodlp.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gnjjhhzwm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gqhrrcjdd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gvxvtygpk.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/goejpgywj.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/goilfvule.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/getdxdlio.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/geekkgxog.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtqqboheh.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gtkhmdxtm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gsrtoipth.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gnbqcqdwo.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzfmudmct.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gupmxxvzw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gujgmmcyv.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/ggxpchmly.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/ghohkkqlw.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/glvyfveyk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/griqmuoju.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/guqjhgcwv.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gkwvrbiik.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gekigujpi.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gtabbxnss.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/grstjmvdc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gjkvtksbf.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gqkhntybe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gobfezngt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gnxadxotv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gcpfvmesu.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gxsabxdqq.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gtfdshqyl.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gagctpyzy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gfdzvduhp.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gtzowdkmb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/geienazgc.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gglkciiwb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gdbspuctw.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gvlcjkugi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gocdfkcpz.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gpymiorhe.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gaxvcobov.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/grcfioshs.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gpwdokggd.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gvdlhnemt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gmpupoccw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gjfjjfbtj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gboalqkon.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gbbzickhj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/ggunmudak.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghccwodpq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gxzxiprah.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gzntwfvpr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/ghsywqcmm.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gvdccupcr.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gzatpxtax.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gjhlbenua.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/giapkxzie.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gjdeeasxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/garegooij.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/ggwotsyhl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gaogjqwkp.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gefhkchdr.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gwoacyfah.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gtahtfuly.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gzuddimun.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gzvujgfln.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gtjqvmdyd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/glnldowpb.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gkyhplmym.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geitflotb.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gfhkouvfi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpjddebpi.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gyaqbnssn.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gddfbuefl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gjyyxisox.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gmkfrmryz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gryplqrmc.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gcnbvdsxp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvulxjxgs.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gjrlbjsih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/ghfstwydt.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/godcsgyyq.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/glgqqticw.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gnwxzvbgl.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gdetihmcs.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gpvquwvwu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gvnrszwpv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gtpmpqvcc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gmcwcvmgd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/guqkzijlo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gvdbaovze.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/ggyhxrlmv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gitxloghq.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggsvsrblz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gxjlrbbbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/giuihxhar.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gmpxgvkxe.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gkgttqifp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gokjsgela.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/ghbdjqpdo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/guzefonou.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/grhblhnjx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gvnyondyh.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/ghflnzkau.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/ggxjmmuqq.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gxfwribkv.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gnzcswvhw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbsyzwzcm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gbugllszm.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gqzcqwqwb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gridxqfte.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gchanzctd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/girqbuemz.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gjtxaiowp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/goanswajx.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gcjdianhv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gxyjntnfl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gveangilr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gnyjxkfrq.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gmersemdf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gqnjythhz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/groxailqt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gykicbhvq.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gllftcofe.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gewaggtoj.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gcjbvhybt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gjmdamjiw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gyvudyasu.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gquuomeks.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gbvpreklb.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gkzjdbphx.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gerrzajip.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gzpdxrpos.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gpequtcqx.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/ghxhfgkey.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gnfqyatnx.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gmqbwulnk.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/giesurbpd.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gouscyybi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gzhxnzfkm.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gzcujrgey.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gczfoufwq.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/godgqmyei.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gzgglnrxa.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/ghopbepln.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gxsbjnkhf.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gndtvhkrv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/geewupwvx.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gsgghfgzr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxjzfiels.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gqcgvonve.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/ggkbwizdd.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gbscfdmvf.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gsleyfvfd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gffyvqrll.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gwrcroiqk.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/glebrbqfa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtqosmxsm.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gwfhmyffl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/guingwcdh.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gomsrnqjj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gvhnseklg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/ghiuaeaei.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/glgushaxk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjrisct.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gqkbxinhz.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gsqudahfu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gpxjonusa.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/glqekqpvg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gpceplioh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gmyuflgjn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gaiexslmd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gyzebzxqd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gjedcyium.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdjhmwxrn.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gwqujcfuu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gerpbdkho.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/grtsjldfq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gnnkaruju.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gjptgtgje.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gllgmffsa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gdmshoccs.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxblqdrx.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gizkyripx.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gdhenzlmx.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/graqbghoz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gpczfzkzc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gbgvhfdyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gzcntswda.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gueckartb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gdbhcadzw.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gmqtccwih.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gwxuyawqx.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gysuhgvii.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gmdbcaxmy.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gxexzbuwq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gzqtmfzkp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gqkvcegtx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gpqabiuue.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcogwcjso.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gfmufvuqj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gewrokgjy.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggyyxzaub.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gxhczzfyz.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/ggmtdgwsp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gxzzgiaqh.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gvsxqkjcs.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gqtnhrrcx.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gupacbeqj.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gtukqiquj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gfibkpnvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/grpqehvnf.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gimttuvqj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gsrrqdhti.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/grcpvkmda.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gbbsbnjwa.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gqzpgjcun.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gvynzyrol.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gkpnbnnlx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gnczkkyyh.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gijhxrvgz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gwmyglrxc.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/grfohyhhx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gclesthrl.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gwzisirjl.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gyzrhjtvf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gpgsjwekz.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gwgyayygg.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gomppevnm.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gkfnkhfcf.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gjycafsfd.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gfoihzrvr.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gamkcstqj.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwlvfwqim.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gtmhmephj.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gyrwbhqfk.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/grlmgezbt.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/ggijlqtwa.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/glrfxexte.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/ghcaiuuvk.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gclsiakfn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gdcsxnjiw.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gmlhmiuyu.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghzsezgcm.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/glvxyneck.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gqfcpfliw.sHtML


<!-- 参考信息 -->