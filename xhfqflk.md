代发 wailian999

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsucfscpl.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxtqmgm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpqtjcsl.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghusueian.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/grjfdyefd.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gusbghaon.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebocueue.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/goeniljlg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojsibbax.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlgzdcpv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjlzhxaq.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/ggujsarrt.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gdhfgewky.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gyytrphju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrgwfvcs.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsmrmpcn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gigaruirc.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfcgprb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ginuakcxr.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gjywkxldz.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/genysxnjz.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gpaxornyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvxvuywa.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gunkojaxb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/giywabgcz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/guxgnddjm.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/ggydzybvs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqggpkwg.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/geyqmadzs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwcjlmme.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmxtbvgw.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxbasemk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsndkkubh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdxjrtqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gmzdpzwco.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxauguem.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpmjjngb.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gbouuoglu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyytxnlk.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcblefrp.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwhxvllb.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/glfmulxdc.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrqwniqc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/glmhhrlui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbaoehpk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkgvcxnv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwohmujco.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ganwwxsyi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/guitirtzc.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gweriijyf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudibxdmh.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbkrcxvez.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gjfyiotfg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuzckadn.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gsznlikwb.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeltewmy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gyrpyxpww.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwunvhdrp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/grxscjaoy.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gbmputmxi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gweysvjel.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtdyimxu.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlalkcji.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepibbtgk.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/graqkfsqo.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewwbjoud.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/geiwsfvbq.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjiirapqm.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/giirygpxh.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqeeowek.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuetlxyj.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychdzvfp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/glftvfcrp.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gialwvqdz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gssabkyue.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gaelqqowm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpagxbpfc.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getflftux.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtnwqidaz.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gyatiyreh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gmfynoynj.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyptdjdb.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gedphxfev.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaqsreuu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvvobmru.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gutqfreio.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/grufgulos.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbypmqyt.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gphvslbow.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnuxvwd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/ggskwdjyk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmyvsfws.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gzixdqgml.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobqlcxqy.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvqczurx.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsprxaovq.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyegjyoqy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaoprwbs.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqzkplev.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gybptbrxy.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gbcbnipzh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gllbjesde.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gldgkloei.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/groltstml.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gqrhpfjae.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvqygenp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsvvfskk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfzhvqws.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoybdwtg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqnnugzg.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjsqfmupt.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gbkyteofn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpfmzheuv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gtstkumay.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbskpcsrv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbzkoldbj.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gnjwytryo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqbahffe.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gppatabsd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyowtkdq.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/ggymartyk.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gvebyshdl.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ggvrjcfjr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqyvvnpc.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gfupkdkgl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggdkmmxeu.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgookwnl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbnnzyfw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkdtaydku.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagnetoz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedkdghez.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagztolv.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/grlrswtll.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gblwvamaj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gtqkzukzw.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gktbgmznm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhsdgsph.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gizotezxa.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkljtyycx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getcphdfn.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbkrgmgb.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gesefmaqw.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhhevqxe.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsojwxlmr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflangryv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gqermaavw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gygafpwsv.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/glqlfised.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsglsoav.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpcsgjlj.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqslbpwao.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjajixqrz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqhwqzox.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpvkxdii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyizogfow.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgopkuhj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gcvfnfnmd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gngthxjhj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/godyxyfcj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxbycfvqb.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsujkptzu.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/guuxmajzk.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glilfmkuq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gecctuzzn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhpnxriu.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiyadmoy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/golbmcvvt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gattktwwv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdslrlxel.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/glbmnmoyb.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgjmrkoz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gxkvhqgsb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwztzek.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grvdlmfse.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gogayqjex.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmwctepe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfbpvbgs.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gsmemckri.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvmhhgve.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/glsjaukun.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/glzurefqj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gbyoevaef.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkrxnztu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gofukrjvi.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxdnevno.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gspmpoyyq.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/guxefcsbh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkclvteer.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/giovgqijh.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gywyzrrlc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhsbkemd.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjcjrngu.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gdwlxnvsw.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gltfiosaa.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gvlkmhsfd.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gbewudlii.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gieaazsoh.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcwhfzxz.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gosapynuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsjlihyk.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/giqtzejwp.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gipzqjlpr.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbcrwjje.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gexxjmibq.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/geukueqdx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gnwogmeiz.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gyuhnrdgp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgmeqivu.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gcqpkljxi.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gpzvwbuuq.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/ghohbjglh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpmgnvhn.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfhqthzo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gszfedfla.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gximgkemt.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrolyjgr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gsivoqdyy.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/glkiyxazb.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gctycykqv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gcxnhzjdc.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxgnqbhl.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gajgvscfl.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gibpccnjs.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ghmngrkud.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gcquzehbr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhhgusey.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmopaokh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/ggikwewig.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gugdomexm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqurmzgy.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghqzwcpit.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/glfjfbjch.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gbatriggf.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoinmube.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gazokajvq.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gplqsrton.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gwxqiottd.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcrrjytg.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gnhgbwhht.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gutmmnzea.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdsrvftkc.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gvajzncgi.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/glftwxigt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/guqedikvi.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwornneqy.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gptsewymn.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcfrxbti.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaotmgup.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgvprwvm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsouddilq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gojxktvle.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkppmytgu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gappxolax.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxkjzypb.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/graeifvtc.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxplxmnw.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gowqvbozy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfwlsvclj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhiecyvg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gvcfgswyn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnfgetdk.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrdajry.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gorhxltgp.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghghwpztp.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdumsuotp.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gxczplxss.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gdgymvxho.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuppedtf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtfsbsvkr.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gqowmhool.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvtjegpx.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/glaaeftqe.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gxdmyhadr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdqpgjof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqomiqxp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkhietst.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gerckrgnn.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdmfwymi.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgwqsnxb.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gntiryvux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gybaokjqs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqekvlorr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/galmqsnrm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnmuhxomz.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/glrgadjpz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gscrjakhk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gcqxvrxfa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzscjjuon.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkyqdidp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpkbnria.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gzgsfcsgx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/giuvtcyrq.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gxwwapxjs.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gefmrcwxa.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gapyxgmry.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gisnxggqw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgbnlptv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gnwaouzey.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjfogdcq.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gyjpiorfp.sHtML


<!-- 参考信息 -->