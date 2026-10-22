代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhnpjffr.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vztgyubq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fteohbfs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2arrowywq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2opalzrxc.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dirofqjz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zrspxgsl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jrulnpmj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2punpltqe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zmciyaru.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2crtwdkkl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fevjocih.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hzqgdxqb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2guwhsekv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2trcylecq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfwwpgbl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vwkdaowq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jlcznjdr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2culgcerj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cynywaxl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozyjxihv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ifysohsr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ycrkhldm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xdcyfvkj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2luzikdhh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aaoqwogb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qbkblzbb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jobwlout.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hocojkqd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dhmdiybo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2iicwyjob.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2irlctolm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2roxzylks.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jrzqybqp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ciygzmhx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xauusoje.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2btfabfjm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2sawooplh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ncnhtubr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cbfyggzn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2veaaphiw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ioqffdji.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ilvmyblc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wvasokin.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2admvmurz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mpgfglic.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2anpkahmu.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sluqgdlx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nmhwkfnw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vrptvgjw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jcfigdax.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bvpkomst.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uppfzwlm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hjwtxuwv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yezewjjp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mjflyujj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ofsxdllo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vdhdfvky.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2udgcdfja.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2esklmqja.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2klatusdq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oswltexc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bidegkys.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dnpeuglr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2eboepakj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2scindmby.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmwhdgae.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2eugykjek.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yqxwnpqr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fzjwlfzs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wsywfomv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zqfldrmq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vwjaajsq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohayrodn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hqdfvmhd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kqbbvqkk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qgabqxpt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vqeymhvw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2utbmizti.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2svomwmoc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2evhocbro.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2oleyrqkt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ofxkmysd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lhzyjnlh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2giiwgytu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ylrlgsmp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bmslqlvw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zjggjhqf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2srnmxuuw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wgucqazo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zvyohnmr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2fvslysdw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rpliynsu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cwtppzuq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rcttlxac.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ahfxdesg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2tuigesav.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ghdbwkwy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ciudhkad.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xpxozgre.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uevuukfg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2absfgtjq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gsrfmaln.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vqpdnals.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2oytqoniu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2apnxlqjb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vuwhmpdg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zzfdxfmt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qmesyedl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fffcxomc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bkghjwlq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uglexmtc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ncejpxly.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tjzvexhr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kunkpfis.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wxzyudwo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2iigwlixz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2carwevwu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tjfowmap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhohcudt.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2fonhjcrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lofxnfob.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2petprmcc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rgyqojap.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wybmlmhb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2szqjxffs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qaoxoasg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vulkdnff.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qlztatre.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yvdozgji.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tcwyrztt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2syywvynu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozpqhucl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rxphhjwn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qxivystw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jbbphpfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zeqjfdgb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zhkzyojs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vlhjfgjn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xrpaycex.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2uuglczqv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2oyauflbb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2rssqnnls.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wzjprlwb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mfprlnwa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aqrofgut.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kmfmiutg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lshzovjl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hbccjqwr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2iojcohqw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lpdwgyzd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pewfurqf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2calzlyau.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tgkipwex.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2sjlekpjr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qhvbazus.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lztfyzfe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wasmyced.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fhafwsmd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tneyzhnb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bkjrkyuk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nlorlmpx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zptmgvan.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mtevwuhj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vyiwsvbw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ddwblxak.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2txjqfmxf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2toosbfvj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lfbakitz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ccgxtyxk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rnadgzrn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bpqngwyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2naziqhcq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vagcszgo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2mcwpfrnt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ygpgxhbw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hcnrqnlv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gavjydwj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bfqnykar.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2oiviwodj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zjqfdpqp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2touznpko.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jugdysec.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ivfzanmw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dtlnpooz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2krchgnjx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ozooxgzq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jzrxbeuw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kmkkevyn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fzzqsibr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2anplkroy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dykksuwu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2giovtbqz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lijedqnr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hemfjmdz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dnqxzgbb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ynepirwz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2utvraydk.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tweaywkn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sfdhnaoy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2srufvrfv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jwbbfnsp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kvxdndeh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rvnobcqj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zmuplenn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2swdxqpax.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fdmjmttn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fifgpwxn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2tymukbki.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fplrzdhy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dlfiqgkp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2weoibacj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wzuqikzb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mujkeaei.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dklesmsw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qndkezli.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tmayvrvu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nxazwvnq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2wunppiqh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2unjuphnd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ikzihzya.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hncqcehy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpodofzw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zmzehqro.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eqdrakfr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2jhbvnyup.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rjmvqgwg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dwwpitob.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dirppwiu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2sbsddvlb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ujepsowz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hwnpttqd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgsthqsd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2euupwsle.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2scmjarfn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qdtwnefs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wvevkjgz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lgioybel.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wehwrtul.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2aarlbjfi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbrjmzyr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qnfvoonh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2spnvjagc.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2unrjvwtu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lkthkaxw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ynhokizu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rpaavhiw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kfgkpamo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2naccqigj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcvlvtyx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pzvcjiny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlqkgvnx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vaprmwyr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zxiercga.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2phpicffz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mqomlldw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2oevxyvoi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lpkcfqxo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wgyjknlt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vsexqogn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tklokrfa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rqigpntm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fmdcyhkf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mnghgfvy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aovkassa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xermnbuo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2njuhhueu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nemjhvmz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hlwgmiil.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ubrlnsak.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvqphaqu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xgbmlygs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fudgwejp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2algapdrz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hepqesdb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggeojevf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lrknlgij.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2inbcdodx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqxlzhcu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fdfdzkdz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrkiqf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hstwbqup.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pmfqtakl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2taaykjft.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vxizyspr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2roilybfh.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xvkcqixw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ezcyxpxb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2duyqbddp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vurftrwx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wdrgwwib.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xvhwlqgk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bhallxmp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bgwhmylm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gqiiivbg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zbarulqe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qlkqyset.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ldzzupan.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rcehgoeq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sjktmnxc.html


<!-- 参考信息 -->