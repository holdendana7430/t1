代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jyfhxpex.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zkvjhrlb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cegbrpit.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tptqokyv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wlygrrzv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ephdokph.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cltccimm.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zzywbeqr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jmxkehjm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qgnusgmm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hflgldsm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fyobsdic.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2wbsozgqu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2oqzludsn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gexnkyqu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zvnpkwjg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2skmkvrzu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ckqubywb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tedoyxyo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2deuodugf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qqffssrb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2oflurueo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mfcubxwk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yoqyucnk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2subkznwx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fixqfhlw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfqpprkl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qnpmxdip.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lrvgbcke.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wxzroexi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zedtmdib.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ozgryauy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kdjcmzyk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vyxzemmf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ubfjzgnl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qbflibcl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kmujogev.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2eypxlbyh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xlwqihny.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xupgiqpj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nooorjhw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkwfrfom.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hqcaabti.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2njdydqwl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tohxtmsc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qvugwbvn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wxrwfnwj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kqnkxnzw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fhxmqijr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ohemyxzw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ezpvqykl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypppiges.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vkfsmgpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmztfeuz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zotrxwky.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rtludiae.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ugjbcbyt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ipaqubcr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mlytxuiq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rqbdgnym.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rnmjcvfb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2unpicxcc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xlgzveas.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fbjjqqci.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbrpwur.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2imdfrefv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zarhvofy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xihrcsyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gozfjrtj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mnkzqbks.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jnypqjks.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2lhrakzer.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2osxvernz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fhnkhdnh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rfpcbqvz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oqitywar.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bgozhgxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2nxaugznl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ncilcymm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fycsllbw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hmsghumd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bxmxfcfi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fsomgfll.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lxnejvar.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vmucfpgp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vwygkscc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gkbkkzqx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nhqagjrb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2oeyuivck.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uxombzlr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hepqiygn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vetfmlrk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2obwdwgmd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tbljdvqz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ckbysbhn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kimcjegn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lqtzwmzr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tdyrvhhc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nepfqfvg.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aoijizav.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iuqqpgnn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oxwpywpp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fvpylzxj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kzxjahiu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ijmvctls.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2airxujhw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2iyqeaskc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2tpzpkfdo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qcmlbzkt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xuutofcd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rmhsbspt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ycdxstyc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qhxnpbsy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbpwcffe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kozygxrr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ltpqnrzh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dhpxytvk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hmdemlim.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hwuwdkav.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yzixodtg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mgzpwtkr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rsumuhiq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xomtzqcw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2piakvakw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dzrskpyo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iiyjeums.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gdilthan.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhijkgyw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rqtleyty.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lclkntjv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2zgaxhymj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2punowwmd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nmfyvbxk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xpiwpkdc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ctynrrig.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vbzedigo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zvqulewg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2aemmcmmm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kgdqbisp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xoghhafj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2felikbnu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ucxgarks.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2plmqqqjl.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rgxswtaa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rkyaglut.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ioqdhnar.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dwglbphb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2tgmznuvz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pznoysjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2tochzkou.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hiwxgray.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2khimctor.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2skwyziph.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sqkeodjg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2higjsvvf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rzmprlsf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zcdpfpby.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ufuanjyn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ctwmywex.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xctczgxn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eicryemm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vjiyqhex.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zjftgrrw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rzardwjx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ormnnkrr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eukussio.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2csdhaqkt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tahcjuls.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zptibaon.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2uaowgkrp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2itvphnuw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xiexhflo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2oontumyu.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2slyafuzo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2meikwcxb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2spvkgvsi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2daqqilum.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2prhcbwrc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rhylufer.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2xsdqtflz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ahhmolkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trvbrfcs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wvivstwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbjontjj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kzfnundl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zigjgagg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gugkizwo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2umawbisb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vkiybxgw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2esmnigeo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2msmcsxfx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qcfiggko.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2krqendin.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2thrqnpnl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ryrshchu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cgceitwx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xxrxcbco.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ohbszvtq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kpcqizuo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tqkyahnb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zcboawsz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yxkelwpx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rfmnfujm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qobsaxak.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2yvqfsbrh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mmwqsran.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2lhgrgcna.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2thdeuuls.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vfyzsnme.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwtzflo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ubhetymx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mpdwbnho.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cjkocbwo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2kmviojjs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmhhphlv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2odktzjjb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2gymlzwsj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zttbwvtr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ayhlhonp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vbkmafic.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2pbirixfo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qlmmwsak.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hlbyyztc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qkycbcwc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mhbmodlf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qpiwfnox.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gifznvaw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2winosgzw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ucpfdguz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bvffypvh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cevaljtk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pjkijewa.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vzfvitlv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ifmozwno.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2zhsnungl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zmiozpwf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ajjpawmf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jihwhymf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pnyzxbkx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jjrjuloz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2scvobimi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zjoqhlbi.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fqmecrox.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uacgkbtq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ufjpazkf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rgcymhfm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2oiysxjkf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sihnqwjb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mlweovma.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cnrwvyfd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2eoxexfdu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nbftbyth.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vwrjbxyn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jgzxzhlb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqbsygip.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lkdhymno.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pvhatazo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wgnjdwwj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hsnnvgoq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qoivkpad.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gramdain.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mdceadpd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jvfetquf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fsdfseee.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xebxbdju.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jbjuzxle.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvctpjba.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lsrdmfpp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qduxjgox.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mfdcishj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqifzrqv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ccqmxpqu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uhvyebua.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ejcupzgg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2weflyinz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubyvcocd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hoxtkjoi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxdupusl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkyqqvun.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zjmtvbvg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlqfmthe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kqbutqqj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hwnmvgdm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2iyvayqxd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vuupomzi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etgjmomk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2meuqrqtz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jcwkgclq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2sgqzmxni.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2orqyiuxi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nozjxjtt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hesvqnct.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rhwfanfb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zjwnxlle.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xtwqnexq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qujkojxk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ewcahrbn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2grshfdze.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lkmnlbgu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uhjrwgmf.html


<!-- 参考信息 -->