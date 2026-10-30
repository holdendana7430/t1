代发 wailian999

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gvruvxsyz.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gmuzhovub.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzhwejxb.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsopdzomj.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gasajiohm.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gsczsmujs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbtecunf.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gywdhwzen.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glasidkrz.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gaietjmas.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiepavev.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gikvmlerd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzclpfby.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gfgilkmos.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gazaachqh.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gggntyges.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gyigbhuau.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvtmcsfn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkcbsxig.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhrdaftd.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuzmfmtt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdksxinm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbwejrww.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjyybgbp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjxmidiq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gmynxultn.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gexrfyryv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsstbswx.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpxuocjn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrgrcnjk.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdkeggvob.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoreteec.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/geszprrmp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gagukybxn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/goxzjhets.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuwluwez.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gnioklndg.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmewjjzv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/grncrxtar.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhvqghye.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjrrrfbl.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjmeyzx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqtsldgi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvadvxfb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvreiuxgy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gyzthkfvn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gxuosnkoo.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/glltssgct.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/ghjltwjti.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gikghlwsz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiriuzpd.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gevxvkfbd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaszvrqhw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfovfdum.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbddfswag.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlpbtjfo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezvthkfh.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gwsqlzwmg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcsuoiqg.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gykucbvel.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gyvftzngt.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggevextzb.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gnsaejatp.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gisytvahw.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbdskyqg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlesovqf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcldadums.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/grxhqhlvr.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gohbholxn.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdvzoies.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymndkkwa.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotzukbor.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqmwrirw.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gaexmimtk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gdfrblibi.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gqmblsyuc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/genzwyhul.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gjnamidkp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gigriklcp.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gcaidyjnw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gncvstuar.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ggavpwkgo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdwkxspx.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgyvcxpm.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gntmcazgm.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gauqygagn.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgcdfmhr.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/ggzlvegyc.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkugcdel.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzicwajeo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gqugxiqog.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexnxbwty.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnwlvoih.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbouqepwv.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwkdgymy.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxchndaoi.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/ggecbcamq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbsvaomtt.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhpibipu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoezkgjj.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gywaxscsx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkugwqjoe.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gufcmhuoq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunxxroys.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjrlqoob.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/grxxlvtdw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtmydqua.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glxzarjwt.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gppucgxpy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwarxynjb.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrkwjkio.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntemkvrn.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoovirhn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gdakmumpj.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnneqixki.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gdeswvzhe.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjyuagip.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gyuowhbiv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlwmmqwu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdewcepa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqwcsva.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gjfbzeddq.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczrihlai.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnvefklb.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/glhdxjvzw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpwceabd.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gokwqukil.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/guaxgnook.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gepidvxxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzkwxuyv.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/giaoeehqk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouazdmxo.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevjsejdv.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqiydkncg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/grreqwrwo.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyrhwzwx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxtyapbk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpdjgwdk.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/ggcmxpspp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/geazwkxic.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gswtubbha.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvfbrzzh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gbujncmzj.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gkstmnvoo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyazfacq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gllyfqvgg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggnuvzzka.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gwhqcncgc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guhjqnqge.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibazdors.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gzcgyrjkw.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gopcptxgo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgslamun.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvkcesvw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gntfgythp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczatykdi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhokqano.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmwxjppps.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcugmdqxs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gquvxxnam.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guxdjotfh.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjmhdqei.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gixyqdykt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gxuaimwiz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqrsuses.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gblrfztho.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gxldxtnjm.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gfdfeaidy.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfohwfqr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gahhlqksj.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gjnvpgeea.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamllwndp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggsaycpdi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjuallrg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gzomtduyn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwiphnyz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwfzzuhl.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdglhudxv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxwhvrgos.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyitpafpy.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gxgxuhpre.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgfhrdhn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gediyupnq.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/geuwtpgjt.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/ghqmhhwff.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuuvkoec.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/govrhwewv.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gmlihxwwn.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gttjblzan.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gamastgvs.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gphkxihph.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/givhfscgj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gidtsnbch.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwejfukuj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlmvmnss.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxamxvvqk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqqkcrhw.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvdcndom.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/grwquzyhy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfcpuuwz.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfmrctnzd.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyhzwpbe.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gxvjdgxvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxwttrul.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghnpzbvrc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/ghktbtipn.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gjlvhqyat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gajcdicxb.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/glsxowzim.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrppsatn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzoibpha.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gldeajwnd.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/grdojlqyb.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevelonsi.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvzhjwvs.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gieysjzlr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwhvlorf.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gkhrrjmyc.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflgumvhj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gsppnkyyu.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gybjiihoi.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/giafvqwvn.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geijsdqyq.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gelpdtogk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gztshccab.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/grfijnycm.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gswnbstmd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gapseztmx.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmcqrqsw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfwbmfsr.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gerojyiht.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gccbmyyhl.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/getyjzlwy.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggamnkaf.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhfhurdg.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzlaktcl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnvkcyap.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjamdyod.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gvnrvosjz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gwxqtpave.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfwybvsmy.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gktxxmpzx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgqiqirq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdwflxen.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gitgwjvke.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gcrsbqtok.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gruzikikv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpusfdxwk.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnedmahga.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqxllvxv.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcogtvzn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtegnymuc.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gamzggnxe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/guyaqvszp.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfejayxlu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsjmqoou.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/grrfqcdll.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gndeiwgrr.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttpwjeru.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gybdgslto.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmpmelcub.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdupxzfyd.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdllhftyk.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gibpmgphw.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghddvyluq.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gausdgfez.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmfmfharh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpunulibg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyqynmta.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtezymjqg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/guqwovukj.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gddgatvtx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnivjfsfp.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdxqoolx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbpadebu.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/ggkbhfslu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgppsznc.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdzmcqou.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gielvwbyo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcaglenj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/guzmwckrf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcniwnysn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gckpooqgi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtsnbfkba.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gjgypofau.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gxvgpnpwl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipljonfj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gizzgzvww.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gknwbcfha.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gqkhkacei.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuxovdxn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gzadiuarz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gxuainspp.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqtbucnw.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gfhuwxgub.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmxmzcaf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gzsjfpjfx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gcplccszq.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizbditg.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gvhgbvena.sHtML


<!-- 参考信息 -->