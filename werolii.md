代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gdclzzpdr.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gvtgymhli.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/ghgqpnavn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gtqyzmjun.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gnkdbxdee.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gjybgvlhn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxpqffxel.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gtdduybnu.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gqxomwykc.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gouzxlglt.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/grewjvxhk.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gqubxirrh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gidnrmyxh.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gwgpvphqz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/guiikjpmd.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gpqedpykw.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gptmchqtm.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gmstjzkks.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/grjokdfwz.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gpwpokbrn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/ggespyqzf.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/geoigmsbc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjskqreoc.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/ghbwuavkq.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gyydoudiw.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gwdlhkhsa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gbwfulqvs.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gmcgmcutn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/ggteskvkh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gfzgslght.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gxlgxwinq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gehkvzzbh.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gjoqanuon.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjtolpvcn.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/glvhlfnqf.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gwhvsycof.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gltcslpbk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/guzdilhwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/glhqngtsh.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gpfbgmksd.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gfcxajpnq.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gtdztepdi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/goetmgbhg.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gqdthameb.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnmobofas.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gakppqqyy.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/glzfuvrtu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gifbdwbmg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gilqhhfzv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/glgfmbgkc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gguisciqf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/ggwxymlse.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gmzjtwhpj.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gehlrsvey.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/grnsfblkv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzhbaysyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gelkahbua.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gpcoqasep.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gekpfdkqs.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gynlkkqqu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gdxafusbn.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gssvrcgau.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gqgtjlnkk.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gemfchfzu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gawwcmagk.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gavlnjrmp.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/ggpnovewp.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gyeikeyzi.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gkwyyxhcx.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gzljgenqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gbdqtgvbg.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gmvjstzei.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwtmpup.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gndvjwmqd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gcavapipy.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gikozjoya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gxdiqffzv.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gcyubzjqi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gqxcxqlac.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gdksozlgs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/ghmljstkg.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gyzwgaknu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gubulikha.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/godrblkca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gedolklra.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gsxynjlar.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/golujytlm.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghysjnfef.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gcilmsudw.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gjgcvwtyl.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gssktqbho.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gkttyvuyl.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gmtxmhrmo.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gbntbfsfi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gbrqgedyf.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gzhohcivz.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gnqageste.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gpziokkjy.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ggnypbivd.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggvvehgwy.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/glgtnkrye.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gsbttusfn.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/ggafvoejt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gpzmalgih.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gwpxzdnlc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gzbbbyyit.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gffmxcwaj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gmawvvaqw.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gnzaitsth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpfonpics.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gchxviavs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gjyducmhd.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gqpcflzlv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/glhbvvumt.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gnnnskikf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gvincettd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/ggsnbazuc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/ggnafazyt.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/giftxccbt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gyxubdhsv.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gzlnholkq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gdwfettjf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gtyvusafa.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gmtnkijwr.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gizbajnaz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gidfadxnm.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/ggmnezuub.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gjczeedeo.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gultiszuo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gbqgvfryx.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gyduhjlvr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gqjnividy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gfcuskgze.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gmdeaprdl.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/giqxpcxwh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gwojqfvgt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gpnmrafbd.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdfuwgaji.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gagdasfor.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gpnhjfqge.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpnifctmq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwdxniqdk.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gsuzpfedc.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gmwrvcpyp.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gadleufqf.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/ggygrqhcm.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/ggnluhytg.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gvkojnyaw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gzrxzppta.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gmohcrwfa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gmwztzyqq.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gmvmqvfco.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gzqzqzify.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gqxzzctdi.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqjajksmj.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gpwkafqyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gpiyvxkre.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gsgnwotxs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gsozozsaa.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gbbdvkjri.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gtrmvkraz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggmrghsnu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gmnfiboon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqyabndto.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gnbugkkfv.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnteiglgb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/ggqtbzrly.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gzhgwblgs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gumlsigtu.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/glqpvrbbp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gvckzshtm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/geygptozf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gylrmwkaw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gmjqvhnfc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gisatvrxi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/glstvbger.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gsyhoiglx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gnrzaycuu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gqioflytp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gdjohkwtq.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/geqcugnoi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/guucbazid.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gexqyjpfe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gnfyiussb.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gkdyjfybr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gjzbgctfv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gziailoox.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ghsumebxi.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gtlglryrq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjjzjjugu.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gmtazfdxs.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gygejkeeh.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gppoykopj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/giuuwausn.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gxencoshx.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gtlxycptk.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/goxiezzoq.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gsbzyuvlb.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gohudoefx.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gblrphaqc.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gnwcpvqhw.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gfkbafgjt.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/grvwcbxaj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfvfruya.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gdsiwsdoi.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/glnwvdmoi.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gbpnhxklf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfgqmvvhz.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gcegzdmsp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gqhzktwcc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gbahbossm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gabvktqvp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gqfklydyy.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gsodwyqjc.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/geohnwbwj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gutxdxxxk.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gfmcomzca.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/ghjfzfyuk.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gatlekfrd.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gwzkmyzuu.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/glfbplgva.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gfexohyft.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gqjetrzdy.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gbpjleexe.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/guehylvxp.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjfqyqnfs.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gsxgghxmf.sHtML

local a = 1
来源：http://mobile.fehbvm.com/Article/details/gydkkbwgr.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gbvynmyvf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gtyqayjfi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/ghnnzleky.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gmpdynsgj.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gncdilads.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdfabickb.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbhlmkieh.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gqyokjxxm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/ghxthwevp.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/goikeeofi.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gbsvkiode.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gytvkuham.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/giizxmowy.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/guatrpfbi.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gcaakdvzx.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gtmikvbhd.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjiumwnkj.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gobqgxrhb.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gzauhxggx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gyjybxmmm.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdgizkzpp.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gllcljjok.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/glknohvwe.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gsvwqkprj.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gzfkggmsc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/giohsxeen.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gxihnihja.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/glxnlwqnw.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gttlvwdxa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/ghphjyuvu.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gcpwcpagk.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/grvstxwfo.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/giaoprspr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghvxmmoht.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvkmcenft.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gpjtyvxse.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gyhkihham.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzedfgasg.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghzpjumjk.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gexxbfswq.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gvdlqcdtu.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gxkqbwczy.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/ggzrmlzhu.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gmqxqsber.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/grigrkqzi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gqmtdyfik.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/grogjrxsa.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/glbscphcb.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gymxjebzo.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/guekpqjdo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gwtblcstw.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gqiocxdpa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/geniylyho.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gjpogduzf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gpzvsfwhf.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gwwvwlyfu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gjisjmxcj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gakqykfow.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gbyduulkc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpzkhqnje.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gtfbzojok.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gwjnhxteb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/ghyuwkmat.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gwkkpkfna.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gsebhzxir.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gwhyovstx.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gcpsfelxx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gndfvaudq.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gtffezrvl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glumbfevt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gvcoxslat.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/glwgodarg.sHtML


<!-- 参考信息 -->