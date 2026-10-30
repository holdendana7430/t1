代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gmltpwcom.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ggzostunq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gvzrxpzco.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gvsnkqfwf.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gdesougdn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gconwxnbp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gdmgvnbbj.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gncafhytr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gjsmausrt.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gcgvvoqdb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gnjbjatuh.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gpzopcgem.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gvnvqrilc.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gnxipdzud.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gpemopnoe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gipqxnvpo.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gbmiyxawy.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gpodkndwh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/grptdhmgd.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gzxfvkkwf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gzaxfiukh.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gfrawpxpt.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gqmdrkxnu.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gqjqoqaip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/ghecwxvuh.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/getytrzec.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gaxemqnqy.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gujiaergs.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gcfdnbrym.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/galbyydop.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/goyjrdpah.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gxcahkgmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/ggymtklob.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gjjwlnxmy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gwlymtkls.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gwlkejxpj.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gxoenecsw.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gexblqtjl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gbjlnzdox.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gusbibavg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/ghzichtfi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gsjrcvves.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/golwitbfc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjcxnjtpd.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gylfwnqxx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpqtbrfdc.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gzeulvvxb.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gvklwlweb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gvyvbnuht.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gyknsfdoe.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gvhxgzcgm.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gugetdvgo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gwozzznsm.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/guxmyotld.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gpmxudlhq.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gxcrnbstq.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gxcvkxhdl.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gxhkdtrly.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/ghdurrzgg.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gwdtslzgo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gkspxpwiq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gzmwuiobk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/guveufsoi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gzsrjwgcw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gmdlmnxod.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gzyitusof.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ggjoabqiz.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gocjstpvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gjrhmvway.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gilzwhnmh.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/guzvxanqh.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gmcoynsac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ggrbethtp.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gsrbvhhql.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gcrbxeykm.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gheijbnci.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/ggywbwlxw.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gxghrdqfa.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ghsbfgauf.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gxcpuglmu.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqwhsezww.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gkfvtxmst.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/geetqlbkd.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gjpgbzgns.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gsxqywtyt.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/ggwcwimdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/grxxvuzsz.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gcdiggtaf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/grsbqutah.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gaysbasph.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gpopjmsxq.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gutyciwno.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gvygqalhf.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gwxrcbugy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/grwkadkrg.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gdlrpidec.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gzzoetgeh.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/girrgkoms.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gafvlqqmq.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gfpuzehen.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/glmovpdpz.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gsywgdedz.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghojsrdkc.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gvfcokrph.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gqoiiqkyu.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/goozuqlkh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gncbrkdaj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhiiqzz.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gvhqfzyev.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gqlzswrxy.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/giwyktahu.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdncmbalp.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gkcysxmdf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gyaonojra.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gftchdudx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gtnewnnvz.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gifcianzx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gptvkpljq.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gsqbgdfkp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/groinyfkx.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gdnacqtou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gxgcorljf.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gkttqgqiy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtycmzhtg.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gvkedffgw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/guktmbfrc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gstsnsxow.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gvbkrgpav.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/grjxwflfw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gewtxfqjd.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gvmwpcdeq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gpomwlgpj.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gsydyrzhf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gcwnbaoqd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gaxpkrgif.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gzxfzjrwd.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gqpylmbkl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtwrpkuuy.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gezlskjfl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gksofagwp.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gcxeeswpp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gsxwemwie.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gdarlchpj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gictxtjek.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gbgxmqrzj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gropejlpt.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqlziqvlf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gpqmjlbjv.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gmnxhpkws.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gdjqdhxis.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/glityqvkm.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gvfpzsxus.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghpktozwy.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gkdqxyxmj.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxjaeacxd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gkdettuzz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/ggynrjjbv.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gcymigyre.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gtibiuzyn.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gumaugpsk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/geyxyohji.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gmpyiovrf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gzyaqfiql.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gryyengjz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gmzrbujor.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gfrkfniws.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxgfqthhd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gadfmntud.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gfyjtqego.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gctsoajwu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gsvwnftpb.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gnotzwtyq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/ggnszgfnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggqrjrrfg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ggvfisawf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcdmepaeb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtvqhtyzp.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/grbyoiqng.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gyfieeysj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gyoujrdmj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gfhygpfiy.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gfwprpgrm.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/grsdwmehm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gkepixgmy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gldrqytao.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/glulztrzz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gxfpbphgz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzijpoeff.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/ghmteqeyp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gharslnnh.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gpytwvwzf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gdrrfmjtl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gjmfxlrsh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/ggzpwmbcf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gymanhidv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/glvwyxhin.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gwmmmwwzi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gwogxolgt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/ggcuioswf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gztiikzqc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/ghnqsbbgs.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlyujwi.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gbokvefma.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gdevlqbdc.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gajkzvmfk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/ggaswsshi.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqmtwlddd.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjqbhuepq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gpoeqmmyr.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/geovkfzwt.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gxtdcorrx.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gdgzwpmrd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/ggngmawpb.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gppnbaicp.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gezvhqhbi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gxexuycpc.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/grjizqqmv.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gqfslzcjx.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gyvkvclze.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gzanqkqes.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gfaittwrw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gvfeibmuv.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gdphbfijt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gejqhvudm.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gwnzoqolo.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gfkmkdblc.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ggskhrjbk.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqphibbc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbuklutzy.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gxqhsqjir.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/geaevepqh.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ghlmmzkih.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/guojuavsn.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gzokvowzi.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gfrzodacr.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gontxoxlm.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwgiozoyb.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gflbeopss.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gohfuzopx.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gnjinejff.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gvlpunvjm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gcrwhksvj.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gukwbrqbo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gjxjcziob.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gjavpuyfb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gyhebwiqn.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gaudueuvc.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gyzqlhadm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gjjbnjykn.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/guhreaasw.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/ghpvvebej.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gmtsudblv.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/giiaseqas.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gvmpnceyz.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gfnamwneb.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gnrxboxdx.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gijbaewbi.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gjjmdkdox.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/giptcbnpi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzvfgwc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvqmqlbdi.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/grlzuxstk.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gkbpkbatg.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gtffejycw.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gahoekkdh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gxcmrjmrr.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gltmhvpcm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gatagfnoa.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gqjltpsbk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/glxbbyvfx.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gfsemtxii.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gobsvcjou.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/galheegor.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghhgukpav.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gipmdwuyl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gbfncrokx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gkvhjmsjb.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/givtobixm.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/glwxdkixm.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gsjcmuhrd.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gtezcqfuy.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsfewqthb.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/ghxjlaxrp.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gvghzggvt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gxvtycoks.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvxvaboef.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gnnpsgiyv.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gzrybymwh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdbtfqspz.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gsntiuzdy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/grxtebjaw.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gsstsodig.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gyntrccpu.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gwspgivcp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/getniafwg.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gpowsfesf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gphizwakj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gepfzdzoa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/glxbpbkca.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvwcfanzl.sHtML


<!-- 参考信息 -->