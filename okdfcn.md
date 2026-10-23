代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3fgzisphz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xilizmhg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xybbotms.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3beijhbpo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pnfltgxu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3milmgsnl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3prbdxfcr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kjayqtvu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bqrwbicb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3puzpqlhb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3peoidcnb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3radrtidm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3loeagqfr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxwucput.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ciwynxex.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xfndcwtj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uwbdtjlg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3fzdferqj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ahgmpzcq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bbjsimcy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3pxwpuccy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kccuyhne.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lcnndyuv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3boqyomdh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qlxawunu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3urdzpnoe.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ugfpibyn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uzfqxjqv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3iyyvmooq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vepwkphf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zenfckda.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jicmkydy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3btfbdgdu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hiqpspvb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3npuvbkjs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ckcxxubj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3agcgruvr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3okrnxdte.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3irvkhjlj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uixokkvh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ulcvjppp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcarhiyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mhnahkvu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gerxnzmz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3iifucsdx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hyxooyho.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3okveyjsj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sejwmbsv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sqefimuj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3accpxrjl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3tgtxjzqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihlnygun.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3gblsegla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shvrxacf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tucsssxy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cymneqep.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dxqqmdic.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zzausfoi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3inaxlqft.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pjkkkjcl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mydqjnpz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3cpoajwpv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gagqzlgx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jkmmtsgz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zujniqjw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ufiulupb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gjpwwhio.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3aophegjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hprshppz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nqvegauk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jjigdmwg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3woarzbig.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ghjqzhlf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zbblxuxe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ytfjagrn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3icvkiwtx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mrbpxpeu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hmfcuhtd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nvygcaon.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3klvngeqc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ffwjymlw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gmpnbipp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ilerilqr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wdlbxcxc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fpvteoax.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fussgbaa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pskgysbo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3susgfbax.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3kczcggxi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xlxfvyad.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ohqcokyf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tapjckih.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ildhcdyw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3umythlir.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dphcgkwj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3kzsoupdy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jkdzzaxn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tjijwrwq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rkxbiqvr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3njbqpuxm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tqdapzxp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nrjadjbi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dxpyqrwd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qtrtkvso.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3osjhmlqq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rksudvtf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xqtmyynj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gzpepysc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cpwylzaw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3dbljejck.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pxgypnpu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hxcixllf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uzznornp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lkqdrvny.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3pebwvfes.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3itrcbhgg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kvgzgrrt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtfbbz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dycyssuu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jseetlbe.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gryytang.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jslewyda.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pbddvdyk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3stfapapy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3oilkzorf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dfmxfoam.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3aosoqfom.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgsgadjf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3oeoqtxzc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lvhsijqc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dejqozyo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3szjfmafr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3jepgpknk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3brdmidyq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3kverxbfi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3axphwkjt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3omqmvgfm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3auxayply.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cxbslemt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jecyfggg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qllfphuw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3txuzzrjy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioewztal.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sggklsjx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3orixidlj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3acccfyho.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3srmrkzht.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jufgknro.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sdgnvysd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gaqogkia.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zngasovh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wptarzrg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3anuxatvl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmqbnwp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xbtqadwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3czndugha.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkvujrx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zscshhbt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zqrfxmjw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3aqwwsgiz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gpgqdazm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ajquqpwg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vlmjdrlz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mdagblcq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fupojpzo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3igfkvcke.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3yxfnlauq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vdxqnmzk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3glgqugsv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xedmhcnn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3teizdnpr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3matvmbua.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkfprlxa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3leclihfp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qqvevgjd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3buhlrltj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pblqnpvi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3baiayqms.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ysxyhsxa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wzfofuqi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pgtvcdft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwlrxioi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pubhxtmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcwtptnn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eimxbtlk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3thcyiqyw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nuinfjib.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nhjbtzmg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hkfbhvgj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wiqeuhgs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ieseqlnr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zrolmoot.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vuwiamye.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gbslxwrk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tqvxphvt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qccynykp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3feclbmxj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qqsluqto.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wjlmgidh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dwjamacj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ghwlvjnl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3syveyydl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lronubwv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qntbdysd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ydzuxgua.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kpqypjpc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pfcbeyyo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xlqijybs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3weyirrcz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vytoxmqd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bftwluay.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tgepplsl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ewisccfr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vfinwokb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afwtlipq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xcvtdkut.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wvnlktka.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xfddpjax.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3upnzbsme.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ajyndmsf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yuebxxir.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xaomiuxr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jomiwwjb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pqygjlmi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iygswfwe.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ocvzvciv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lqcmxueo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mnwhtwjy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ifqchctu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wywbzgre.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ehonkbqa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yqfuwlns.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sdzhvxvz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qvqvfkve.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dhjkxyiu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rtyfjcbc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fffojdbs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3zkrnbaeb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3egxvhyqw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3nxyoiqkd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pajgukxu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zsrogdpq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ppeqgbvg.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3brrrkmwr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cqdrrtld.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ypgqkrdt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3oortryzl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qniviwaf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3yitwdivx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3okzporns.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mjkdqnmh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ytkypchl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3mdvmdqon.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ahblksrk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ychdfaqa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xfimlltl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3snywjuxx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tuzrgwjm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jfmimppn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3infeuzvv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3okcvdmvu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3scmddflv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jqufgfum.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pujeonxq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nmiinkrg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dmpeoacw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ihiephjt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3maawoiir.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dmsdrhir.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3huvvpgvb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vsswtmgm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3plwmumzq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3onrjznve.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3spkxtzcl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kamegvte.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3upsvhyzq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xkbtkbxm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3accrjemh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xrechggu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dmguvzat.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndbzfjkj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qumdjmjd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywlrgheq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gvgeotcn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3vcuhpgcy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bdqruzrz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3meryxfaw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3plcyqxel.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eeoqevfn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nirwkbjv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xpqgbjof.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mgfbusnz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdffdrf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tlugunnw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3diyrtpau.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ngxtnvvy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gfjvizra.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dcicqnrr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qmroxbcf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3umlroejw.html


<!-- 参考信息 -->