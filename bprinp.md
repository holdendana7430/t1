代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zlhoqyjq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2mgwzoydp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2fbzqqvhi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2urxsmmyo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rubvuwny.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2plfgrcfv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hfimqucx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xwpdnqvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lrexbdnl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2avdkqnns.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jxgubfib.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2buqhwgqq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tiadssia.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2leqxxaoy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mxcumyho.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2akeaiqcu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hngauoua.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pohlofyr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nahtisti.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rtepmxob.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2einkniea.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rsefbigq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qfvfbzbh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ewtnhkaj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pmhtrmuw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2pmcbucuj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ragvqzqa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tpapjdom.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2thudxvcy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hzpzbvgv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2oteakodl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sjxaaqok.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2uaprsqai.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ngcehjgl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mztmistv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2imjaevvn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xwoewajt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rfookrjl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dujkpquz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bsjenxvs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xnodwtkx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vkfqgqiy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zozofbsu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2uduhbqrz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zeoykadt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2azrfvtrs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zicluqpn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2saismvqt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2zthbtpfd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nywjiuat.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bfqmmele.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpnbvpct.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lxkqsqob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlxvlswi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vmsmekvd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2yipimxvf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdpalkqp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hnwzqyqt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yjmppxlc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tsmeyrff.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pewxlyfw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kduwivlk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2srgjxjgx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jntiajpe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gcxlmkkg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aogymprf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wdhydryf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mzkngtye.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hojdcydp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2skpnjshg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qefxksaw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nvnqiilk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2wcbrbcxk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uedlyffk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vzyhemyb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrsgxsvx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jalwolyb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2soadnmhf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gfsacneb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhkdqktk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kbpvljbl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zeznhiwm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2iqhijptp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qywmtxkc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kybuirml.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xzwlbapb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2iezbhral.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uyhnqbbr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rezcddsl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kziejmij.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jtbyfbsw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2llobrwyt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfmpwui.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yhdlayqd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vvazmhyv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2oiwqciae.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2blboagvj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lutppktl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lzjdnuqz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wmtmoshs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tvjkahgd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rndmmtrf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zlfquqyv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yapoyris.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sfrqjsze.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jkhxvfdq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qksboqbc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gqcgghrc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2umtshevh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wehsnyzz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rcmpwnfa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cjjnqvgk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bbzizeka.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2emyxsduo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wkkzeodl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vllioube.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zkygdwrr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nobjstqn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jzwuqnfj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2flbkzwgd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zbrxxzmn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ujponkri.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qroosjmf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2bxidhfgh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2seinbkgt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ovsedxqn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ruyatlqk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhsgrpdy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fybuyddn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hrkjjqka.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wtmtivlb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2flrjgdds.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xohnezmd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wafrqfbz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lyyqixmh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2irnuxqqz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hasezksm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wspxcgrw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qahphwsx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mmoqsrri.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqwnsthx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hbaalkdg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfruhcwo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bdrfsncl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ldfgayjo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qjkhozsi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ljljqoed.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ljltfjte.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yqobyemp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2jistqixg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vtwifjft.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jotkwxre.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ajqitzeg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgtpacbl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fkcpscxa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ofyfihqc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2esndofvr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hwyhhsrk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gwvgvmex.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tuamrjcr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xhysbsqt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nejmvsln.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dljgxyyo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mkyzzcwh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2uygesydn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kpugjdve.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xrzrlhrv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rowruucs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ruspupak.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2adkdhtad.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zmdecxfq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zqksvzqe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kxwhkror.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ifnvikxd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vzzusvji.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2giaaaffv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmffhwg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zhkuhfdg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xdjvepxd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gwldyhhk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cehbdjpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znvabyab.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qkhxbotq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctrcfsfh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aavtolev.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nfhjtwcb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nidznwos.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nhiqjzgq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qbfbtkma.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dvttwciu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2eqlwdlko.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yvfjvidr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2loupxnau.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hmbgxklk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rnujwful.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dpcrzkfw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xxyejdjy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ibfopaai.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zskcqafb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dsvstysj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qnavfgmt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lrziufwq.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqowotfm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2iixgbalv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ykpsyxxc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2txiaiese.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mzmblnsj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgcfzwr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ixrkhora.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tumtaoqy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ybmnsoac.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2drecural.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xlpnrkpm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfsvwuu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2irryhrvv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ktjcwjee.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2endzqgex.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2brojwjes.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bsrxbmuj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2endsbjlj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mbpkuvsx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qctfygwp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2unzublyx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mmzeiuzp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2dsgjjfuj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fnrphkko.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vwotcvrm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2luohuzvj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cndvppiy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yikdozye.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jptpjgif.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qbztwvvv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mdkbxeiq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2whvpafze.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tnezfvli.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2svljgnxk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2twgzzztq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkvgwykd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xgcrxdlz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2iaepuysc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2celzmgsq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aeprmvkb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ktmtnlzu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2raxrflkw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dzwlryxj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ugciyscn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcbhlvyg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lnyjdkjb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2shosednx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ponxvkwv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hiuyrqpp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2llchjntl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ntsmxcoh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2iftodctc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2bgnvyeyb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tydfmojy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tlvkzsqx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2onugsmcc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qafngqqi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2lyvwybbg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ktnskmpn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cnlmunqh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qxgthgph.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vhljftmm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2stwrypci.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ehvjsnio.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tykmfjqn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jntckkdq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jkzfoiln.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ckgabrpb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qabtomyg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipalnddd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bdxbittx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsgqqivq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wkhxnqnk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fazewfmy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ifwalfgp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fqnnasci.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fvxpcfjf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ldsjdsqp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdwvadqw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2foqhtkvq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dmymqngg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xzpywxkt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hhyaghze.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uzydepah.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2grskldsp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2billsfvj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2utqsritb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bjqoigix.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2eqzlreul.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2irqapcqv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sanvmrir.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fmftfjsk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oporkqpa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vvscbhhu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ssmfonqh.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2veoxhplu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zkcmscrg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bwmopeny.html


<!-- 参考信息 -->