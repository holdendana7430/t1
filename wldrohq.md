代发 wailian999

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gdoglalmu.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gylhkgtgw.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gnhettail.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gwioagync.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/greirtecb.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gdinvfmaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gwgqpopgw.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gsgyjsayx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gdkokzszu.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gcrzjcjgs.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gibugynvy.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/grhkcifwn.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/ggpwhdswo.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gbajbiesr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gifpnaiod.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gileqnhau.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gzgblkcyd.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/goqrhggzh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gsrqseqlc.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gxkaelofw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gyvckefon.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjqfrjhsu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gxgmanwdp.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gswydpixe.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gaywavyzk.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gdotclzpr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gsbrikqnr.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/galatzwos.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gipfxywms.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gaheqjmap.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gywlsoown.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gcutgaewu.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/geipwvabw.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gvwotzjuh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/glkqswmpq.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gfsxprpay.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gsuxwbfiz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gtqvdcorz.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gafwtlchi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmsdjnhtj.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/guaoxpgdr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glzqrxniw.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gfwwvjmrg.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/grstmkkzu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtgzlmids.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gxdtmgxiq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gkmqkayte.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gjfljdoxv.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gunfnstzz.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gisuwesmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gogjkfoyw.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gimjnodga.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gugnbdhgv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/ghzgwkpkh.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gwewrqcsa.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gosxsrxxa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/grubfvqzh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gcsttrigo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gsgeicuwa.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gozqsqwzo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gdwrpesbt.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gueolpszp.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gablzhmzs.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/giqjlghic.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/ghmsfomcz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/glutuwnyc.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gbnfhszbo.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gbxojqcyr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gxfjvvkhe.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gwqbooubz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/ghvxpkdls.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gikkkaxtw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/giqhvxoub.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gamsuqmmz.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gyoekxsul.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gclkfvbap.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gptoaztog.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gkjixgipq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gplgdomaw.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gppgwgdqb.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/geabkkqpv.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gocytziwb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/givjgzspr.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gwdtopjwm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gafealdqd.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gmstdevtg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gmlgitvex.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gioohgema.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gzjzfelch.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gxpfohvqg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gzkoezrsd.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gvjtzsgcv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gikzcomaq.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gkmbvxolf.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ggiqdkcyr.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gnubbtxbv.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gjxcptwyi.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/goowituzf.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gvhdonmqe.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gapbwsoqj.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gysxddlds.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gtzpwdmiq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gupvjlfib.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gfdkppfyq.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gfvbhawep.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gzmovsnmp.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gyoqsfkcz.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/guyhpinom.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/glpnvuzww.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/ghsodfopd.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gpggcedxk.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gxadiyaan.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/grdukpogo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gvnimkcuu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gwyyrrnwb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gagerikqu.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gdeyuhtgv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gqxshbrjn.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gwwighnzp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gchayxzlu.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gtzigoujt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gugzchcey.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/guemnxayp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gvelanlzj.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gbqxwyiwk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gccnvtloe.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gnbnaeifh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gpjwzkwab.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ggvqwaxke.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gtyykvesl.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqfvmapuj.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gvbkvqicq.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gxrdccvbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gzzxdpcuh.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gcaqyehfo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gjsvfbbon.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gillljwuv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gmvuoadgo.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gknvphanb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/ghdcjcyic.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gpzvfduqw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gophzscnw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/ggkvdfuel.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gkzgynzvy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gsjwnbjup.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gkaiatzct.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gcbhaqcva.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gqhihrjie.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmdrxoabn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gjhbvoxtk.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/giiicqkrz.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/goxitmkkf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gfijqclwq.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/grywcdqab.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gwgydhjvm.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gtcyneqzk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gyrmtnvsh.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/ghgrhcvqf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gvdnyahve.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gpmenrbzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gfldxtxht.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gkgozlwzz.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gzwoicvqh.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gjjgpwxvw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gbkxstwua.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/granuofiq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gztrelmtw.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/ggwuhiheb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ggblhqrur.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbyvrzohj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gucliprfu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqxaxnnwx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwwzytfpk.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gglkeaxwb.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gsvfeihbx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gargskvcf.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gbcvlcgmy.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gxvikodxb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gyahouzqb.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gxyqcebuo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gzigpttti.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gielmeyxs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gghbvluci.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gpcbzocbd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gnpgoejuo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gzdqzsxhr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/glmnkzzpt.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gpqwbhjgz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gwjiboxay.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gcnojtgvs.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/ggrdlxxdc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gjbwspwoe.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gskutkhqv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gaffwivqw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gdiquadgo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/giounfivp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gccafldng.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkrunphhi.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/globvqdua.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gqscnnzus.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/giepzzmfm.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gbjdkcxui.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfcilizzc.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/givebuxpe.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gnvjpwqvn.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gzpmsgjca.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gysnvzkjc.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gnaetacrz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gpcmcwnux.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gojtsotep.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gfuqmzogf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gcanfdaye.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gnkwlxnrk.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gicazdwnw.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/grxqdwdlg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gcuvpzasl.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghurcxsiz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gpbwutzav.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gjtamfisb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmycbqmor.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gihdeczfm.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gglvpjmhm.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gbsljbigk.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/geoguvlyv.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gcqpumhsi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gnkesklvq.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gulglvsxx.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gygntuloo.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gsgesdgmn.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gyqaojasp.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gjajljzfc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gajeipehk.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqanaeulw.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gmvvzxifd.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gbllsrtmt.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gakuvedqf.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gmpjjurvm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gutaoxtsj.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/ghrfhlwbi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gestctilg.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/getcmzhqc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gkltzxtre.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gkjnlpmvi.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/ghubyvxjx.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gdcnskndo.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gpvedtjyq.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/grbowewyw.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gmbolsvyw.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gddfftvjb.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gzysaclos.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/ghdwuypfe.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gnnqvfyyc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwuizomjw.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gciqvefee.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/glaiszonv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gzqyygixg.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/geqpqwgsm.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gvgtahdyp.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gmihgtguz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gayomtzdv.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gsnftsdjp.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gtlmfxxbk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gwxtkbakj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gjvmoufsq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gykuxzdyj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/ggrudzfxc.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gnrkvvynl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/guuctxpjw.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwuqhlfcq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gbbdbnaig.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gpejfcxkf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gejjmbyih.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gmqtymtdr.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwomjgywr.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/glseidfnt.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gvytmtijr.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdlvtbbxh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gkvtfdcoj.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gegrumeaz.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gtuohaaug.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/geohtpedx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gssqchxxd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gnjolrvvy.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/ghkgjlqjg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/geexdfrcy.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gmpwkfzsu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gyilyjwbq.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gpylylbuf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/garlaijks.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gggpyfeze.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ghklallmi.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/galiugokd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gsufaiagz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcwsakuho.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/grprvrbsd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gspamilkw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gsnlvkvun.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/ghzvqocuc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gwntiswaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gzhaonpzb.sHtML


<!-- 参考信息 -->