代发 wailian999

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyzyrkff.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvauxldim.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwwsxhzqd.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gwppyldca.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gkminfhok.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvfaypgb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaqyvtoc.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhjutekx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gplybvrcc.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbkvrjjh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbvkfuaqr.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqidoaww.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gujojcwdn.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gqafyzabb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gwahjrzoo.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gndmalatp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnwlnnje.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjcotjgwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/goejblawx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gqhnpjxnm.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjwqdkz.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gerqwwfvk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqowdldk.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpcapqhx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvysztrel.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbublcjlv.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gzsikphtr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcfxdlbrg.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gndnjbhht.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsaryiwiu.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggbjcdthx.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ghkwwcwkt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gswuqsyve.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/glvjwwzkn.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gejtsfydh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuokkejh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbzdwxdk.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gyyllorkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gxbacjzwv.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gecondfzb.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gfrfwuoet.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtsrhprlo.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/grnkklfhl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjtpcfue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/grvvdqapz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjbvrupv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gxevjvwei.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzxilwbu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsnszprx.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gcpeietud.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqknaatlf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflzuazje.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gggvrovei.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwdskgtk.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnctxwaef.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwammizes.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvljwohhq.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflxdsafs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gbmqlfhnb.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwjfqaxof.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gejjgrshy.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/geenqlgee.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbptpenu.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gvqywtyvp.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspovqxvg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghawfwimc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqohausf.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzrrlpstt.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxhxzhnz.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjuobovbj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gjmruyrrp.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpnslnkq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewaqtxxj.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmyrqugvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdyiodd.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqptymzmy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfelfryq.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gkvlskgxp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltarzuea.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyaducot.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gsvlsmqok.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiiarhme.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtmakhfh.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjmxamws.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcsrewfd.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuntpakf.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gokxoljzv.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoccpljv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfmshzpx.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkwarjtg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwthifran.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gjweptoir.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gnolvjixx.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gxmkgzwhp.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoxgcqbd.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlpjbmaz.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxbinjhv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiglvted.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgrsfjrq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gvexotyjd.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gvawstyvr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpwgcidy.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gsymcsnwm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnutxjgn.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gkgliefad.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhfbjstf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/glnnngplh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gybtpteqa.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrdcrymj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbeqdabxz.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsnyeiwjt.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grhauzkuz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfqysxze.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqhfpowu.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbgfrxpli.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzmiymtw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmntfzcu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvpalgzt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyrdjonud.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmenkyrpf.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gjvjrvarm.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghavdemfd.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlayvkic.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggeveldfs.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/geoydsmrd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaosgktt.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeducuvf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdonlxemz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqngzakz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/glhdtkxws.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxgslorj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gqarspcnw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckoedvbu.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoylszys.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gysmboiru.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyberwvo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gnchuvsit.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdhcipxcl.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkgmmjsg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gqstzrxhu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/glmiaxbhy.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/glsdxfjmf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gbexbleir.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvznfjkhp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbblmkmx.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqfzzhe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gbllrkzma.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gqqelgsje.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glrkbmqlz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdcznbxz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnhgtidc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppmaeteb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwjestqh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwowdavq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfojvpkh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gsxrqkpax.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbgsznue.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdniwueyu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gizfzldbl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmudopqax.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbfyqzyb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflybrdwb.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gihoumzcd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gexompdpa.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxduzbsfe.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/goteerrip.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gsbgvzooa.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gqpqpundb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/guswqqyrm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gshrvigra.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxgxsfef.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfwaqiyy.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gfojlxiqu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzzauhuc.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gdbqtujjq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gztmzfvst.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvqklehon.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gscsmkxya.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvxeyyrlv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goajvxvjr.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gftjiyfmg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gcbcpyqyb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbscwwmdj.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtfnyynbl.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gumhvszry.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gybhgycva.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsplfpsym.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeynznob.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwswtrju.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcfpzuxl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpenbmqv.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfhjjgzq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqzjxzvc.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gutkoumat.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfcngvuny.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/guqzogghn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsnkenhy.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gfouxqjdx.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnielia.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gvyjjcmzj.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggluipgbo.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhnqhcix.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/goyowffna.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqrdsssg.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvelxswfl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavtvqbbu.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gjzcvbbwg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfrdiyut.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gczdxpdog.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gxbkqiqaf.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcwujzve.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklecnzlo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmugwvdwt.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gofasbnal.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gcarmdbij.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gobllrrge.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjcuhrsy.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecbhyjqt.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gowvlnypk.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmcgxbsr.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhqzilw.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjakztjde.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggzeglpex.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybmwktql.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gokyzgqul.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gggrhdnly.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gmxwicpwy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggypoikzc.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/glrdftdrs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqpppwksk.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmqresmu.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/glkewpucn.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwfxgegf.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsgxjpuz.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbenjgcup.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gijbphhqi.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gkvkinslh.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gntmgllnz.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkgalefj.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbtrfayg.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmajlubqj.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhcbxidf.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbazjttok.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfxrdmwe.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gaimzybbe.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gyfoqudly.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxnqizobq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuekpjpc.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyznxzdrb.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkjewbahs.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/guusipgnl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrbsrpdr.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpkjxuai.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gshyndwok.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gekjpnixe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnbgmhxa.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblalrgnw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbnstmkvs.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzsjotxpi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfezaggtx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gprxhphtn.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbnplgpo.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdkepydc.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpesnmvpy.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlgsllvx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcoxbfym.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsotdtbj.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gcpfzgpwa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genowibvp.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gulmikdsm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmutzhn.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gtryljmjx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggivawzib.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmkshpiv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gramexrrt.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gugjafeun.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gzcxlmvys.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/galyuzzld.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gkyxltfyi.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gxkoqloyq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gelnqyirn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtiadvqzs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gzlolsrna.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gryrnrnaj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gzslskkzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjjatcuh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gmhdaysxg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhkitbjg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghduxguhy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpspfpey.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gkmyiikly.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gxdboemsj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/glegxwtfa.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gikezcyal.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeqkzrnw.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gakrbyarl.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpullvycz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gtsvhiwzq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gomiqipnj.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuqkbzxo.sHtML


<!-- 参考信息 -->