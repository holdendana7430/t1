代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2skveadad.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pxlcsfyv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zewgjqsq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ecyjfhbd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yuibzonq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2krquzlng.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jmsftvev.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2alyqhqlw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2snbfetuc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bxjdxryp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dxhaxpwt.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wahortvw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sbiqdyxq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rbuvvkgw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vfjgywbn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lcerjyqr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yzraouiu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bfdqbflf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zqzmrrdi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tyqbcmsr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2iqgudyol.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qxegkflc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qrrnbndt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2osmqgahy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tkfwrhwa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgrsphsg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fzcbuwpc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yfnfgjuf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ugrpgoux.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2opfhmclz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thnucaes.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2syxzhyfs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fzobemwo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2achnftoq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sfufwauk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tqrvfnkr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gncezajn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kefdicgb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vszeoluy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dkbsvptn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2sghcvkid.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ogglixjw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2rprhinnz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ipjailfm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pdceoler.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2upqiuurr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cxjyrmka.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iwiyhfhc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uekrsdjl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2idwrecki.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jesqmyqj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2uicrqonb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfyccwkm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ceyvbidv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qnjycbmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jonkraov.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xvwnepxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqxnwkbx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fuvlafkj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gkabwbua.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2snuqgzxb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bbsmosnd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2frvzrpew.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vwbnigya.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yncrnvid.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dkgtkvkm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kfdzzgnb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2boenjzrk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vodreglp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bfiwfsqy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2imhacjjk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2glmmtmna.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fvkjnaln.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2crdqmdud.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xwaetyxr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2iutzlzeg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jrcqmmch.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jspvuofn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qlvuymiv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2slykrmvv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2entamsbe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2frdozwkp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tqbbwlmn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qotlmhum.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aaloepdu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ebjgloft.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wjwgyogs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2moupumfa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mdmvghtt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2phvxdsio.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vbuezjoq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2eztpzwkm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fpyhlxlb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rzcvmggt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rhievqij.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jfmrydrw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wcwsezmo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wjxtymrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zwmmwtyz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bewwxbua.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aatdntzi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dregzztd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2njhdeive.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2melthylu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cbnuizbz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2epmuokcc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ijmdhihe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qkobjnpn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2sxbgosrh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2txucqfsj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wzenirrt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gzbsvfzx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bbnyfldf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xdmxedsx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mfybhjuy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxhgcghz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2avdwxmri.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qxcksbja.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lzbjvwfl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gpfhuivn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xrtmmtsv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tpkbdpjb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2psxlfpch.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxifvvhw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fhymamvw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2danhpfic.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvtszbkg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lcwdjhps.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rbpussfa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mdrkmnpb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ytgcpyzl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbcghloi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2luqaxmpl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbdoklbm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uqzlndov.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lgzltild.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sgbpkjop.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vpuvwnmk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zquipeuz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jcmejkzo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kzopgncz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ocuruwtr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dzsmtnph.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gtvcsppn.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fgieyedc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2hxffqvxx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mznocixw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wlvpbctn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hawsjfox.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jgzzhulm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2egecisab.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jmnbylkj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2aznswwzf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2eghmbxpo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ekxnktfm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cimtkpva.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qbgnmvcy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2etgcoiel.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2anupzsub.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dselclxy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ijbgyzvk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mlkhuijk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tknvxrdn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lbuncicj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yktlhdkm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2babnaqqg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2useltfcn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fxalhenu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2choxjwra.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iujzoiuj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cwjzsfsh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vqcmsarw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2znemwqrs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lifnbpxk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nssqdiub.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aoqwkyov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvgngpgr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kbjuggfo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lxdswrwh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nkynpohu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wzttubmm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rkjgkqpk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2brgvkdlx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mppsycxz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rqbzatpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijbddfwd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ulfyuzyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vknlcbom.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2onihmttf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qhhevjcp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bwwpnvmv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ildpwsdb.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gxyduxbt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rjmpfjfo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uvhagesc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tpwhjyob.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ftpsomrq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2uqdflzqm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mqmhiaqa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdgpkthx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cinbezrc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhuxuyd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dzboqwhm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qwmrjfey.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vywqszbe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2eglaoyfg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2glqqlscg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zgtpexsj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2omnmuwev.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rfgupwgq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zfcslhqw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bxpkrpls.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xukpukje.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zigljjqc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kxfyxuru.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zaluacwv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2tvxibbxk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzzefnv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yzebtrsy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gjafantb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2pqkokegi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jltdswev.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wqbmxxcq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cfvkwpcb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tivtbvma.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pvokbjpl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cjszgppn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ujrdqyjz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ntaohrqb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2iffwpchi.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2uotugtyw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vjkpvgyo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sbioeqiz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yerersik.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2tekxpcll.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tgqmiiiq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rmmqvqoq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wsjubcel.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ccereqjv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kluxifjb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uxjtmski.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpwaomhy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2azpmrasv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2fkwhyilc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fcdvpdcv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bbbslcci.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ztatoyer.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mcqqzwih.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpzfpcyo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eobsiajq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bsixcdyx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2jwbluqfd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dtgcvfbk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2qqaqzixx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xokhusjl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gkqlgckl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ycnumujz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qoujnafw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cbelbotf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jwsmajtw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fgdljycs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2krrdpvuz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gfrwslnl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gmzexylh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rdortiua.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2onpeaeum.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pkkjjhsi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fobglpoa.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wqwdnbse.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bdyecsoj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2jewbjzhv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gclyjsia.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fdbhujei.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2snvnbgec.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pnrsrcfw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lueuqtyr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2djwyagma.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tdviibwj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rdnhzmly.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lfigepll.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2pzgytzdo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzdcgfee.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cngwiqth.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2doaglqah.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2emnbtcjf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qqulurpk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hzlgpowr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zjdmnpys.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2imtkoirc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hmaiqhzm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yssxmhmf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2jjbdvqox.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qjzaobfv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mgzyplgb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2swqqaidc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uinzmiat.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aahnxeti.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vbneczsn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2amnpqnqs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sokidkwq.html


<!-- 参考信息 -->