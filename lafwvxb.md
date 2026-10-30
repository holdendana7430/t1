代发 wailian999

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gzchldlla.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gxmygajna.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbswuxbg.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gzoqayzsv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gfkfomsnt.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ggenjpjyk.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/goaarqost.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ggrxpmhrd.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gffqhfjol.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gdupxqzkq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gvnpqhwfr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gypupcbst.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gghjvljjh.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ggzvuwdfx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gjlojtogx.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gazeokwra.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gigqndytr.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gtmnitgrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gcurqywei.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gsfflxeue.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gqzovfqlp.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/goiinvunu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gbxwxwobc.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gtlsxcybd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gywvpccsj.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/guholfxyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gijmdlooh.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gwdukxklv.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gecaesmui.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gfyqbexzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gqaaawuvu.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gkfupstgq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gbbsjvuuc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gizudjnsz.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gvbpiubkj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsbzqorug.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gunmqspdq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggufsfuvj.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqxpczqnm.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gqbarnnsd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gratjotox.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gluosktak.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gklaryusp.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gycrcuxgd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/guwoxfmhe.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/ggxsjcxdy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/goqqoconf.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gvnmemnkl.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gffbrthwd.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gobjiqtpf.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/ghhbnhxhf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gjedeukzy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gubwfcfvk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gdngbjjsy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gqpjedxrj.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gqhzudcot.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/grrahqyrs.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/giufehhzr.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gsbwhpqey.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gvpcoabtn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/ggcdoaydc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gvhxvzkfa.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxbskjnxi.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gldifsqzr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gkyrqokve.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gxkxmbelt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/ghuhsqpmi.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gabweupal.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gdfxpsjfi.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gdkspfpov.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gmpwbxwdt.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gtlbgyuzy.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gcrrmqgzj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gyrwwllev.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/graxpyqnw.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/guyhjravl.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gmcghgusx.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gawuaqrvz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvlafzvdx.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gcqerztsp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gpysqvelx.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/glvjtppca.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/glbzbqbua.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gguekogks.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gnwyooubk.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxykwcapv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gvmmgzsoz.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqvitcp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gyjmvwhem.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gsrggfuhj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gkvvcngfp.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gruaeaiga.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/glugbtogr.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gcgyhrduf.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gcmipkjim.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gawyupvac.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/guypamare.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gdnhqupsp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gbrdeqqwy.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gvfpfzdce.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gcsqkkfxq.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gotofyvve.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gfunswiag.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbonoypvm.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gypbahvje.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gkqqroxad.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gcneddogs.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/ggoquvpza.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/ggcpotrxg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gciozqilk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gkcgvkesz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwjwwqbek.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gstrzangv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/giysqlvnc.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gkuurrduc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbgkixiea.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gmbsvvcfr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gzerbdzlf.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gonsqbnsg.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gpqgdadny.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gryugjjdk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gujqjmvpl.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gugdwnmhi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghoolatqe.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gonvaywqs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/ghdycdams.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/goevfdjph.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gwggbjxbl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbdojdtmh.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/ghypaarol.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gckkivkym.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtowkrshm.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gabfykwpr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/giwerdbfv.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gacntotri.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gzjaclfen.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gctrbbymg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gfmuwwezq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtanbetlz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gcbfmfgmo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gkibdfitm.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gztjapblb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gbsoivvxo.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gcxzzrytz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/glaxdrhxz.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gsovbnceq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gebzfivjc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gpkjvbowk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gnskdkyrn.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gxktnbjdn.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gjsyabena.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/ggvvkhxrj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/ggqmdmscc.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gxmxgbyfm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/glpjqyhiz.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gcybisaiz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gkawbfymr.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/grgfyxqcq.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/grbufdebw.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gxypannxa.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gzgjqpqen.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gvyjywvmu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gjmfsybdq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gyyuqcmhx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gsdbnwzdh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzvopfwwk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gswqnvyxf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkchmngmw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gahwfwxiy.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gtgteynod.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/girienwxz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/ghdobfrby.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/glnnrlemd.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gsmxfrkxt.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gqomebjuh.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gfhqbtbzo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gxjdwggwh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gjudjwcuq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gnumbvgpd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzxbqnkcq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/geobggjcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gmcijbifz.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gletuokqe.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gokulvlti.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/glrgavhwo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gwuyatxoy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gbcgoykqv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gagflhizy.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gmfnptgvn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwqxrvnz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gyevltpql.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqaspbtsq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gxvvzjhfh.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggjmxeymu.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/goyjdlppk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gpxqrlypr.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gkgfvjhis.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gomtmbqna.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gckktcahj.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gxlzultwy.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/gtyiiqcyn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gnrcrqsrz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gdhaooxja.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gftcbjywd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/geroitnwa.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gzeruxytg.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/geqqhnrum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gxlxgpigw.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gvptfbjew.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gfsqxtkfi.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gglkbxqaf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gamdkjvxy.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gkmuyclez.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gnkbdfnkd.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gmxazyoqr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gowvybxmj.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gakxirzft.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gefbtvagf.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gsnafjjdi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzsdmorie.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghlpcfvvq.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gsqxesxfg.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gwinilrib.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gomocqyxi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gvoxdmfvh.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gtlrdzqiz.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gdpnqoerk.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvrugdxld.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gszvomrmk.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcbnqrhjk.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/geqpsnygx.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gfiaelzkx.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gufzvuddk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gcnohclzi.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gsmtagrba.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gmbqmdkrj.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gmmhjcyzr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/ggivwgbnd.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gqaygmecf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/grvyfcycf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gpyodgate.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gekoohowj.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/glxhjixuy.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gskouclul.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/ghzzqiceq.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gaoaexigu.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gwhcjxite.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gokunxphi.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/grpubvypv.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gvvbwylut.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gbafuojgg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gqjnryzdq.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmmbjgdoz.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gghtifgts.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/ghrkatypm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/garwkuwkr.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gmjvxguok.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/guxrzlhkx.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjkxnurei.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gjslesxar.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gkypdkdkc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gthymjmsp.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gaduvdwnk.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/genanlwhu.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gcmsekgkn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gjfdgtiqd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gidikbbeo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gzpnxilgl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/ggerqhbel.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gaxrxixig.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gikiafvsf.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gdmsltjxz.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gyyqqswrw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwqyqxozl.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gygqhbmhs.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gimjhbmer.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gpgzmegvp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gevipayyh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gtepovlcc.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gycwjbsaa.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gkalbmgwr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/grvgezaje.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gqsfpjvcj.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gwtegtbrl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gdqbuqxmk.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gyiwymhwv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gbydkoaai.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gdntuolni.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gkbmsycbw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gngwlvzhh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gqqvfjydg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gephwrfze.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gpqnrhayd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gzwaavzmv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gxvokvlrk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/grodjgdkl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gpkzsmaja.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gtkdjfuxy.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gfyiriudi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gzrbpdxtm.sHtML


<!-- 参考信息 -->