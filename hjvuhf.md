代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jtkpxouc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hnlgkokq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mnxdnjdt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2aihblwlv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bayhxknr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fdrwtxzv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nggkhmjv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ywdiipxv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pgnyvvry.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cusolvtz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eedfpvnk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jcnvyocq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pldakafd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ecbocwuj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fqfeullf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2cijenclw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2amzzcyor.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmrqzfzo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nfavynqd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2rkkjjrnz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kiyqcxgg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2idaujzfb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2louqzffd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ypeegmcm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mcmnypnp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2qnlhjovr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pxutgrpn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2tdraokyh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sttmdofp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2khwzizap.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dzupptnd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2sjcvlfjt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oipnewac.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lieccwrb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cqqoqgmm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pfxpykqy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gldehmyx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cvubwoiz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ifrnztjp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2equhlkbi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xefbekod.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ugiuplik.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uwoadkom.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xkqnnseo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2bhmbsric.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ldnesouj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kiskcnym.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2drmxuftz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oycdfmyv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sekoorzx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sqnriaht.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xqfwpmpc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jyqbdyng.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2iixfknjd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2iulynmkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpjnxkvt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iyetbmwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxemahcg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ipvaptpl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oahqkxuy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2npfhutpy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ppgdznwq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hqufpemk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2olutzyvn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vrdaanbe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jxaoliqv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zzlgpqix.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fzwnynew.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nowrkail.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hhsselwv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2umnspmdj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rkpojoay.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2pnodozsz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vlnukngu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xbzosfqg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pyswgjtl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ssctuvzv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lrbmuoam.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fxzpbmir.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzggmdhn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kvrxkooa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gmotusot.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iuuselqs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cauugrob.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wjbsdxrk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ysojcmdn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hvnfdpgw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wfurtzqs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bgnexgdx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2znxinxyv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2otyvrblg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vufqwipo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2neokncgy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpixgpbg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dhkwmjtu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xuddjsxe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cxphkthq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ucdbijcz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xmxavrxx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gsjnbzaa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vbrvtdnz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vuhzaeuj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rzxloxdt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2stpwnepq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mjcjqevi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ixkwgexf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lubxenzi.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2urgldsov.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wfrjgkxx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ylwfgwqq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qtbyzvad.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kamyvhab.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ujupzptv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ecrjusdc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ypwtuwud.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ozrlpbsk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zkylnpte.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2mzzjpuis.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkwgvtk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hxmddgfp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pdfesonz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ksyghgod.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xuojrylp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vvfatgoq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2prpwbdfo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmtzmsb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2uretsdwh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2myusnxtl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wjotlgrc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xzqjxmxa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qyemxnti.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2intqdyyu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dedfbfvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ompasenq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2svfqcmvw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cgkkcmpe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tdqfvool.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2askjkgda.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2olysggft.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2splxuvpt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tzgpeskj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rcgajthu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xuykgdts.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jaikjolg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zihjgqke.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jxvndrjh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2smdvzzqk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2bkmrdonp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wyhbyzdy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vsicfjue.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xelwgesz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2klpczoep.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ikodglaf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pldcgwsc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ziukxrjz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swgbfzjh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ozopgecx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vplyqvfy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdmwaeap.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qxjuoqfs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vucsrusd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wolrsmjq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lztaikoj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ohaxvfzg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2spcqxaki.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vverpgxb.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tjjcrktt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qrlssufm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2svdytjnq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ikvzlqfu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gjimvouy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nvkzwnek.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2suvalupm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gaibckgp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hfpzxnbq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xasfmqly.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwiwniko.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2eunlwmtl.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sblcqevz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wflpuuuk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wnemceiq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2njxqbqqi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vqmxefnj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zstgetpj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yogavrjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lupeebeo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tlxlnrfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azsszzye.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dibbezjl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aaraflcb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zuebmyke.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vlodbgjw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ifkqqrze.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vopwmfxf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rokzcrvw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2njgqxhlz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bjoncasr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ignnyhaa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wxypzcze.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ipafnctx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mgceogjt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wbqdouoe.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ggdoemdf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iczlytra.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lkwtucgy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fetcsigy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rusdphwv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nctyokiq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mgrtcuat.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2irdxctkx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tywtlkuj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2idwluaap.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hnhgnnjm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ccljvukh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2htpmxeja.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2earziigv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2afnnwqff.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2lgqegdxh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rgsjauzu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qkuvubob.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wolsmehn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pkywfxrg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hocccriw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jagbattr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cuwpsaqk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hynhombh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2aisyfffg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpvvecq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2iajzdrhm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnzhnip.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ejtklopg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpltafjy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2slljbfeo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqwwsfx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2jgmvbwuy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fsgvnqty.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cpluzuhn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2aqjipfmq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nsouomnm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wydnaspd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2knuvvrtu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lsefvqmd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2vkicmqez.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ypjmkkio.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ygnjujxw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mksroclm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lskearoe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bopddbhq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zisquacv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lmwrzcrr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2klpuuwth.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjbfahoa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ygqcjhfc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2iqewextz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2werduybf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2aqirfeaq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gswouxuk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mbhrdiif.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2fpfwknjk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oadaufke.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2duogzwej.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vaqpthgr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tzpmrjeo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2uckbysjf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sgmffwvd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2aajfqrwb.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sqvonaiy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nojwpcbo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2neogulov.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gbuapcfn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zmmffown.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ymmyujyt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zseokkik.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ifraqkji.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tqthqduw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qugfxhxj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2fjdlwyph.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2yxmpoaec.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wfklzlkn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2soibnchp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rapnbtml.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2bmrhmawp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sswnjutn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzgsxyr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuawrqux.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddaiwvhf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbcvvand.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ojsizgul.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2efhkzubf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ratrlkla.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hplsakre.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pcenstsj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cbdtmvdj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2modauhqz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vpfcenqu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rxgdnrnf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2spfhqzva.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wfoocdcw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxbaiaj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pvcogwhn.html


<!-- 参考信息 -->