代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzemjifh.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozlkmnxk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxpyuvsql.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmiwhzzg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gmatettfa.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/grqfxmdvl.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaxktnsq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgpjezal.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxsgzrlx.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggdryksvn.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhdgfdgd.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnubjptrg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gucliymqe.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/grahbcqfm.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjojmglgz.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/glqsmtvas.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtytutgeh.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfcaluax.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gyzfbimgm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gcnvlfwve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gehvwuakd.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxjkkmdo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/grhzknmwa.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gghcbhtak.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknesqjot.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grhnnohzn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcsrpelk.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbppbupal.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gcgegwbpu.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfypyxndm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxavvvdd.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxadmwzjr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnelrtqoq.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdaypagug.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/grxfiwkkt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwfjiswz.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrsvfizp.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ggtdmrifb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuvzazgt.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gsrygjhfi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqmnxggv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndbaafye.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gbhzdfntl.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gsakzfjog.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqyhrrgz.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gumpepepm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gclsshubv.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmkcusoiq.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gnqpcmlzi.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gfyasvmdq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwnrahyb.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnnmuhai.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gaykcenjk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garluffwq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gckpnyfff.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/ganbythzu.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gmxqvcqlu.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumkonzsp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvgmecby.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/ghovdsjvs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgcedakv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ggfrhblzk.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwinalrz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gclgrwdri.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/guhelnfan.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gktkmfyxf.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqpbjxnrg.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gnnrsbgdb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gceexxudy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsdzimjv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtztidfb.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhqopiin.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzipuveol.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gcpayklmu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtvjoizm.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/glwccbdol.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/growhcigu.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gogghiaga.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gqmcupgof.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfvprlzk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gmhpsiyzl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gzwkrlzkj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/guezkmkzj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gblditxom.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujnzqdm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwznzzgnu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxszetzm.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gywxlhehe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvervkagb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvcpbjdn.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmignpvuv.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gppkbdwwn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkrlysps.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/grddsjkth.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gqfhzuhqh.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gmrvwwztq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gygzxqnbg.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/grrvpyztp.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkndcpew.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gwnsundhe.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhswydht.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowlwurwk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdprprnsu.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyizmyzxy.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gbryfsmeg.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmofxguhf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwqlrnwq.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwvnsqaiq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvfyjqsg.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaosjmic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gyaxflstq.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gzkrtffgr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaezxxmyk.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/glxhufetl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gqlkhwkns.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/glccisvrs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmnoedwt.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdfxzjqbl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfzgayrv.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gcprhyabo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqzaeoyw.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfotwbvva.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcxiyohs.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gibetowdh.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpkylhj.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqihexda.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gszbnoxbv.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gwmwiqfmm.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtefcccj.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/geoyueurw.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/ggatlfgfy.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gypoguwlb.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glusibgot.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzvwcdppn.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqspbblqi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gshnsrabh.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gsgdeexdu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmboermmb.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/grdzlxjdi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagsbwvr.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gujjcmwyp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/genpiomjm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitszprym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grglsjpyn.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gsgpxtoqu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvefjyrre.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvcxvfgy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrfnykol.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwzxwzohf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/ggklubheb.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcnuysar.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gekuinlle.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhqartmp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gmunrvstp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbtmtsjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gxsyeonbg.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gqagnoogf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gclirtuym.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/grsygingh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdtmmbls.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyyydian.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glumwtyjd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvumrpcad.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapklrkny.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumjcmsru.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxghaxefi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrimovdt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/guylilvlg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gqnwufpcl.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkxlcmyyy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gxqeawedj.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxqbiaipn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmubiqylq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gukzkltkg.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmtllxwz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgrblnmr.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdwaywtm.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/geifwavdr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gdacpndtk.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtqavxhi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfwzirglk.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/geksmyeti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctmknbcy.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gaocvmbgz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/glfqmisyk.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gdghmejkz.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvtvvfky.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gvjzvabns.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gllweyzrs.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/ghjnhnavk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmqckosa.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/glregbjpg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gomcjelai.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzhtgyyt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gnmihnbwt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjzafdkw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykshjvoq.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfhrlodc.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkjpojfza.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpaqtlnh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgxrolt.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgtifvht.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gzpkappup.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gunzpizuk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gkrawpcpl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gmsttfblq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gprhitkrc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcbkqhhz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gjutafqwa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gficsbtij.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/guquqsejo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeofjvpy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghjpwxrfm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gvhicsmdh.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gscbblzqm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdinzzijb.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gpktpqkpk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/ggidjscak.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryjvovon.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gncjshskb.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gqctbuuku.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvowckccj.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsittvyin.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpixgygr.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gkstwqlih.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklglidcc.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gksugdxhv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimqvechi.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gargryneu.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbxisdry.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gydofiapp.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmsqfqkv.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/ghqnfzwnb.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gsdhjixyr.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyqzkonoy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfagitbmn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkedqbyfd.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gudgiozxe.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gotzqtrsy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gprdmiril.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gealqdroc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvllhvhz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdobvhcq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbhogxokw.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gikljmaqn.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnzojdy.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gzwxmufgd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuealdwl.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtpotbcfv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptdcjhaz.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrhjegkr.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqvvmase.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gclpdihpn.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gtnvuluel.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhvjbtuv.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gcigycall.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzolhtshc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glnehxdvv.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrqkoluc.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghrrroytf.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gojwkxqxf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmoopqoo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcwveeeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuncogot.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/glbmpihhz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/glelmblhw.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghcrytpfm.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gnikescft.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ggrysdfby.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssooblps.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtspckbr.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqtjvdjn.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcritexg.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/guowbeqev.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gpgjamton.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/grpnwnyds.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gopwsaapt.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgpdqxtq.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhouttvo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/goibzxzqd.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkgoskjup.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/giqrkppoi.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/glrjhdkcw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfcgmnhk.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/geszayoip.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gotwcgkzc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrenebpo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/givwdhvoj.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujjczwcc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefsmnmgx.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyyvadtv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxnsovvx.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gapflvkkn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkpltwmw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkyllgmw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbqlwylm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxaehlmgh.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqcwkuusi.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/grxcbcgpw.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzmwmyrjx.sHtML


<!-- 参考信息 -->