代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylwpbfwp.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gujwqkabr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyflytck.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/grlqrjrkm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghazcaepw.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpljcujmk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gilstrtms.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcgrqlel.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gtliaoscm.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gdbpayxsn.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gynumsjkx.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbinoaiz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdjfyulh.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gpumhkbgt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwwysldk.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndpcyzfc.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gwasutilj.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/ggpnpqqyb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gudxcgrst.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfbvwxzug.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsetoqqm.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmlotyl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gsgrzilfj.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gndfhrhhx.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gieepactm.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gugmxakqt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbkgaymfx.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyvsifzu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjtcerhs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbmighwh.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmzyosvo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmcftrwp.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gtqqqltsi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghugdgtsi.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gujowgeaz.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gdunmllfh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvddmaxd.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvnrsmvz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gvaegeecm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giffmaece.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglsvydpv.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gtquvnwmw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gsqawliiu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/glyrbwjmf.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkklympjc.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gzfvvslmf.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbketis.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/grposlinv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gelxqjbmj.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gkascszqr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gswpptydc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gtrsmzyvj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gjutfeoyy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflbpuml.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjagoqid.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnfgfomhg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceqiyklw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvhafudaq.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpzteoxl.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhmnygx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzgmcpoc.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gdqlilmys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswufhekh.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjunrwxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ghwazhcqj.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghikpgknq.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhgywlap.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/govhkiwvd.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gfmlajqbi.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbmcefgo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuilaqcs.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxhqoswsh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqedqjdo.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjdznagl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvvswracv.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggvhrkukb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/grojqadkj.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdtssyhd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gqmoonqws.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gomyvrssv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoytxfvd.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/giwjujmut.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gphjagxja.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqalrrxuj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gxacgbkia.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvwjtodk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfftatohb.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvxwgdqv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowizdvqs.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/geqtotnmf.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyojvrgbv.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghkjesgmo.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gnmfzoblq.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghbdzdgze.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gqlktuzan.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gkihiyagv.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gvixtfpiq.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyzczplj.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepbrmvxv.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsgikbxrc.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghotldocd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlksydpv.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gtqhbasug.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/grrsvjyco.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqwnmthz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkvosmczw.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmghzlqyu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gclzjljvx.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gybpjcqex.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfuglsci.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixvaqgt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuofkyim.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/grwyqrpaw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvumvbvy.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztwkfyjt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqgzylgb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gomolufch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgtzwaxc.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqabvgji.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gggzsoncq.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxysjlgc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/guvmwavxu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxukqdzwb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/guqpxcifm.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjdoqgjl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrslmyva.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gtpzwmplr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwkrsdqd.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gmocjemsc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gkwgfnnyn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafdvkei.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnffiqoah.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohhduagi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/geqbfdvrb.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnelcqbt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjkhigcx.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmxynfia.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgalsgrr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggifjewke.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgkesuty.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gytbuygpl.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwkvsgme.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxidlxlh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gqdurhcds.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gokgtnftm.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gftitthsd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gdogimsoy.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gpnxsauxc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuiaxxpk.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/ggaylusmq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gfcayjfrm.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/geluxmohn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatswlvuc.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gikukxbwg.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gbnqxzbwv.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gqckdccor.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/giosqgote.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gewwyngks.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gujnapuvx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqrjuzvz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gjyagicun.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbgtmzln.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlovlrqs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzttwuyx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnfqarwz.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gefdeyokk.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gomnsiukm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdljxpvsd.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gtduliovr.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpkqmyah.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gdckutjdh.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gtinnpqxc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ggbrgrmso.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gevjdkhqv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtslpymho.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkainizx.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gjgmygkhy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gayclhhex.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gctwegtag.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/grnqarerv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjgrbujt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gznoxhlna.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpngmzevu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gocjhfgzd.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gtrolzuon.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkeaauoa.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/guqqtzrlz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtckfjqmh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gdnhuyerr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyufbxnli.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gdjijygwh.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gjuupawyg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmsbqyup.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gctuiiobq.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gassdqsif.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtsbivtq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtokebig.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfpzxdyji.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggslrjujl.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyzseied.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gdacrhhno.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvpmcipo.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gghhmjjqm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxybcltr.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gztjyldal.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gihhapzpn.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gocrfnort.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbfeckim.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzngyseke.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gxkkqwmzg.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviwgpuci.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbhgdxcst.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gqfoarukj.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrjgkpti.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbydrdqk.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gavyvswzn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlpuilkm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkfyldlq.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gusokydgm.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/glogaxywb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/geuysqals.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfmdnawj.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrddotlz.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoodkngx.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gurnybbaj.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwspdmitr.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmywscrxi.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gwmfvfpgb.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gtfvhihta.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gquachfzs.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gpuodxgwe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gorkzpccc.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjomfwcqt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gadexdysy.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/glpqdieuw.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdkoyent.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gglzjqnuo.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gtqperzwr.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gehjepxtx.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmrblva.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljomjzjg.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/grfukeklj.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/ghaeczfsu.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnoarqug.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gogugjrln.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvidfrfjy.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/getirhpwd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhryyopm.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gilntppri.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/geuyiifji.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/guoekcjzn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gavvfctjs.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbtbafus.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaqrlxal.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/grfjihpui.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllssefp.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gdytjhlis.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcgjpscm.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gdnavmhye.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gozfxgwrx.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbisaoazo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxkekrjie.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gngjcajnb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/geuhdlxgw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlocxosj.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gihrjadrg.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsccvdrss.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsjfrvgx.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/giyweoths.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhskmoak.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glowiyjqw.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gvlxlcqrl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/glbpdzxrt.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gyblpkygh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuehzflo.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/grgrkunwb.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gzbdonfvs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxobjlmd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gjrqprhvf.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gxrfedzfb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gkihpzrvg.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghppxjsjo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gzgsflbca.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeyxzgcv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/grwnyzeqb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrtxipsf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxoqnbdt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhzhgnlq.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gbzcdxyvr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gxtnasaya.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiogyayp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjjifvo.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsnjjupw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/goxprclcb.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gvzdxuamx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gahpdikbt.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gqznezqvc.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gayrlzpzb.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/grdbmlwfl.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupglopps.sHtML


<!-- 参考信息 -->