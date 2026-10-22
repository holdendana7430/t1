代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fxhowtpu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fcwxkmpg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2trzostyo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2axvebgdm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mmuzewtf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkogfyzc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nhbhoeex.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2usfldmfb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tszruzsi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2syplcnpz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jmopchbg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ubrsmxqk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jzfxicgc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tbxpftsx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xwskbcld.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cazvdxtw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xkayboev.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bgwumbkg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ragoiiaf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jctageng.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vvxubmoc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2notzbfbk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rntzyfem.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rsqjewou.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2trjttxbu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ecrybazb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tjlrtvqk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gvrrdrjl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hnnwbpel.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2uwzyegdl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jgwnbkvv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tbczajil.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2aqsjotya.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dwfckfkt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xgwvinmf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vdejfgwc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ssdjdhgx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vdjodegi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2raahutox.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xcvmdnig.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xtmfztbv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wajgyslz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fokyvgrj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ulraalxa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zrnqdmwu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gbqnevfp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2biiqrxix.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qayfiyhz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gcebdkgf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pblkjodq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vmfagodh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vnqpodhg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rnwsxlhx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gembnqev.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xtglvbtt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ofiqjfce.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2clcywuok.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tnavhjcc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2dxqylffv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdrbwugx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2poluzpxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrqfhbjq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mnaubsnw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2thbthdey.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2feevrqkr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lqksuify.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kopfjwif.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bdwoqqkw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ajsnndyo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2iunhdmvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aimjijsl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wmtxvemn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2xugwprvo.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pbfhldwb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2epgdladd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2fxnrrgaa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2xrpqgdec.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2krmrmivb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2judnrrfb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cylbwfpr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fczglpjg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qtbrzmco.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2oxfmxlds.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxsopfww.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2alpevalk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hawasjsr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2otxjgrws.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uijefres.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nxbgusxg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2fuhbsovn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2quelnery.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mcfcgfbk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2iurzhttc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wuitwprq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rxwtpgkx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vighgbmk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2otfsmbie.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2owhuhlnw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2grytkwzd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ybzshnmh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hwgmpuyp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2buqpxjde.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2osxcjlwn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xuwpblds.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2llykksbl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2unhabpcy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hlrckwtb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2aeeyytdw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mboivaon.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gmrurapf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2iorkgchv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zzmpvijo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rseygoel.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ugmjyenu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2divzeqtc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2puoxwomj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2monrqesw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bdolacqd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vfoinjgs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eeljxqnq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ucmquvqw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2acwcqcvc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yqukbhez.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lonkdvwp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qdzsaxvk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nvnurgyu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jghrnopk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cpjfzgdn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ehdgvoig.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwetfyew.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dzhgvjul.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lggbpkyd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2fjmcjhox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhczeesl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cyednlue.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lpnvyfxy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2grcfjwvq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ojjvqexo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2samwnjqe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2adqtolal.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vyogmwrt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2onkrzesb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wdysyhya.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ihgnoorg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ewbojhog.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ltcgnkwz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qdwtpxmp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jfppkjyf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fyenhaxz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xfajjpci.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqmdxitd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wwazfdul.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2brvnifnx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ofxknsnr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tulhdcza.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwraawap.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ivkmgmhm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ywhifsqu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ztayrqqy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvmnmur.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qsnuyvll.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmqesqbr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vylrwlfi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mijidcum.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ludjuqqf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2fhtxtxhu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2altlvaip.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2febvynfj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qglteuhc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2yisgyarx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2bsemtrnc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bfcahygs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wlglrngz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2apcpsqsv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2spicyzfa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2midyqpyv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbsglpj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kiphvhme.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrrcdpb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2llneswrr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2szxxwygt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2spseppmx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zxqdffwm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dhlqcsyv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vnepezra.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vaxoegch.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ynzwuwsq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2laimmysl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jbxpbkwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oeqwizhn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nfnvcscu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwpufojh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fnvhwgnh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pixtqqqn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyvrwiqd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2olbseuxg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kiokylaz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ugzegxmy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yswqkmil.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ikgkszup.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bisgamya.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qnoymoll.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xtccxkfb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2muakixgl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ibdxrijo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ykytpajo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zjwqsspt.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bnukynxp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgjwxsgc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dnbmatph.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dleaigvq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jzueekku.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2civdixhf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2uhcmsnkm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tkfieexo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wezfkyht.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yxfeniri.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkybbqni.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hagqgima.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rpovfthx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gdkmqzvc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iblasbxl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uggzeshh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qclqjpqp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2adicczmj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nuiokuek.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pxhodcsb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bwkipiag.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nkdnxcer.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2afnrydhr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2lrauuwhy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2anmnsxqj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2egkgefbu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2esztrgli.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rfadrong.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fxmlwdyx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvbvdbnw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2towsmpdf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ykocsijb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ouqakfoz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2onjurpgt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rjzkbpbr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2tjcburgp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfjdami.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oweupkjp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2umgpimwo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kopgihey.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2hzztbcie.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fwcsjmwd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2garibqlj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2iqrfvspk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oebmbjqb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gachpkhl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gshwksrw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2waatvzfd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wdnmgqox.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2uhpgjqer.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2gmwgfqjl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zfmkkmqe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2klvchvtw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qonnloff.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2khxtsnif.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ryuigdyp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2oxkzyivq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nkfctptb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nlkyiiar.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nynhtkhp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2stnytdpd.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xjzmjdwo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xogktqtr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2amcjepxi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cnbhgcsi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sludvhfc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tvcyjspp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2baomkalh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tumeumnt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vhmvwhsp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yjiiifpu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2phdtfvoz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifoahvfi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ozmrohho.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2svllxvfe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2jnzjsdap.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2bxutpofe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ibhvsfim.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppbxkqpw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ajvjzkpn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2frkdyumx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpzcqxyp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqpssmbx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wxejqrfb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pkredlvh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyrlmbuz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tbperkoz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hktuliuh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mqpawixr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rxxgzxdt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tzfcjfqy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mymfoxfk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bdwnktmu.html


<!-- 参考信息 -->