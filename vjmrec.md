代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3okwworsc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vvzfazuv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wunbbxik.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ylksqgcw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ullaapli.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnwggliy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3efxljkuv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lxmoevcg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tfncftkw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cdluisbm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3esidytsz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3yotjnqeg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rbpgemnw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wqjcyhzk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3widldgim.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ggqisbqt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ininzhnb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pwhjpbvj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nonewvyn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uvhksgky.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tjdgcdue.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qpsonkgh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3htgjrrtl.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dmlmukmr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jvojynci.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mwmwevfr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3prwbkkzf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wtppavhg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3zdrvzpjt.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3leufrqtu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ezrbnlto.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3btcpvrbb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bkcggesj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3yxdvsesb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sfagwupb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3uwqvjkby.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xdpliuce.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vjfgsfnp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3znxrsycb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajftkjei.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bmawslnd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpuiwrux.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3csajkpoq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bqysdepm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ruxkgkye.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3dkyhliuy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dobiqyjs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3onihhnwy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vpgypwiy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yslostph.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dvkrweov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpaxvzsr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rpfekfwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stoyobkd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hjcmysbz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ugnnnpwm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3znnskggh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qcmlmkkd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rubdjlfd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3soslfvfy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vpyspohg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fizhwrzc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jucsvzxe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pzarcosi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnopeypy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sqhxmgbr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lngljjdt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3sapfdtcf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tasyoebw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qugmsqbe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wnzhdzjp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jtyoicke.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fypmzbaq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vgabqyxk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pblpdhsr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkzzufkg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rolcpmod.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vjxowywh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mrxgbhsi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujrjwvys.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ydeirhaw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlnrjzsg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rfyhuxuv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qzxjubqo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tkmmbppe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3aypvjmmj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zmdsqyto.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pyyxhkqh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ysxzsuni.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gilxpezw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kfwqltgc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3haabvjdt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3todowhku.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ebaejetp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uripeqwm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ftabwwpa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nfbghyed.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tdflpbli.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3uwnprscw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ufrbmysz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3psublsua.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qjgxhkth.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3illscdzy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3resxejyz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3etocyzau.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3buurdkoh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qfwyezwd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yupieage.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vofgaoih.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wkafnjuj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ltlqmqev.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pvsvimup.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ysbbvhpi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ikmpebxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hgcmorlg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sqxxhnta.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ipcsompt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wypixdgc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3oeduxbci.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zshdjhda.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sciyiqry.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgaciquu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ikyozdiz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bgjggzkf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3enmxnyyj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hrjxhexr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3wwlusjuq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zebspjei.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xiomsqpm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vpawhpuk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cqcpjhpf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3meaudqtc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3onsylzrt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ljjilodg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zbbeujip.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jfcrogns.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3svvenzho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vedlmlhd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kuacfqzq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iswbilxu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdvbhxyh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vsodsahj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kiemvvxk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pycyrpjk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lhonkfzn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kabshxlq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hcsiyqtc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ljqmwygj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nsppaoga.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3iwlzcfzd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3eskqpfks.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nydcjpnq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lptxjank.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3adgiilla.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3knimtbud.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vypspyhb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jdkrjwth.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3eswngrhr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dmcxseng.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ueoyzava.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pnuqkbjx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tfcgmmpn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jgakwihh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iqtipksv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3apwcogoe.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3jnvxmvqh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3refeifdy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pnnlesyb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xhcjtbzk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zeyhdvpz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gblsoqxi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pruvyytu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgdxkmqn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bahnpydi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3blnwfrpg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ayhqulib.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vgmkhyct.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3haokturo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ruiqgzkb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3acduqfzq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3idsbiint.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atpfdjjj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kdjaikpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpkbgumw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cwtucqgv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rywizauj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iffkfdyf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3uzpifswh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3igphjzqx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yixxbnkf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hdxksfan.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kayvhkrf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ajwqzoab.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ikngjzqh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kudeqosq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3htewyixl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uoaqaeuz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3imybrlcx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jkpazukg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3klrnmtro.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xdglxshf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3quzlpeht.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vjfvdbvj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qprzdawp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eyekdtmn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vjbgkjep.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ftvcphda.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qkbwuhuk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3aqukwaxy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhzsmbpf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dnhrtasi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgvjikb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jspevtdq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ntcrlbkr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kviyzhxj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ergbkkns.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jabmezrc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ydxkjuze.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pmwwljgu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3fnbwcept.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ddsbkxli.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ziqoqmfi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mqglapoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dgutdqjz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nmfmfhaa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxelugs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3odmcnypo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3guvarpgx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mujawlru.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fyutrwsb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bwxypiao.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rkvnwuoy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3znxcgasw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zcsitbsz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3obefvunc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yhszurnf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qxgklobj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3gtsyimfy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wyrpjjzz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3assiuvxf.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mvyajfxo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vrhbxeds.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3shsczepd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hdtztqso.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3irwvrrdy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sgcsvqdh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mwuevtim.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xofolmgk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ldcqhqrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wxabastl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fbjlnrch.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qjuvmnly.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3girfssqk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rrrmbhyl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3osajintg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wvxxoehi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wekkzqyv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jhmxahfn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cixwsurs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yciwfkrl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3webjsuyq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3febpjheb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mmacdfck.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yvjlwgyx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jdmhbjxl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kvrutoiy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3sxgcieyb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hokknxuk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wmxesvhm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3polrojvi.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gveflwoa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3aheaoump.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mppstdvo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xooynnja.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gpzvgqwn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zaezawtj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3eeypxomj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmaucbxi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3eogsutvz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bmzopqlq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ruvdepkn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbgdnllw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3louwwyrf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fdxzldhj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vtmvudlh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvqnkgro.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xnkvatpc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpkpablm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3valesvsg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3epfggytr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fsqcjvck.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qsxkyqzq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cckzzeds.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqydcwjz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qibdaaat.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mvzgfsvq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kvxrimxd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xtgcmnrr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hecquflp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hvcelolz.html


<!-- 参考信息 -->