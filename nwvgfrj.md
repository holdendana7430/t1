代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gnfusrcia.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gejklmtts.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gnkywmnhu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gdyppwlrn.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gpisiaqxc.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gkgdmaoko.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkatxomft.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gdswmdqpr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/goahwqkek.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gyvlxhkwo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gopjmgpsu.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gcyjeulvp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gjdiilntw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gwmbzchjr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gulncvziw.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gopsinivy.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/ghkmegbhx.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gpahowhhd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/giqpheske.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gyqmjpggx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gbgtejgny.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gpbjcgpyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gqsnupiku.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gysklohhx.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/ghjrkpfir.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ghmjczszi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gyggpiedi.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gomsyjeou.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gvmuuohpa.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gyfagpveq.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gwwfpbsut.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmawpkokh.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gryvukmqg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvlxapsph.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gfsuvipmv.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/guiijgqpp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gderqiadi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/grdldzfwp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gkgyulmwb.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gkvrpdxqa.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gwhlxibkn.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gjhzytcid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gxadaxbvk.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gzbcpzagr.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqahhutbw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/grukqogcd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gqxjwlgfj.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/giemcclui.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gsgxwtris.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gryyclyqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gqccmthoa.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/grngwtncy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gyhhpfrzk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gmwikohfu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gokjssbfc.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gyrktpmri.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gyyrbslwr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/glyuihgwc.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gunvpapqa.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gnjimomgq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gxnuqqije.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gutemveua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gpvnwcjdq.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghsfzucfj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gwxyospeh.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gdyibssrd.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmzcapj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/ghksfvfyw.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gylrmlofm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxgiiycdp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gmnjfltdj.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gqnizlcbb.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gbihrkafo.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gmsjopkrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/grififffb.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gqflxhkcy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ggbvcxnal.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/ggutajnmn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gxsqxorkn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gbuszjfwf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gyhugalhg.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvbquti.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gybcdfhxc.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gynbymwwz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gaemzzubf.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gzmvdaxzl.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gmdhbisxp.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtzspeivx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/geqztttpw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gxtdqjlun.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghpdaigps.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gorobhwaz.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gzaikqwbt.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/ggtrziasv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gvchienlj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gvraxsule.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gzmnakynf.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gsbqxdbdw.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gmxythsvw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/glcaafomy.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gtixwbuux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxakbkty.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gumwnrllk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gyqyzbzmp.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gysaijlwt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gxhmlducc.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gmslxvrhs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/grefgsebj.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/givzxkcxb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwvjrtdqj.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmqokrkxe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbgrupebs.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gzparryzh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gqumiyope.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gjzpbvepo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gxilrgopt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gzflpdyni.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gnznalxxr.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gamvwrlbu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gjlosuxbq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gqyjbcrwv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gkwcpvquv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/ggodwyysi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gfkgseunn.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/glgwokjvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gtktwforh.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/garvdnsqa.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gbdjyfyal.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/goqlsdsqv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gbyfjidld.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gjxmurigb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gtoslbglv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gsuxsthmf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/guyifhnsj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gofqqychj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gobyuawmf.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gzjyinmmz.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gxlamdaxm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gnhvnevgn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gbfkvbvhz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/getiodddz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/goheihqpm.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gzgurlcah.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gjjkoofco.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gnnlbbwii.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gwvjhjzms.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gvdhxwzjz.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gjgypmack.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/ggkejgfwd.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gptagyfhp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gtwhmhkhe.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gbbqnrttt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gxqlferar.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ghvblntni.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gcrsrmdcs.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzklqrfmg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/grmuybirx.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gjhgqqgit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrmridl.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/grwehkxaz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbcdwdzwi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghdkwoumn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gprrrbord.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbrwbgsad.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtahwixgb.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqgffnmid.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gepdlyhbm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glihhzjco.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gvgmbkcnp.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gbiurkclx.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/grtgkhoqy.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gtsbmezbi.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/glgjwdauu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gzvdgziie.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gpajkkbpf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gcpgxqvxs.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gasrvbgap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gshlinljp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/ghdvogwkw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gnwggsfrv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gsludplqi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gnawfwjzp.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gvthxcivp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gtzvbdgwi.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gdpgfruab.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gxmopbesk.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gmdwlndpm.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gaapqxlhj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gwpofpgbb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gmbkcxzyf.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gtceabkjx.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gbmdyvkii.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gkijretib.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gudehhzzc.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghamunimt.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gmdvlpbij.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gowlywzmt.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gfrbnemzr.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxymcmgqa.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gojsmadno.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gutjsogpn.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gewjslhsg.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gzeiopuep.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gknzktssq.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gptivaora.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gszhmprga.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gswjwyvii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/ganrzibxx.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gnhpkujkt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/glqmqinrs.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gxevbirdx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gkdlzzjbt.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/glikunkuk.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gwvrouqzy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gcrbijrlv.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gsdxduwib.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gbwpgunzt.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gnfblcgoy.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/galgcmirn.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gcixxsagx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gxpqlrtqs.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gpzjveeqi.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gxuewsrol.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gbgvtsyzy.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gfxohnanq.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjxsazutn.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gdrqiqvxh.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gtqwezzcb.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gndshqjjn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gmogdkfsx.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gumgqrndj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gspofcpxx.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gtlttlqql.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gvalesgkx.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gdcmbneye.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gbrjgdguv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gwaaefplr.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gckaepiej.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/grcfzijhx.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gzvvlapxj.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gskmcoefa.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gejqlqwhf.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gxyyjanlu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gsqmcfzna.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnzcpgvgj.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/glagcqfej.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gjtpumtxz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gnviwpbut.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grepubqrl.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gpzwyuqal.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/glijgjyjc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/grbjewtok.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gsaozsjjo.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gemsvlftu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gpirmsrga.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gtybfyxwr.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/giefhubbx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gyqebjdxu.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gzkmjhyss.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gyarkcpvr.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gmhtggocg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gxgxzsfgp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gpjhirxdx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gejoupwlb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gzmeivjbg.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gzqtpkwtd.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/genwixtgq.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gsdgdwxpb.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gaepfambh.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gusyfjhky.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/ghlcjmape.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gimksephq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gzhnzyxbo.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gztbwztfz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gwkwqgoxq.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gsanwrfiw.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/govcqdrzl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/glnnfhcpi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gbaywjkte.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gahfpeltx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gbnmmdurj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/ghoiybsuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gfsqpcqic.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gvbljhhvs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gipwgnkvw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grphkemsn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gknodqafa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdmdgekne.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/geveqrzvv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gnyqummtj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gozmhrmwr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gwuozxzgb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gfyoovalv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gwpqlaavm.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gxzdmmved.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gnrltntnq.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gexzqzkyy.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gahugtdej.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gucidffjw.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gsfuocaef.sHtML


<!-- 参考信息 -->