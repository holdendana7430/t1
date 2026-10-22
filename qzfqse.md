代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2xcjfsdkw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bbyptyaa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wwyedntp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qogshodm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uuulddoj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vfjkcckm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qgjysawo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2exczixki.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2mbuukbuj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2waweedsa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2rsvfxjow.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ilyaeser.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wllrujcz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyysvomn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2iiwsanzz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vgriysey.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qtpzbaal.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gjegisva.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2dfzlulkz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jcegajjm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bytsohvr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vtpfjlgp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dnlexfsf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2llpaoaqs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wggpjjwl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2artmldun.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2brrxagao.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ypabhird.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ksvbihjw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vjnuyhzy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gnunityf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2emdtsgoc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jqrtxamy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zksdrztm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2glxodlsw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jqhgfprm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uqalrkgv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gtnolzne.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mtecgrdd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xvljmmov.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ytlbbsdg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ubyvgmkk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bkemhonz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vzwdwsvy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cmclhawj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dzrnowin.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2guxhfyrb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2cqqgvgxs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vuxamrui.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pbpklzrm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2wsxgyiir.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2befuxctr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2arelqvkb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2btkmtljp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2smjzruud.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dvezfuwe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qlnjahkn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2egctocds.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2abisqbvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffkxiyxc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vydbrryd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzjpqdyu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qraopevb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ixwvzihf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2aiwqindn.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2douimmhq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2mqwlxmjl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dvopjyfb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kqjnwnsh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2aajnuqdo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ymuvldna.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2psncdoas.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ploandzc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vngbcfoz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pxykngzy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vfaywyex.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gnjyvhct.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ffmpdyqt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2utpwsrea.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rvlyucxl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xnrgrcyf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ssnotxas.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fyyfmdmw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yguidozx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2moyxpvpy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pwxvgqcs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jbhcbuat.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fcstudbo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cbipiafa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jzzfsjck.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2blahcysc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vkeqgsyd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rfngfudv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hwniljve.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2gbiskzsf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vfexhpkj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hzutfpuc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wgemmfqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2srwdxgbf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dhlbgmdb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hlqnybyf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mfgtumqk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2luowhato.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tiyhtppz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrejkxu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2viinrmzz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nslwrrry.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tyuttntx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nxyngalf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hzliouoe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jtlgffcw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hkhacnmu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dgtlumro.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rddmaqqq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2aayzayvx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fyapgjhr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kteyywqe.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gisyuraz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rqeolnux.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2knvqdphh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sggaxkbg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nurymkmp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qneflsfo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2taqwkguw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bodlfyml.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2scyblrba.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2tmxatpal.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vmnnwods.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hawtbult.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqmvevon.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yngahrue.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2saxhwrbr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pjxlpikg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oyooaxps.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2abyaemuj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoeahrwn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xzzugeaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kljlsrhc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ppxgvlqn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iilxjsxa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2csytevww.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fbziraez.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gdpvbiey.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ecbgmcda.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zwfpdmdg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2sddvwdfp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkkpaqnr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lhrpvjnj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2khrtlfpl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yfztkbrn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibbwkvwg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2githhhwu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2duhlyxma.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tzgfsyle.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gsvmgeba.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiijyewd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2herfjeiu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qbjktvmu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zhqydozd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rgrrelhz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntpzvceu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylscwnlj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gvjnbqef.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ngaxrhva.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hrnnbbnr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcewfsdn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xszopqqi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vynmugaf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tkyiuufe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ftsdswal.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2lotaxmqn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2uvgxnofd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdogoibp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2atvkosdk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mqbbiiov.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xolyjlhb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xkhltgxx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kynsrxso.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cpxvdgbb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ybrvmwgp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhohpbkj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ndgtiwqd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pbglqneu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bfgaqkkq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2axnnwptx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zqqmgowt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2saotndhd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bumqmamu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2slgqvsnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsguicgf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wpubnrxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbribjfd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwzbthym.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gcsyohnb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dedlpoxj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2duwlaceq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hrhcwvyb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2blzsuaat.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2svvwzloy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2aexitasw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2toumvrod.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2htrzljgr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pkfptnfs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jbrhllwq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vtrpdans.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wjgszumv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iqpjgeun.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jkyylycg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yeizekzc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2tpdzresy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pmovshvm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2comalpfr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vietqzip.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hcthgwxu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jgpmfasx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2axhpqnzz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hinstgbu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiosmkhv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cparkdgi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oefgbjjc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2surjrygu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bzpyxtvt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bdeusths.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ofyilwsm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wqjvzshm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2phdugain.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jnmtigxd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2etzkaflb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pvyfogwb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmacggb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gveomoqu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jftbtotr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ebigtyvt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vunbfhsh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gnszcjuy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xhffgvuq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jbamfffj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kntrmchr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pbeuinxa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kdskkopl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vnqvqajd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fztasynx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vifsmcrk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ejpvffof.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2meqjfceo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kvlxguex.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tvhbuxni.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jrkszalp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2woyrtmrp.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2apfletvz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qktevpep.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ozgasalj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ozejeukq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tnsxbsle.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rufllmsl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2krvoeknf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qizpmzyu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ewotoykp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2krrbjvkg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2jnuegnzs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qefmlwji.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bqcecfvw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yomkviuv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ycblhdai.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vhdqnbhb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hfucrbre.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wgbasnom.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2brvbnytk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sjeopfzw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ehcflghh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2nsrvrzta.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2prduwhyr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2imhxlnfq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uysxwgrk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzqniyhe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2oeshizun.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aqnkphsf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2pmfenkyp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ezoyyblo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlrtwakl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pfmcecju.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2opjmnsjv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xcmstkyx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2gdzcwuci.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2brustgwu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2eacmeshh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gehuomma.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jqpwjueb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rvajfzkx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ovuhbgzu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2anffnsqg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vqxbznww.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2geugpctk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mdxjwlmm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uckykatf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vysrnggy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2czmdlbcw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hzjnnuwr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oppjyqyf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2itfcabgq.html


<!-- 参考信息 -->