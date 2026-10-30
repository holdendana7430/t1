代发 wailian999

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gglflujwa.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/glkjzqmlb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszlsnzgw.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfhakobt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gjmkjdbmu.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/ghrdlqulj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ghqezwoxy.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/glkutebqx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/grahraylq.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcgmkwkz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdobcwcs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gjzkqdgkk.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gklclhnec.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsbmkouf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gutjtorgj.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gdhfqkqnh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfjsogydx.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbuzhbjg.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/ggftdzjfx.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujdepda.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbqdwgtv.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gqayjsvyi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdtkinpf.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghxouoyvx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxrccvxf.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/giwlovhnh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gprcuxgqs.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsstilvli.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwriulsrn.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtrqpxgon.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gjmrkztrn.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gnrhyithy.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/ghmgmicad.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gubeapqjr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gilkaqfyg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gklnvlioc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtwkdqnl.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefjnpkoh.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gkotrdnon.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/geleisfrn.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gyznjmlwy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnqiqbzsy.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/geljywbjl.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgggmcrn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbgrixpu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzfobubp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwokcqxqv.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnegvobuy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgyeenda.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gliadyuhl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfhlxyod.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtcxhupxp.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebgwadmi.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gztyhnxnq.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gtevqxese.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkcrurlr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvzkmhiqb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjhzvnqv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspzgygdz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/ghiaoksij.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gybykepez.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gqjwrysjx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gfykjtvwz.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuthmqet.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/ghuqvbgof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gikefjerx.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbflcymd.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbokjltwd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gayiervoc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerntdjjl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gduxyjrlu.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdgtnvrv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurfmaqlg.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxgvbbkz.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gilauzgoy.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gijrzxqnd.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gevrhuczq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gagscngnq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgfgmvrl.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gckpwsxle.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gmcxvjxfi.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghliywzhz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncuihzti.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/giuqgpcxd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gnbddyeqj.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gjwxpwyzx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxjdsocj.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkalunfb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfkxpawx.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstbqwlgl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/glyhxsesn.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhxzdjgk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgwnoixu.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/guatntvaq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gqzuvlqpv.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gbskslhrz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gstsvggbq.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgyweqrn.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gppksfbjt.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxaqygck.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqczujfk.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gunnuqpes.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gznxilzul.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdobbztl.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaixcbae.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ghcnuxlra.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gpcnnbqyp.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glzjamuuv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/glaebqmvr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggtidsray.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxunvqzxg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gedquvopb.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gliniupyq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gjgmuvliu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/ggvkqbslm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgkyfonn.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbkhozzd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/grawiimri.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gekdhrazd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkukwxrmr.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkennura.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceiwnsmt.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbxzwqqip.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gviaylmtb.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gimmowjbq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gaktvhwyd.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsnulcfzs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvchqobbr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfjqnhoo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjlrtrmm.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gntjxoryf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkzipbyz.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gswleqqai.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxdtzdxy.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahqlnxi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gavitoyrm.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gutzgetpf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gedvsgoft.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlqtlirg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjzjutizq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grchaxvcm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsdkmctxe.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gidetrfuw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gncvbyzhk.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gckqjkool.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrmrrkcs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbviclfq.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxddybqkw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghmcqpytb.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdcgdexjc.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gvgkwrtyf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gofxsnvmo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzgbcjgt.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gdniqnock.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gzisygbwc.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuiwykqy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gmyxmpydk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/goxwzzfax.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjotyuzl.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/giyuwoqfs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqamzfhpk.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gonverewi.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxoggoysz.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywcoyyxd.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grolxkjav.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gjerxbsfl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvirnndid.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxenxcuwg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gxogyipci.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzkgpcnov.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gldpcrohw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtinnogla.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfuzkkzig.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gzwkwoxpx.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoddcbde.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepeoghdm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gelprdcta.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/grtdwwsra.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxfdtjtm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqtysngj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gclbpfswc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnsbmvus.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsowgvqml.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxldwipgd.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gseceopld.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzlrjspm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemytadrm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxlegedl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwleaiohe.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtynywpfk.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrwyaquw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzlavtbr.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gemnjyvwl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrhpnljp.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnvfwugg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqhaxnwaj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/glvivvifm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgkcyfyh.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpqkiumo.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcshlfizf.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjowiojf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gmzcbgygd.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhhbilrg.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyffqrnfr.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/godxvxmbl.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghxstrelv.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/glezrmdsi.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gsbrqqeal.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/guhshoddh.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwwevcym.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznvfgmum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gbqwfilxa.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/guhwddjdo.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/grlflpstd.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkkmzjpm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvxiehywx.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggyhvbkgr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsybpvere.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/geincxevd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufuuinwz.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdgucfdi.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/grtdhfxbq.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/ghonmlffj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghasufylq.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gndzimpmm.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqmtvbfqy.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gywxvzquf.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/grfxfhyhs.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvfblgiy.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpohcucxc.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gsjjgzonh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/ghvirbpwh.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbfcioma.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ggjkmrsbq.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtzrzpwsw.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtkvllth.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gklrnmgsl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufplpzuz.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gvfoznkcy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkoqmzwl.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gprdopuws.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcghoozas.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gughadtko.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqospzjaj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/godawamgu.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpyjnxxb.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gshcubuak.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/geoxfgodi.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gslmxjzap.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/ghabdsqlt.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtctpxngq.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gsqflpuaf.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjhstnzpt.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glebaycaf.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtnriwax.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrbnabdj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrwvchvq.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipqjgorw.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmpcedk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvmbmbdz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glarpfbgl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gifeaziad.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqopwuuc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpbfucws.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnvsuayj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gagkqjrim.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkfayymg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcvutppe.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guuogqhlv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhoezfch.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymkvtybv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrbggzet.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkepigiju.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyhjbjgz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdcignzx.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqaglzvv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwewojvo.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvhfqedmc.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gupyoujgq.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgmjbwg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvuksumdz.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gteezbhkk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnleqfplf.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/geqcyahsd.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/grddrcdwf.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gdrqxegax.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gukurudtw.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gocysuibg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvmvcbbq.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqxzmnmp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqjnfnkv.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gbcftxiha.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmevugcid.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnamtzdbw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gautvkcpd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geydodzny.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvcbpnbb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqiwuzvn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gdiulbjli.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsvkpmyoa.sHtML


<!-- 参考信息 -->