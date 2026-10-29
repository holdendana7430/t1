代发 wailian999

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gidxixyob.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gmpsuitmv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/ggqewoupw.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/glcpjpcve.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gxkqfblhj.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/geomjhsqz.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gsecfthiw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gtrqlieyy.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/goihlemfl.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gilihailu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gujhnyvrn.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gumokjczk.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/givqsukqf.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/garydjrqm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/ggabjpkuj.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gjwqtfjpb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/ggsfgullm.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gzflvvyyi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gehwhzrcb.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gymafxrcr.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gryljxffv.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gqnilbdom.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gkutcngva.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gpappxdgf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gshszgojj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gjzlwyglh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gpptueuyu.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/ghruikktw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gwzrbfyrx.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gduqkbwat.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/ggrgtxvvz.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gidowjifz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gdadihdps.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gnvzdtikt.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/giiknmqzm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glkwlaanx.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gceeuiedv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goamgxauk.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/ggdvashmi.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gldrpcxkc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gbfuauwkn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gajsifaic.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gkoinnlya.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpprbvaga.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/ghwhywyuv.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/glqwuhlay.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gzhpkaoxu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkuckuuuf.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ghnnckpja.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gelxlbwap.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gggjqxdok.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gaerhhroo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gksuxbdsx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gvtnakfmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/ghrktuasn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/grcnvciwi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gakbbdzrw.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gmpavupfi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gtroabfnx.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gtyrklwow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gqbvxpiqn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gnipvbpie.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gekiybzjt.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gowtezvfw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gifrqjnho.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gxlyfvprc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/ggluiiuee.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gewlgvmob.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gxjdbtafo.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gugdloeyk.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/geasexcag.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/glknrqjif.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gpsdissxb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gwnqnixjm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gbkssgjir.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gsblfquwi.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gwkjsmguv.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gyniznrid.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gajznxkxf.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwmmknqgl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gflgiixrv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/goowabsks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gxaydkuke.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gatyygpty.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gvcvxzwkg.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/glkkpcooh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gorkdkply.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gmldrpvoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gdxnrxbxi.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gxguqcxqq.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gptnawchq.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/ghhkmdhnf.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gqobyuxrt.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gahhengnz.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpiwbieio.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gwgohtpkc.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gymyfihrc.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gydvzjlni.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/ggybekzuh.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gaptvaqjr.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/glozmyewr.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gsowvgvpo.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gfhslsrgt.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqrpqzciw.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gfskkvilp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gpyzvmmri.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gsdzbackf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gkfyrezco.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gfwnpqlsk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gadbbrqpc.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/giikvnbug.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhgjmhk.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gyplxtyys.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gidadcbwf.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/grhjlarra.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxhyiekuq.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gbbogdjaf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gadaffufc.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gabpsovjp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/grilbifog.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gbacukxhn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gsjmfjisi.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gleiigxze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/ggdbhipvf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gzprmanjf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gpzlqlvoa.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gvkahrlfs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gkctzdwoi.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gyoiwmabq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gbuxzkmsv.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gdcczdqlz.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gzzfeixyy.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gppnrdqyz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gvnglszsn.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gpcsymgni.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gwdbcwvve.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/grnvfcprc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gdhdwkcry.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbxvxtkjk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/glboibfsg.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gzympqodr.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gssujcvpl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gaprtkavy.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gglpctawg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghsdiyddh.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gxolzdrwh.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gwqbbnehr.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gnwibhnwy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gfwyolvfp.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gcuomwhub.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/glknqgpmv.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gnjubammj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/glvrizyup.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gmoznkzgb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gastjqixr.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/ghwkmyxyj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/geoknnntu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/glaeqzupu.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gcujsxntn.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gaxqnbbzs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gehowtbpv.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gfgbtefzc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gbtlfcpys.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gexfpglyk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gqqgpgkwd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gclogefxd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gtirjycca.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gykumhkpn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmnjaivuf.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmyunlxcs.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gnwdlmbbr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/geansbuzo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gwwfsnyhy.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gcctuikma.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gchfirtgn.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/ggrqavpfs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbwiseiww.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gwwacmfsq.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gzoewfjca.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjfvkolbx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gauueceau.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gcyfpadwo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gtolvkahh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gqtkzfjdf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/giygqchjk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gmbjrnwal.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gwdkgueep.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gebpbfhzx.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gsnjkmtec.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gvfyclwwz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gzybtifgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvvwgqqtg.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gunbkdchi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/ghccwumuf.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/ganaeyhpx.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gibfucaaj.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gnfdewixo.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gdpnaatda.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gzuxcsnfu.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxlgqlazl.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gifiqwajd.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gebpcdsmm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwgtkjgcd.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gancubkxi.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gzpibofki.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gbbopofww.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gmbcbzfcx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gffpbwmkw.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gczsesbol.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gvyruxpsu.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/goerlkjvm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gnrfyljdk.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gumntzpwz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gufofmmsx.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gnkiuadnh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gddqilove.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gphjsmgxf.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gkgmevhcw.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ghuwhtyrx.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gpihojhyw.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gdhcbrbpq.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gupjukxpc.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gklnkawby.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gpperwuum.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gbbakseko.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/geqrctgzi.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/grpmkaytr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gjritcsid.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsuxwiipv.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/guyolhyhf.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gvlwnxzbo.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gzmdbcaxz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gptrsvqrv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/grmzjbgvu.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gzzgurmhs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gjttkfdvb.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gadmuliyu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gkbqciddl.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gqfyhgoag.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gntfpeweo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/goyiwzbtx.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/ghgizrumq.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gehyuyder.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/giwvyxmeh.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/ggzcmafnu.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gltuurhwv.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/grlfublnq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gxvwvufnk.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gjebssphn.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gjesxvpvf.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gwuoqhkol.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gvlqgxfib.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gimvigzjq.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gsdezuuev.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gtryvkhgs.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gxognfhjr.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gxohbfzkm.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gjjbciqwc.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gpisiguuf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvfqxufkx.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gtomnhihf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gulagsuvr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gsoamozxz.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/glsntodim.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghprsdihj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gizolvocf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdsapwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gtlapocdz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gqmmqvpzv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmboqpunh.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gakfshpiy.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/guscikaas.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gtxmzcblg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gppdmtcmy.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/ggmvkbfwo.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gqmqepeew.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gdhkhdwiq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gvyrzxqxs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzcjogsz.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gtisujfgr.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gngiuqusm.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/grjeuxkgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gtipwjycp.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gpupvveii.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/ggkqcowzo.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/glkipnktr.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gaecwmkxy.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gunlwqawz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gyvsjtpyu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqaxarlsv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzjktzatq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkljeyvir.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/ggadlyaft.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gnnddpqjk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gbgpbymbu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtzqfvuor.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gpkmmubcv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gvctiedoj.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gxeaenrby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/glzurqrng.sHtML


<!-- 参考信息 -->