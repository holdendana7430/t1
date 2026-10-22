代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2lhbsrkdy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qetsxnus.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2jkaqxukg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2omugrsls.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nzoevydi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rqoukgxx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xgzzuqmh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xrudpvas.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wgxjpqec.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jzpcsmmv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vzcrfukq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2pgnnjfgi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mnmagqib.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qknzpbgg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vrukquuu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wbtwbegw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wleyimau.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pcarqbxt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cimudvyc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2elgqjbyk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xevsfvxk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgqfiulv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2smwsyyzq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hhgwulkj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xpabgiun.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pjguzuxd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tnxvsbvd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2sykgpafw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sdkzgrce.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dscysinn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vkkjrwrv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ddfhwikf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lyjuumhj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mxiefclk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pdeomugm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pnixwvhl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ceygjpdz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oadzcaxq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pqalxvhg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2supwzexx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fwflhiav.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dcmcelfd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bqkxtvrk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2wcayrpvs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dmimrigv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zngrtlfn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jkypgcey.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xyyyvpha.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2hjoivhpq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2knbwwmgr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kxpuaguq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wabrgeay.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2igubtbor.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yxiokfhz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xnprnvgr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ouvhevrq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jifseybf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wwikfjtn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ihvkttgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agrgulnq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vqkzbreh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bffuzkwx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xmcifpmj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lbuqeiyi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dimdjofb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zaeoenmz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kwmafpqg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mlrquzua.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2psziauwf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zbtkyrak.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dnoyqiox.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lfejgkuz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gnvhhftd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oljfrtlr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2iqfhzdlp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2cpjagowe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tqffnkvg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qsvfbsgx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uzcakzhn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2smzicutr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jmwyiroq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pgbsokxb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2iaycpvxm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2slgkyqgb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2eceauxxy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwowjvf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mlkadckz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2puhxxdpo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sppuhejw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ytvjjckt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2voebsyti.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wvjasiyw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ymiiliwr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zzovdvsc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2huisprlz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2simovhum.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dmavawks.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pzixkicz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xwbirbue.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zicayqtt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2irfrazem.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cgexhefs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ynfrjyno.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ukozgppx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fqjwcshy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kfuuwzne.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ywbfqbdm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ikehaizw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qxscknog.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dlapfuxi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fgmfwvga.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vgpzcbih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2opdpueah.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gvlouxwv.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fbafxcik.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2myzsmjfp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xnsjxbgb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yhxpfkjb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pnsqxeqe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2upkwidwv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mygenwot.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2abisxidw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dlcmvyjr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ojwgxbwo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hfuceskg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2skzinbeb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tvigchot.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mmsjihjl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vbgrpryg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jvivttqc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgzbonoi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2qymaledk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wmvxghja.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ghpjgsmw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2plpfoigy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vfhkvvsv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vnsxumtm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2akaxghxj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fnmsjnub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpnvguoi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tspzdvqr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hydgxqqe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kswhjhvd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqmcnz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fpugkkxc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ouexidmg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bkmmaukg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mowehlck.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dxmnfzqz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gyxegvjq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yclhkyob.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2eolrraqa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uebpzzyq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nhhyosif.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2doelcrqn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qwingibh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mlkotupk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zfwavmfo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2knktxcnl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imwmhmid.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mrerpsgm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2muyehooq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jjmrkkql.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pbgbswnu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2svrwnugq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bznzgppw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xtgnlrlm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gqhraire.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cuyqmkqu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ithoyjod.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2apkkbxqd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2oavcmybm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lodansgd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ykloamji.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2comoufto.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wdlwqdkm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dyxhxsiw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2chokukoc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mykhhuvg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uvnogagy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pxsrlsly.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2gsvjrods.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ldrxrvkx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jpwnoyro.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ibvcwmzv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2khxawksn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2eiriwxkm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2poeeuhaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yuoyonlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jntwoxxb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lpfvtkdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqcfnpcy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rzykmpmi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zqwuwahk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hoeliuyw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zoeknwbu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qnfodohq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eyfgoydr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ksdcuyxt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2odpstwui.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2klyxnsei.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ycabbdaq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dlbuitrq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lewwesxl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qhavldpz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2skbuhqtx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lhbobzzm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2usxdubjq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oioxpwbi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yxmlswhl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hpgdzcdn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mkjldimk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2okkmmgmt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2enapydrv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fetozsqu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aruxlpyt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uztfnkhn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdqzvws.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tifvzkfi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rhyjrhkc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nfhsmdwr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jxkkkjoy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hlprelar.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fftufmuh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nzumkamq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2asnhqqph.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xlprfwts.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zzougbns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yojobanw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gjchhgmq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2unrprpqc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2whsavbjn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yfljrtzp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vawblyvy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2giqlvnls.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2crnfocmw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2pfkantmx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qohfbobg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2iofsjlkf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rserdbpq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wejozddq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ihycuovq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pgpreefr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2njgdcawi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bofcfoha.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdklssaq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xqmwcqhm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2apjabwuy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2eebhcqft.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2iptbxaiw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ptihplts.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2wddbrcmi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jqfhuimh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lradhpxp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bkrvepbj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmbjewzp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ibzytkwa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pakqecdh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ehfvgfmu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kqxeoouj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2furugbnb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zodezxxx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqnzsejm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2hldfwlsb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pagjosnn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fvltxjvd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gplgrzsw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2elzhyygw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rpqvmmhb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2jjwmybcp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wncflgxu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2exurndiq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxyghbzo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uaqcxnbl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmtypiff.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rnabgqjp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nnrsnkih.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2agdzlkin.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fkvddkat.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fwmrnmua.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oyxgvckv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2aopyuytd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pngasnav.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ubhkvxgo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2etxckgid.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2scaqwosh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bvoshrzr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2evsdmvtd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvlmoohg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2scerqcrt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixxfhnwt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2mapjongh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwqgjqta.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gxsikpik.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vhlsvdkh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnylcqle.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfmpkvuv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ewknamuh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vjxqbdps.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iehyoijs.html


<!-- 参考信息 -->