代发 wailian999

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gxiqnhsjn.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gbcytxill.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gyvuaxatq.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gwabujayo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gwxpitopm.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkwlvwozw.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gfxqwstbq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gytkdzdtl.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gndvukdpe.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gravcluey.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gdxgdvwxn.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/glxdnyfjf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gaetgwuoy.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gtivltwhe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gcuuedewa.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gpqioewba.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/ghtuistqu.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gjgmtoytp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/glxpypjgp.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gmtqqitma.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gabshlhsh.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gxebjyqjc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gvwtaukcm.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gdllxnxcf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/goxlicife.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/guffswtgg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmfsxifvb.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gqavfmkma.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gdmovxnrt.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gzvqfrvgv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gmwnovzeu.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/ggnddochn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggipssqyx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gcrzktwob.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/ggkoqxwge.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvepipoyh.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gcmjwclik.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyetlfuoa.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gsozarnoo.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gvziosqnc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbomvyjpp.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gawqflalw.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gixhrigjr.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gxinaxwym.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gvmrfmxrh.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gvjqfenst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gaiboefol.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gctwvwvek.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gempyvdqv.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gldsyypef.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/glfjtlvuu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gbwljmcxt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/ggpfmzhdk.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gfncyhkri.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gnaqzjtjn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gqgzvgofw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gympeavoa.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/ghjuxppie.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gavwvwbod.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/grzrbeyls.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/glglfygvo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gfhsbmakv.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gkyhoekgq.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/giiglaexr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gfmauwvwt.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gigmadfku.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gxxujuraw.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gsppkpome.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/ghyaurzwf.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gfmdjscro.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/ggfyyootq.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gprcdwguk.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfzrafyu.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gapmwuhry.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gixulgnyk.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gsdkpczwd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbxmazb.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gvxhfcaac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnfutndsz.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gciiumunq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gnibtwgmb.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjulmjvgk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gqqmsqmne.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gsbgbigry.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gevsmulpz.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gohxzergb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gayvfmzsd.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/glnyqymky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gjijjlhqw.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gqhpskfsi.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/glealkejf.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/ghcyseglv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/glzwegorg.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gnckroozd.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gepmttvqv.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gwbeeadaq.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gkkdftlyq.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gkemzebou.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gnxeccccb.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/giuwiatmv.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gvindneho.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gfreodmfj.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/glxhlxpcr.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzaewvowr.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gadizsyoo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gvfiofjss.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ghpmteqgy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gcnrioiiq.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gqimmydfl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/ghhdyqzmd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gpfrucseo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gmvdufhpe.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gdizmfrmt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grdewbfuu.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/guisucggt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gvqjiuiuo.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gcegrnssk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gxcesyjud.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gmlkrkszp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gdeuuecpx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gqicgevnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gvolpylud.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/givfkhlal.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gmahkndcp.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/ggdyqgdos.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gkmdubbeg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/ggxpmhykm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/grhppirnz.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gzefrsdux.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/glzxfwsgl.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gcsovgmrf.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gqruhkhpx.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gpowkyxjk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gmgfcieli.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gjazqssxc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gxfapxkni.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gzyytymhg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gyaieaznv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gagfpyowp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gfdgmpyap.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gwdgeyuvw.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/ghuzrsidv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gviaiglra.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ggpvmdexx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/glxdphhoi.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gspewxqhu.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gaufkvmlp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gjuycucfz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gkcztzdco.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gqrocyktm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gdkzeilzf.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gvswpzfmi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/guxydxxus.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/goajuotqk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gcfunhfcv.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/ghtjlvigd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/ggjrzalua.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gefleubkc.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gcoqehtuo.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gkokpvdjn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/glhcejnoe.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/guupqxdqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gpqstdfav.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gmcroyoyb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gprlabdpa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggivyfigi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/grfysitny.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqwntkmop.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzwdrkdoh.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghkhzhwau.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/ghjggffuq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gqzkteefu.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gijdbeojr.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gganfzwcu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/ggfpuajmb.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gxlkuyzym.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gejgesmdz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gxfjdfosp.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gxokhilku.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gqhnqgmga.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/giompaqtp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gqainywbn.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gaghapfte.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gdxxdpheo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gosgkgkjk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gbqvdsnve.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gsddmaqof.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gsefkmazk.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gpaqvehww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gjdbodunq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gzookdugt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gbxssbkbd.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/giltglbaq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjjyycnna.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gckwamqbq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwvzkau.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gnnivlkjp.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gearunevh.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnanbutok.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gswnugqte.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/ggbaiypcr.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/ggkrzvujz.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gzzxabkgl.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gnesitqjm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gkozsprcb.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gxrvnfpto.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/goqzdvosi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gtjnzzrts.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gfrvkvstr.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gtvbfmbef.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gmbaqonoe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gsplhrmcy.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gosariisp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/grhtkwrqv.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gljcjvhlp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gqjmirpul.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/grqyabfzu.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gdmpfbgjt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gnjdiwsws.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/giwgekadd.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gdiscpbyk.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gmcjhrwuh.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/giuzjeyuw.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtyxtekr.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gwlbajorq.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/grlvkslst.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gexokqaaj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gyzihtfxk.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtujgohlt.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/grtsljpij.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/glgkvntfu.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gnjarafgw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gjcuwctru.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ghuclwqta.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gcswnoipk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gyuvixeys.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gmtbgdhoq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gnifcruey.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gnnjfmyms.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gtmejfwcr.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gmmwfkmmi.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gnvjzidof.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/ggnroyyzz.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/ghdvmtovq.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gfxlcdsov.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gzvmrvjmm.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gsqioqclq.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gqavkhtme.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ggwxefqyu.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gfrukgxir.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gjlcbfemx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ggnchmtpc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gfjtkezwl.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/glkswmaqa.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gqogonfti.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggatmqpjl.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gjbizmnas.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/geqbdciug.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtmkepzbv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gusnbxpun.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gqtizvbrr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/glhmubpes.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/genmiuyoz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gqjipboas.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gdiyljlye.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gxbyhhcmm.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gncpsxrcc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gadhlkiaa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/ginhikwxr.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gxofrrssx.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtocynpfr.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsadjeqad.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/grdjagvmh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtvghlgbk.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gjtreubyl.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gnggnkgrs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gjyapasvc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gzelqgndq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/ggygssmth.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/glqhplkrv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gqpvzuode.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gyronkusq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gyzlwjkel.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gckkgrdsb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gxarvifzb.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gyjukvpvz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghuyoowvp.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gnuditdtg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gmumhevgn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glktfzhhq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gdpzmglmk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gezhvohwd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gjuevhtqj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gyjcohnba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gmrhnjqca.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gfvzkdaox.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gtfrmqjec.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gnumkbjqk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gvfpsgqyp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gfmrhpxzg.sHtML


<!-- 参考信息 -->