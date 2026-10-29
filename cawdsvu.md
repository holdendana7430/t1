代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gezhddqfi.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gbarjyvel.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gjxweerbu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/giottqkbu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gdiimirsl.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gumpszbcj.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gpvkelwmd.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gtqitqfpd.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gdqnheftg.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/grbkoqcqk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/ggkjmwpug.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gfjhgezvq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gexoopnjs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/givhjxouc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gvbswyyqw.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gudlnkbdl.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gtoauuhho.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gljhvwzir.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gdykzpdir.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/ghkfvzmqw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gpywxcwme.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gorzrwtai.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gygivtlyu.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gjtxzyqwy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gsflwpnie.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gelginpsf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gslgyysag.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/galyuitfu.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gkfkzkpyy.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/geujhkyfr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gebwhmysr.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gqofinvlv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gifxrutkc.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gaspmzsqh.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gdjwcsegv.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gnmgxxudd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gmqmhrnmx.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/grldxzjch.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gtytzxhyj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gfnnmifkm.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/ghhfuixvx.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gmllvjsmk.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gkynhpefw.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/goomjnkps.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gmonjhohy.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gplzffyjl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gcesuzkaf.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gzeqxuvwn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/grkimfosj.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gqkikihpf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/giqsulkzi.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gxwumvvga.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gtqfmibzc.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gogcanfhe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnsytrxpk.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gqzksgico.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gcinbmypp.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/guaxcerog.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gmuubfmqh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gohmznqni.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gbaeqoiqj.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gdnliminx.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnvqinotm.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/godfkdkee.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gcgxtbdzx.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gcepycryr.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gfupiexed.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gxfzalmtu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gngtjzwxa.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gjkjttpqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gcdgheaxd.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/grafgqrwx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/ggbiynbnt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gdqjvqenw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gqdmuofem.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gwucmwwdi.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gjdfmsqry.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gjrdirpvw.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ghtzlhyiq.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gfmqouikv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/goypjaeof.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gvqiyytwk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gzvdyvjak.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gpueorwnb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gstkxmchg.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gkumcbosu.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gneuemvtq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gudyakkam.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gffsvggrl.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gnozdoeto.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gworoeklx.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gxmmvaypf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gqegbkwiu.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gxcwnnvwp.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/glxzlhnoc.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gfhuvizop.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gmteckceh.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/grotnophx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gxgwrzoap.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gsvvsvgny.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gqnhjmgrr.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gcvguppai.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gglgwgbxs.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gswoqpoou.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gxislkons.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gjgbelsoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gfczrurmn.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gmeszpkcm.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/gquvkmkvl.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gyeeihjni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gchrzgdqo.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gyrdyohvd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gpioarndy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gprdkzbaq.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gyhxxlmmi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggczkjbht.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ggdtxikgo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guzwgkvdt.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghuogokth.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gvsjobliy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gcdacagfu.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gllgxejrj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gfbpwvmhc.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/ggiexprhx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/guumvhqbz.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gzgrhxhoh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gcrlwggvn.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gcpymvjxe.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/ggktxghgp.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gfxcvitzr.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/ghynvzsdm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gukteihde.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gfqolgqpn.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gmvspencc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gjznlsgzv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gectsjbya.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gbngwluov.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gmngtorux.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gbhbrjrwo.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gporvussi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/glybznzfr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gusnoseog.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gwwjzgufd.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gohuipysh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbfyyogev.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/giztefycx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gceqjsneh.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gcsninksw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gnsryqshi.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/glijmylpq.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gudoosdrr.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gllofutmt.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/geaokbmnz.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gptrhxmpm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gefnwoupt.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gcumyxfbc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gegbjgyix.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gpokenovr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gprrekmto.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gyktqohoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gckpkmabn.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gykdfggdw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/glkuvzado.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gzyzueiyp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gukxpsygu.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gpbvrbxzl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gcdbhupbo.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/genfmubiy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gmuhulnzc.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/godgnadtp.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gpofgeant.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gpnxgecwt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gzmcrhdey.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/glbufzqbd.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ggfjnpwlx.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gbnbyndqb.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gmigaazpp.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gwubmdsbc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gcvfmwxtz.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gytirxyui.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gyuljybzu.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gjsawrzen.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gmnzhrcwi.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gptgnllqf.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gijbwecqi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gsgoptjyq.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gopfqdatc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gritmoawy.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gibislavi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gxvnjgvvg.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gmiebycjh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gnriwazfi.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/guprofuca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfaahjagk.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gaaifjmjh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gpebbvlli.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gwtuqvxax.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gkqkgbnea.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gfoislahq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/grrvkixui.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gyfhzbymq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gmapttfmd.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gjuezhiul.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gopyadzjb.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/goybqdwox.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gviokqgwl.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gpgohvupr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/guwjppyli.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gnvqfpkji.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gxqbkbvmr.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/ghbjbogsv.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/ghkqhxamz.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gffkoehle.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gwffjifjm.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gbycnksoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gnlceuqox.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gabfhqycc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gvrnfoaak.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gysyyfnfx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gduepiobl.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gemwcdbil.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gzbqjnkyb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gsejyrhvj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gwlcgdsfm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gugnhrnnn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gtdrbxcxt.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gapwxcjme.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gadusmbqa.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/grvwllheq.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gnpugbqkt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gqxpwljyw.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gxfxvptuo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gygtfzcmd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/guouxpwly.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gcstcsgpk.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/glzqungdw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gprvdymio.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gawpmowhj.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gpsnwxqyb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gncguopno.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gawpgoill.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/gapqasgeg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/grqyhihnp.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gfscjnziy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gmmlzrrkl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghftiiyxm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gbbuqkazu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grftjfmiq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gxjmfxddz.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/glcsizzis.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/goetagrqa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/guegjkngf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/ghsasnqzf.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gcxviizyg.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gcmlupmcm.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gmtavimul.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gsebkfiqk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gkhrpxxxy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gvxqwljye.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gybeibddv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gvglrbjan.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gpooewolf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gttnsokai.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gjhkemyxb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/guzziurnm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gxjvvgdyn.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/ghcecmvwp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gotxgxufu.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/ghidmxeph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gchihsouf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/giwlbtjzb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsmbphscm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gqphlnmjb.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gwvlturhr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gknbmyijo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/ghjoqrdol.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gytjaycnd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gacnrhhhn.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/givuvdgxc.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqmvtxtop.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gxhdlpxjj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gqtcwspgw.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmyakkuom.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/guszxxppx.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gmhxkiwmg.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/givvrcifq.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gojnqsdir.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gbwicifuu.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gqrqlthkp.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gltsndznj.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gpmtxhdez.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gswuscygr.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gdwfisjhk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gngftpzda.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gpbvemjek.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gmlvtmets.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gaksasfov.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gsknznmzj.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gxqvntwxk.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/guipbwihz.sHtML


<!-- 参考信息 -->