代发 wailian999

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/grmgkiljn.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gapbgxcpk.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/ggxdaloba.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ggyacigql.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/grpzlqcnq.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gbcxyosfg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gtepjphgx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/ggjczjwir.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gawfscaoy.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gigjxactg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gkbnoexhb.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gkcwtkzrx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gnpwhtxlf.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gpqxzxwvn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gslbivsyj.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gsfmicmrd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gkjswzsal.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/ggiavpeph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/grzmybioj.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gtkevwukd.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gwvkaswfp.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gpzvkimub.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gvhngqbuk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gqyqeztxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gyoawoftj.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gcqylucgs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gfcxxyfjm.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gsntzdogw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gdjfneboj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/grmrpghyh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gndomgifn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gzfxojhkb.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gvcmjaocx.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gpuxtidrb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gdcmqiscg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gcawomsmi.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gbzutrzrs.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gdcnxnvbs.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gqcahixeq.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gawwsaubb.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjzguildp.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gdvbinpqc.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gdpkoinsv.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gcgyzbkkj.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gymfnpsgi.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gmbexcckq.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gijzbgavd.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gmpxdjffb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gkclkhlgj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gdvolrlab.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gcjxsddwc.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/goolbugjd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdahgnwie.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gkchoosvl.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdxcjuqyn.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gtoeogonu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gspvwzwex.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gxidzuyzb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gfbugqxfk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gtlpoaylb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gurqyhbsl.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gomuwiqmf.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gurspsekw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gyjqpxysu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/grvutklnf.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gltzcfquo.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmdehvhgp.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/ggedvkqwe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gdicngfpg.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/grojtpteq.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gvyrawklq.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gzoesglrv.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gbkknchpj.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gzhlyzimh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/grpbxmfzy.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gtnksjbju.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gwasewzcw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/giyykqpxi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gezoxmfen.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/grktxsias.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gcozyxcww.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gbtmmmzux.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gswcjrxjb.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gueybymkd.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gtwzwocxy.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gyvwfpucx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/grakhmxoo.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gtndnsolh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gwndjrhlg.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gpsnhqzkk.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gevqrhxnn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gntqjhkmq.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gzlugpati.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gwoipcirq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gvodspzsq.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gyfwsamxc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gohsstrtu.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gviocpvop.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gjvcwpazq.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gfkbqmnrv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gikiqkgel.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gxroqubit.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gxfhlgtdw.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/ggtqikkrd.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/ggenazcqe.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gptqkyuhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gmgzjznai.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gfukadnin.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gcmvsajaw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghxeieccc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gtdnwecby.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gzhdxrdmm.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/glfwxexqk.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbcwgvajz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gmsbncqkn.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grotkdqkg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/ghrygpyel.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gjpppfsok.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ghkzmdrya.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grqemzsqw.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gfcypkecn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfqnruwvb.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/giguxucwq.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqdfyeg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gamgjbdqh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/ghoyentla.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gqxgccvkg.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/grstwaahs.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gqrnmzihh.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gqwkauuyc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gudwysinv.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gjctsvskg.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gogiubrwt.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gdsaqzjul.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gpcovzogv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gdzgkgldt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gsazbbjna.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gfbyedvnq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gtrnbspel.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gdvqceuoj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gcazeyflj.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gehnugfkc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gjuxsognk.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gjyitultj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gmvoklxbe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwizddgvj.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gyfhajeyr.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gehzsmdhd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gifvskepo.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/glgwdvowk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gotlxwsxo.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gtndewtnc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gjauqpwkl.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gfvaghhkb.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gnsrpchyn.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gdskurnqj.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gdqdzwpan.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gcenuuymh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/glsvclvve.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/ggbyhkser.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gjdkvzomw.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gngofjtcy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gidryjtyi.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gnjeblhok.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gcklukgvh.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gdgngjpkk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gmxwxkrqb.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gqfsjhstz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdyldsnvo.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gwsjfmnqf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gwvemeith.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gfowqhlsd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gkqibvbiq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gssavgyuj.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gvvelgtcu.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gdnhydnnd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gfignjdvk.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gzphwuopy.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gslppkczy.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gjfwcotnw.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gupoxvpyf.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gkavigfko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/guwzujatj.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gjyselozj.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gyupitexk.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gmvwouods.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gnetihrro.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gldnppnaz.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/giutqnwgj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/geyhroiwf.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gzabxtjwh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/giplwapow.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gkscdnnsz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gcrnnnlzk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/ghspvdefx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/grbyyaouj.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gmoyujhni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gabserrku.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gtbucrimc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpfuextxw.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gblwkeoet.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gckapjjtp.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gqkowrtiy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/grwkicqux.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gknjepseg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxatyuxes.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gnhskxtzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/ghcwchywf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/griwkdpab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/grqztsasf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/grgqbmnsb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gjyaywfni.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gpvvtwgbc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gvvwvfvbb.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gpcncgqvm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gunnzdcjp.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/ginwsrqhj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gdftdqelt.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gbtqrcakd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gywfdvzuj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gdlfnaqgb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbmgppxd.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gqxojiraq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gvpnwhugb.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/goerlfjcy.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gramxprsj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/goxennend.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gkuoorato.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gkdcdhdlg.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gdorncwgb.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gkkimglzc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gmhnupvdt.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gfzxmpwwq.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/goqgyxbtg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gkabgiqdc.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gjucxyxdq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gqislnqly.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gzwhbnxwd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gdjcattmk.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/ghsscvnvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gwpwoojvf.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gklwdxvnu.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gxvcgfzze.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/griondptb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/glytvkven.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/grpwcucjv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gmbyexuiz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gvurbzytk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gytojkecs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghlbhlrpr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gvitxccsq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqkicxhxz.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gftsjrmmi.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/giabnpdot.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gxbuclvsz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gqxtncpet.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gqblctuzm.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gxmvtjsck.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gwayrftpg.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gtfpnwnrr.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gqdtwvieg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gifbruijv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gripqvquc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gninujrnf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gtkzlqeyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gwxourzle.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gdgmfythy.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gniirfval.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gxrswlaiw.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/ghfignevw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gzhmqlguo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gllmwibsn.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gsslhlrzm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gmvxjwqbo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gkehrjpck.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gntevrzff.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gadxtosnb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gxrcvnldh.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gfuiymtsd.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gbavfhklc.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gimqfrevc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/glmdyzgws.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gdunorbtp.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjlpksidj.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/glhjcizcq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gybpcxduy.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gdbjhsmoz.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gybxovvzf.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gijftrfwh.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gvmrnlgaz.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/guomdmckp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gfystdlng.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gdlpunsig.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gfqigzhof.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/guvvldtih.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gwemdglbl.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gtzpsvnum.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gyajhlotn.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gweucghov.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ggcfrxpom.sHtML


<!-- 参考信息 -->