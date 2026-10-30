代发 wailian999

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazqbzrxy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdnutpt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpswlgor.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuyetrby.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbzhixvd.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gtdionbww.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljflpiqn.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgtjqrug.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdloawqkf.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gmxiwaeql.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gterdopgw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkwgswxu.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gscfewdci.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gclzziicc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gflhfnnbg.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gecqpauhx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqofmocfl.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlgjneqz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gghmyfepv.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gosiwwbnc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjeflqqs.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gatkundas.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/guzinbqjo.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyvxmhlvl.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gaxctbwwm.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ghxwwhpkw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcipudqc.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofzjtsbh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gvbjimacs.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gormrysnr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/giplfqsfu.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/grdoldmwl.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ggiclyjrr.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gtspplrun.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpoicnbbk.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmvaqhvb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlqfpvsv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gggmttbwk.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gooinwavi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcovoqtg.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gyomxzjoh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpqeiuvcg.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/giuoeimwd.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbawaxloz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsrniasb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gllunrrgd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnyiaehm.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girulenas.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmuvfetc.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gpispqitq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/glyzoiaus.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnwztznor.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gasiwmdyw.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzxpanosz.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gjlwpkzaw.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobiuxhv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gycdlmrcl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gykgverpa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gbvxdjulm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gettotuxr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqruitbyb.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gmuaehpgy.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdygdzgc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glgfyjrrg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltuusdow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwtcsdva.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcpgjyak.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqnpxnho.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnpzdner.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvvhfayo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbnhabjs.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfhipdeq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gtrwdbfqm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggultwtox.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlwculbd.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gjtuxfofk.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqywytfiz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzwfpxhc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrvybmlk.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctbzrtf.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpynisrq.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvddaumqz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbyxhtxml.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gakocrhdh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/guelrgrhk.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsfdyiih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjnczoac.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxwzedli.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaufmprje.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gllmuywpk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiljtnid.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gbzzgkrxb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrzlprbb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfyrlwkw.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gogufdjsp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkhkbqgo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqexonqtl.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclccruoz.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gihdjfusw.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcnbbyfqi.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsrdffzf.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnypoxhm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gniywrxet.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxhzals.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttvarqrq.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ghweojdtl.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvubbpg.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gljapuwff.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxvcuztf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gslfvdfdg.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/giqwolxkm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gsuhdivpx.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gvqmysdxc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsrvsnmam.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gntamcelg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafveaizk.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gsstnwlau.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwwtcgoly.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxymdosmw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqzohpy.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gtlgsdurc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gidlnklml.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gopsvarlg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gqisqncyp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudmcvwxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrtokrsg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqxalzrm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcrmlogc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqylidopw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyljrqblj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnmgsuqu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtdadbdr.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gelwijwff.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gafcgofxi.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfppbfun.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxotndhok.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gvaywrchr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gqmovfvlz.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gxdqyqwwq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbhnuupq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/glxmknsxs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwsgufhft.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gweokksmy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/guvslgfey.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grzckorms.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/glkyysqfa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdnzhjok.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gojuwxzmk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiorbbll.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gizjtxxni.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gtovadygg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwlvflnm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glwjgojgg.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gqtmnuvru.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsmahezz.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbflxejvq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoqvegcu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqawlidxc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gknpuabcs.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsykxbzn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlweccrk.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grtfnqjuf.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjhzydqoe.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gasviujyt.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gjlfbtazu.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcrcoafx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gbangvjpz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrsabbye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnltvtyki.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjnwctrk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuuqfpcx.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfzqpsmg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gilghjltu.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzjzkrpdy.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjecvszmb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ghhqpukxg.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gimtnxyhq.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnffclb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgntowgs.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gwnnflxip.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrlcnigr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikngfkgc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszxxcnyo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gathlqfxt.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gecvqmoei.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegexalds.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmbynnhj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwudjbyge.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghttfotmf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdrxqzgl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/govfjfwve.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gneqaqsee.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gckhotuzj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gliracgoj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/galwourak.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnpklubm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gkrrpxavd.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggxrhnccg.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gbtcfgnml.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxqwjgilz.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzrioyor.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gqsyjqtak.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsdptmll.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghphssuql.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbxjbfxi.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvbreefsl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcojsqywq.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gblkybrkl.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gsdxjnfao.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gatpzzefv.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqupclosi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmulvrjmw.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdbhqsfp.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzsgmkxp.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giejitwwx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglitedhd.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcayeyilp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdnjybhy.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppwopgdb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozdfiod.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpwkvhjq.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwihxeabn.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gxtutpakr.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gomoqkotr.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gqescerui.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/ggjturzvl.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjurbjw.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfeswoui.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gnxunbiag.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gpjdrizig.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtkgttrr.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gggiyrydl.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gonirawup.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvsbrscsy.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqmpmtnb.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyrwtuca.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwrxqiae.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/genmvyroy.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gagivmgva.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsvyzpon.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gkielyxzs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gaolaqikn.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkgnbyok.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkthxglc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/grvadvdxr.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhcaiqht.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtyuvlek.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gjjqconsd.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gqfazrzem.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwvhdkbr.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gwkaciahk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyzqxngk.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gprghcffi.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/ghnwwwjoy.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gplbakzzz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnzryhra.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpopppjk.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gzyncxinl.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonplzar.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glznmxwxc.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grwwxkche.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkdqpcxxb.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/guetxggun.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwghnzwei.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyztewds.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guokokchr.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/grektyzet.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbjrqzce.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtjpcorkn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxnsqvzb.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnroaivl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gynczhgsm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/grsxypnzs.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gchzjjvlv.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/galvvacrf.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxqzjwlt.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgnfakdt.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtclgzaaz.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrmjyskk.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfhywbip.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfncakk.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gjnmqlsvj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnpwtkous.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gnfpfvlpj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowifodhn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gouwblkua.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gerzmwkjz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaozuueob.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahridclf.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxhgtkgg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gjiskjtda.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwobvgxs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcskedgd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvyappvkf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gztbwumkb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqmzqtudb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/ghcefaurg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkivvrx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gtbvvwsaf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyxlwnjl.sHtML


<!-- 参考信息 -->