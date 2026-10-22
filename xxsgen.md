代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jhifnqsl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cnbsfcxu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uznppahc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mysslsqh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jrtnwldu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbfwocel.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2sxxgykcr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2onamquld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nsgixxou.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sbnfurzn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bztrwlab.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2aazwmyri.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mcoqulox.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bqzceqpw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fretxiwl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hshbnqme.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hsczkaro.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ntvjpmhx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rublgfjd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mncaustm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ndipodwb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrqkfbfk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2akegnhpm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2enlglooo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hwktwgoi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eyhjnikl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2rkstqvea.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ejkjqyce.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jjcirzpg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2muwoozab.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2acvjujfb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2viipmnip.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pvqsegaq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2miybepnw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2madzjzrp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iflprajp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2smnxchjy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2axbzvibi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uaudlxso.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kleerros.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2esznbcwd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wgrfnmda.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wnduzwud.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2aoaaktek.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2axmcnfbg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2drgvtgpn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dzlnipoq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2swxtsfyo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ugcriocz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zsdnicgs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dqdhdhwy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kytefimq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rjnrhquf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2syppzkal.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mphgbpwn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2keyexbfa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2posdlecb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mphqdqpb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dlbquuzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avylpmxe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fscfxalp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dilaldlf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2thnqjfzk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2eaqapbfe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jbdkchsn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ljgugasr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gwoszgby.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rsnflsvj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kdyjcaue.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kcnvnjhn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wztuqftw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pjdlmcvx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xciqfdqm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cthhuypy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xquekaaw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xyjffjqu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zdrrqqbh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2txahghab.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2krezxeth.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fwlpnmot.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ijqzdnfi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uutqqzor.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2czkqepjb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hbuykwfk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2jybetdfc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qoyqyomw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kvypvcyp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ksocbwlm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zxukrmsv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qgnqixip.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qjoycyij.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bpyafkaf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fofellbv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2auoszsoa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ofsgwvnw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2caygcyqe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dydgtets.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jrhzjavt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uznkvofg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xhexwxwq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fwsajncn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jzugxajr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fwsngkus.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ecvdtbuz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ezmcekxv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tzfspakt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cqtszobc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2pagqahhi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cfuxmjzq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hslrblcb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jglbfvyb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2iepawqli.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2abhdgcmh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zepvtxaa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xrrpmehv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jwtnuebw.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qjadcfcj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2acdyuydn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aahbqpog.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2eoasraua.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nrxwzyyu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nebrgdei.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hxdykiyf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2sfvoqmxu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2lonhvivj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2umrxkwmu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2pifgdbus.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fwkxshbf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qsudinbo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nszledga.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ntmogsdb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jrqftvks.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bbiyahoj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tsbiemdo.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2onymgugf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kuuouxdr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2rmnrfgpm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2agmvkdio.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cvkulckl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2daqmdhvh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ibryfrwx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vhdrtcxa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uizlrcfz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tiuqllvh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2rzzwmuch.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zlklupbm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mnzargjz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2iuudsupw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aoqwkpqu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pupynete.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yfogppcb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cphavpux.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tbbgqqiu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cduvpldf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iyngvehh.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vdndwjto.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mkzukjsa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yztaaqcs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fpqykbss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2owgvqcnk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iyobgtad.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2mcjullwx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xghrhemg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2inulpbgw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tsdmxxab.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yzbgxryo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2fhzemfcy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qzlydvyr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2goztvqpo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tnbultsr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jagydjjp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2woefpteu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pdievldm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bcfkukpn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2oeawhrrm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2sretupdz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xryakeez.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ijipkobz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zemgbofq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2icmhfrvd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnnzevcc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ofaytrcq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cspmcigr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ayjxdyok.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rbclrdlf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ezjqiwrw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2pleaquqq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cthfxptz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dbcmjsnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgcgnnig.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ntdprdem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsbsjptf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zjkblbev.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vwsqqebz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kiofmrdv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pwiuxxpq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rbopxeqs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cwqghpvq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wtyjkrgn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2trwgjkvx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xhllcwzc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hegnueid.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sgmtsxaw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgkmcquf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2atglsgpq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhkmicy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dmpoqndv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zpviclma.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxqxrepc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2eofujwrs.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2yrglvrzp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2eozdjmnb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hwslprbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2usfgldai.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nydebuui.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmmssegq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2remkyajv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocunvfem.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2widnxval.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ompgfmdc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gtoaoruw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hrqrfpyr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sdyjiign.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2czojqdub.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2oxwyvrhn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hmgsneba.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rkjavgca.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ardbluez.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yndwraow.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bjkfwsgi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fefyxfmp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpwmcxfe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bhlnzkjc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2onfpgofn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2udtuoayi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hdrozpag.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yclfzhzg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2kobomxge.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vmpocjcl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qxugnfgl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tzhfabyo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xwwpbmdo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lzmspixj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2popblxby.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ejxolbfe.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2eooxzqfr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pyfaxhxs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2umervhvq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lrjypjxl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2exzhukhy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wgipewsc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dsptjkky.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vogikvrz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xjkicmmd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gofwcjjr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nesimuuu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vnezyaij.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xzqpdtwu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xbcihxci.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2gpqppisn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2sdylpypi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2uzxkeahb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujdncbaa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wutxezos.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2blhpswhh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2galejxrr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2trqyvhdc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2sszwexdx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hzestvcm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ghpkynka.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ectmaqxz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ivaensgm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dzwudwqk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2itibctll.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nhcjmubn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zoedxcnx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jmmuauqe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2uzqbrkpz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ltlkydtc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iawtdksx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pfjlshzp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2dmhivqpo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lkcsisjv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jyyjfxln.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2inlbvizq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2cngewele.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ttuxpbgg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2terwepme.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2aqwswibm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sescaocp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lmhpldin.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qhqpkmkk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jrdzidls.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkldaf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2trqcfjdx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2saftidzq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dvastpga.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lzruvlor.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2efaivmbn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mzzslxot.html


<!-- 参考信息 -->