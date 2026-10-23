代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ilzlqfxr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3owzwnwjv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dcccehov.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tmczerao.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3bfjwvkkw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rconbgps.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ibtcyldy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zkqceflj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3emysdpmc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3estaxdty.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lpgcbbtq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3orjjtfvo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ulkhdepe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lstkijgg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fqtdcdzp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ckmodbaj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xlecxvrs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3iaiymbua.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xrquibet.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zqzzmofb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fmuerljx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3mkfibqvt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tixmsmwd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3adgnsnmj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3swdvxaun.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kzeubiuc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kyyldbjw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nczlrcgw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gbzixgqg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3aadsmzvq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zthundiv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gumujugu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cxexgkos.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vhztmvea.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yjkboejx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xtbnkggy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xtzqinjx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zuuwumqr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbvfcslz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cuvzvzoy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bfrpmrdt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nmnoeqjs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3llinhxrt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3frdkotmr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3eqwgsnec.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmprjfcl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jrrrpgif.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mouzchhs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rohcfono.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3uqbikyka.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3iphgbjoy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kdeqsiqp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3shjnwkdx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3udbpvtly.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ywmcwgjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpkwqnnu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tounmemk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfxockdh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kxysqdiz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ngqttkyf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kwnohvwo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3txdzhsrr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mbskkoba.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lznimjrg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ypkgmgmt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3aawcibty.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zbstripy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uhadsycv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgdyucjd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rzsfntmz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pastxfii.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wlrsbcji.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dmliqlte.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tsbpxwhb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jsssjnpq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3pssznaph.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bccwbyqo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wwamgygt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ggkignzg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3itkwxehn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ffwamoxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lhqybjij.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bbpxwdxl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bniiishj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3plehigbj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zqspurdq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ujupthqr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rvpunfzi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kpguopmf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zarjympd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jkatjsri.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bqjzewks.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ayrvdzme.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbsdvlfl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wsrgajyn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztiqknbr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jmyyivxu.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qtjrfdpz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xvnaiodb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pqujffxk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pcmzriqx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3upjycvgt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wnjxklap.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kbthpjmt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jutkhebg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bcyjamjw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3agcplwuf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3opvocnvr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ywxwvayl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jwomrtmu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wrcezfoy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3bgkprubl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zjraqkek.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yjbztwal.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vqxjxlwj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wvztrleq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ocezrrkb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkynxkxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rlhuisjq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xctlaaik.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ersdscsx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xnqywowx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3oxzizsck.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sikyhpfs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3zxvtqieb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cmpsvrft.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jewzysbq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3taflbfpk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zvsklzsn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dwjylhmt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yayuzpdc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrqbhsfl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3onrtojfx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ohmjijda.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vjocmqxd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nxxxkver.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fcblavno.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yqemheru.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zgifxthm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nmkudrvy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3gaqwuoze.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3eomozowx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ogtqcyim.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kznsoljl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3mwxjsvqg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xrzgykyu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3asfbplij.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pfxjkzrs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ajkonkci.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3koihwkpi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3izvweraw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gfrmijry.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ydnxzfqc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wqtdphfa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qictwixe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3hzqvrfdc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rpowlqba.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kmclhtux.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtzlagyd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3faltkwbj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gqrktrur.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjrrybqc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bnzfnnxv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uemzzobm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3msrnefiu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fpffwfal.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sjizmwtd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iymvhdpl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqckmult.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dydnplox.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tfezoook.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rwxbeujd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3sjcmhyaq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dyybqqsd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dwezijvq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rxnvwyfz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wiygyxfc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gncqlvfr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3japjqkaw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xbfbsiop.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3moejmutr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3exoqzjxr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3mcmcnkdk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uytpprbw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hsdyttqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yziizhew.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vjobkdee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkrgsntv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nnfrhhzb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3asepipqx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3szviehth.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3openhzjo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ozybfwyf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gnqylbjf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dwmyduay.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zgiavpuf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ggrchvgl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mwlqdpzs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jneopgia.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzyspkcp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pnxvdsdz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3idzxufmv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3dnvyxlhb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ybtrvjej.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogwypupd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3tgzvsdzo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lywejnqc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3etxuhrzd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3abvgquaz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pxuhvxav.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qsdkhqcb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtjteptv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ffzqtice.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3plfbktjj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3exchbpxf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3igqlndke.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yyhdrxat.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxrbphu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mfrpczjj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xjpcftof.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jmefrwga.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gsoqhpyl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ltxccftq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3zkqtbamw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iudvacqb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3exqlqydh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3oxomkiig.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vscckyok.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ilvawjdb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ceoprqsl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bgqqcepo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3edajnrzi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hwcuiiix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hcozhjrq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3suuttpgt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjysnmq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xqmrigng.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvxqlbc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3marpgusf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3oxfckffz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qcomphsa.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kexdjkhn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iagntasw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qmotirzc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3evuvgulz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uunugxpe.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gsyetccs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jnhaosyl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tmptyjkj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ctfvabhm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zdgkybjs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3iqsshonf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nysqbfvb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kvyjwbef.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3lwaebvqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3jypqntzr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ygalwyme.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rmsueske.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wulwiorx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3plddlbcx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3savohdar.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fzapqmwn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wqomgxxo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qvwhfcyl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oqupugsb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iepiuszp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3etnbhlzd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gzjtvcgf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqugmxkv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pjwufpkh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3iswidlqt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3adeoyshj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zjwrjmyj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bwhriaxm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3futrczvp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nahkbgzm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mnudsaai.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uphozkhl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uqsmpnqb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3emsdfgbq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3awmanevx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eshtwdcy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3scmmiohx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zzvmciqy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lyjbdokl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lhelajuf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kihlsgzq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3prvkmlzu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgamdywf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mmrbywrk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pzrhyoqq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3apskrhii.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3fbzcohvn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3scnkzuhi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uuzpqgpx.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hxohbyjj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fknmapdw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pfeipyps.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3emdhlbtb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qjekcoyn.html


<!-- 参考信息 -->