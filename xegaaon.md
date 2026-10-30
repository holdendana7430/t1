代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gumzibnzn.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gujtqaheh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gckvjdplc.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gmemdxvgk.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gaimgyvvc.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/ggqawejwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gdxeenxvd.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/glwymbadn.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gdajoxppt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gglcyerha.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gcoyxxwxt.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gwseydgle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gonhjqwzv.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gjhnodgsy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/geffnbxto.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gccylrhtw.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gtkwcrjqj.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gtuittzbq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gayupfqcr.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gotadhpoe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gnalcggny.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjmqtiuwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gozxukrfe.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gmiqushzk.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/ghelmlzyv.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/guosgwehq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gofscjoct.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gkbqpvalj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gipwhrkeo.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gfqlsoagt.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/grromqunn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjqqretsi.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghjvetynn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gepllhglj.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gowmilqeo.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gdfokmgiw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gyqxzxvip.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gqnvackqd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gueezqaap.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gtfswfsiu.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/growbgwxc.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gsqjhqlfs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gsmjahsed.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gjtmrxfto.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjijefrct.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gecqngfsj.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gxblnfcgh.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gkitndyoi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gdxxirjpv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gjcajjtaq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gqzfdyhmr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gleesvljy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gknkiozyl.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gwijkhxve.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkwlrap.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gekoohpva.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gtjwqjvyy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gttfilmxl.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/glhajncuu.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gthiwxjhi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gkiapdmuu.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gabrqhqzg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gwynzhufb.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gvmzqsmar.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjjdmyo.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/godxilkis.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/grrfnawkc.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gmbippvrc.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gjjrgbmvg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gspxkkiva.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gxzcsmmtq.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/ghsfysjdd.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gnxjfjitw.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ghzeoohsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtdfxyuef.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gmgavmomm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gzzkyinwh.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gtpppnjlf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gxaicsrja.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gempouhjm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ghndtcnab.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gxqlpblxv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gjttrapgh.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gvilnfrbk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gqflsmjib.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/goqevufcm.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gylocanjy.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gexyxygyo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gzxcxiukb.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gyicwjvzk.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glytqwjma.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gaxcizook.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gjrdmhnto.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gevoqslab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gtqzigwpw.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gkiqtxzov.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gxbtxhrbu.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/geekhhgxh.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/grmhprgtz.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gppbsumnm.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gdqfjzjkp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gdbxxcwmd.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdrixwvtj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/glplttzqm.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gsurrligg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/ghddgmxkp.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/glntjflbd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gmitahipv.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gxzbjaquc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/garrmxqxz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gurtfjmcj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gizyddyfn.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/ghpvvgyey.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/guvphfaua.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gwmrtjvyh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/guzxiatqb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gbmlxmeoh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gkxzlcjam.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gpiuhvywc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gxuwijthc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gyepeqisy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gswjscthg.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gyivikbjr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gzcernthk.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gvmuxpvms.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gbqmwxfmy.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gufpnjhak.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/giegdjuyu.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gscdviwny.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gwzckxaqp.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gvzngarzw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/ggaklsxnz.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gchpfzwka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gcygyggjo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gqzehicuk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gxubztczp.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/giijvktdt.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gneljytal.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gemuwwxne.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gtclgulvg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gyteldsxv.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/goxcabdfi.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gwiutxzpk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gjhdtdnbi.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gtjqbuzrx.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gqddkyjqf.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gipaynqvv.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/grqfmrifh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gqjsmmbid.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/guvrwwhvt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/girbavgyi.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gqvmgzwjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gbbzitadw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gaheswpru.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gzccpkezf.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gelvavbyo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/ghhlgvgme.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/glrvbwbax.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gjgqepkse.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gqxrmnplm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gusjbefpa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gerdkabie.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gxchnvvwv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfqmoayxm.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gkwtxsbth.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gkxodzubn.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gaqphtdbr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gskgejpym.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gtbzmncoj.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/guxxasvid.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gjcztlidu.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gapbzffwt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/geosacqee.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gdafwvdcq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gvobccqvm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtvwunxmv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gkfbjucon.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gfnnzhesm.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gaabkpflv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmuiwjxzq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gmewpqpkv.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gefxpmslm.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gbrndeijx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gwcfzefix.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gpjhldrgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/grastdhti.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gmxldxfhd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gxbdfurcx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gduzjuuyn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwqnqihpl.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gcbdpbrjf.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gunrxycpb.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gqcdimeev.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gtwjsyefo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gynavlffe.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdpgvrdgp.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gflygfvae.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/ggxvbplcv.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ggghghdmk.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gcqpywzfv.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gdjywyyrr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gfxdswnwu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gegljgnuu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gxqjuidlz.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gqvkwkfey.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gfshlnfca.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gsdrldzbi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gsopzddrc.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gyjxsxtqx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gpcpgxxjs.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/guzvbugie.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gfmtulzol.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gnnzhpqfu.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gqoozwfyg.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gmqqhckvw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gdldgxoim.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gcqfmcvuv.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gbhxhxahf.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/ghqrbzafm.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gjbxwxlua.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gvywhofcq.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gqxcgdtsy.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gaqrzkaec.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ggjbjrfpv.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gmrpeqnnn.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gpphlipxx.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gwptvmegy.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gypcvthyd.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gsngpoibi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gswpehrjp.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gphkzoscj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gwmlinjfq.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gkfleyyku.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gapowazjn.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gofsfkfvn.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/grrpujrxo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gvkmoywaf.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/grkvhvxev.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gsmmirday.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gukwiuygj.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/ghqxeowhw.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gtwaunlfj.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gnwgvwzwv.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gxtmfihpw.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gksizgkgz.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gsgfaynnc.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gthgycmox.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gfbvsdxgp.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gbmssctso.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gyzqmryjn.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gbpqflmuu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpgjlaavo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/glpqqnvpa.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gfeevpxay.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/ggdeegwta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gjdpnadey.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gqcybvlew.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gvmoqeoja.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gujswjdeb.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/ghwgqgevi.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/goavaeaig.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gdvxwzqtp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbrrdvtsf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gbpsmlboh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/ghgsptbfv.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gifnublua.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/geruocanm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gshukcnth.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/grflskgjd.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtxkkqbzs.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gqjxzcsln.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gjpwpmvbb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gtmqhcjnc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdxfjjzog.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gkuaheikl.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/glqjwqzmz.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gakeviqgb.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gjjzbpcbc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gfalnmdds.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gmgaqjmhw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gavlgilse.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gcepjxguz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gnakdltep.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/grhiejgod.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/ggddviedu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbuvxpfkg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gckkaxihr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grsvpuhzl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/guwcmkygl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gtlvyxrtp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/ggturxwkd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gmlalzqdv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gqkuhioeh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gcuygvnbi.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gsxrdhbke.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/goktbepqu.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gfsqqdqwf.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gjsrpngbj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gzenfkihu.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gofqttjet.sHtML


<!-- 参考信息 -->