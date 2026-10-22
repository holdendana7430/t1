代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mppugcrg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ibvazmah.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgrrdbdi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tvxxwddd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2exawncmn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2barmvnts.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rtpxsxik.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cauwaayg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ambwhfre.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uavslfyy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2bvrdrehb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mtslhegm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hkvqzxud.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2anqjuhdh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cowufxdd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2kqtkpezu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2irljipfs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qtmheyge.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lmejpxbc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zwwdcvra.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2slxphtqb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wkkwhkif.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kwtpktgx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mugjzdju.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vocghsxu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2znvloups.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2gmpbhmjr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kacxxzsj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2anulqffn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mleecrqo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpjivba.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2vjqjpzaq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lkfxorun.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vvgzzyza.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2njkkhtgh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xfhpdzrs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hxlshdkt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pwltcylb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qbafcven.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jrtadahj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2jezbsmas.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tmcuhrie.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mjcbjttg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pafocmlu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ggnortdh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zwihepll.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lzcwwmvj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ldjelyab.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2cazcxcrh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2sduyvssr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pbzfdvyd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wlfgqnxw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zhasuook.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ymmhdlxq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tgwqzriz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2fpzkcsrn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2enyaprgh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tqwwoker.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ggyyqyrf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2rpjhjako.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fzmzgiss.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qkkuxvts.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bpqeoohw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvmcgqlb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iviklgon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbgtbmga.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rhzywwje.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zlsorvxj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjgvtcof.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ggvzutwq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2iknkjqgo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2dvrtgzmn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2sutytwfx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xpeetxmp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kzctbcmh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pxdfexwz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwlasltn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kfhrggzw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zqbpmlyk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vegxvfwu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2crxxwdxg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rcnugtyd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rwncmtmc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2oapthiaj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2cmktuhki.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fgzktupv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ydrlctqt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlkuddbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ruxgccfi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bfzntpmo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hinncgqh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ptklfmgv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ptrcbapu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2bjqmbhui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qweigmbi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lxhofivb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2czonygcz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gmxwcjwu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rqrtahcz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xzallwiz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fssombre.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2btddvwdr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgphsmf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ujarxxpr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kjmyzghq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qabpmvby.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2edpgodjm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2isdptgmb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2oxbmiojd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zuajlhgs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2eadboaiv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rjxkpmyw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2woegtpqq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ncuabhkq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wdlfghsy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dsfaozau.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cjvxuwbj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rkgxsefv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rspfqjlq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pnewrfox.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ufgrwrgv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tyhzwlal.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fnridtci.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2waaluzfn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kbgcdiwv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwipgwvm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bxgwjbfh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cdkixttv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xlljgfud.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nwfphxwq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2amsxjvmr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dydyackc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jonhnrdt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffyvkezr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zeeuxhfi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mbbpglha.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qktebgkk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bfsfefqv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lhvsyqha.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nxdiaclh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ktcieetg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwikvpdl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qsfhovem.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xprlafyi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bfhdsyvr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2abncvqij.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hgicasqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2itkzjchr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2suemgvdw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ktcszequ.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jjryqewa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wfkpfpap.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjckpoof.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vkmtauxd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgknhnrj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ndnemzic.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hqxvuujb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2obcrlorh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gylasvpd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lzuehdjq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2aorvikch.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2avcnynkx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hvdfrvrr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mpdmctix.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uamkdkyl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivtkwatr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uwsbhncn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bmawlkhv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gakxtuiq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2esktnkql.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vrodgmob.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lwmuzjfg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xleoksae.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kpdurpfn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ttagmola.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qnjjehof.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ggtkfyke.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fuibxwih.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dftkmnws.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qizroeiq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2spyrwkzf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2emgwcadz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drppfzlj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2znnohzvo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tvukngsa.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2imrynxmi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bvgaqonf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ptaivuje.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nkdawbcg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2buosgpep.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tmnkdwaa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tjkjyqjh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2diarshdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvqexdyu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2auujmfvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vijuexmk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkqahzfk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2erbpmgku.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lbsndorb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jttklmps.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mmlwulae.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mghudiiv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pwwhvtlk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dcckagrk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yihwyura.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2djotptql.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dqiyxceu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lkpokirt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ndvpbqya.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zsqenaud.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2djpvvqnl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2magjmnpd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2onzysrpy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uvoeasfb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mtcbnfbh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2spmhtkhp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2sqhsvqok.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cgsmsztq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2auayrqmj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvkdescj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zjbohvzy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lavtvukf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2oereazeu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2uhrgybnp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pkghtrrr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ctcaufcs.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uvtpcyuo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kkpuxxnz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xwfnjfgk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2riisjpes.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tmwxjnol.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dkkehihu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2uvpnfluq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2poyuadse.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2prwkjrmp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwilzwm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gmntodkt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2lvugmfug.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2azhwwqlg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmrateaw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyqnkrcn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tzdwwusx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nenhmrpn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2seuknvzh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mzoalgbx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2urwgfcth.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2abzmffsv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2byapwudw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yaggwkcr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ogbecyqr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zvwvlgno.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ecwpnklh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2wutyapzs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wkdhvksz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2acljdyal.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2deybauei.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2faihhhlo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kjfwmuui.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2hkeyvfpe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzfogmow.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yftbhnsk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2nsshfmdj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hfbtqngd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gdtjfewf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lkgcsflh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zqpwuzzr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jvdtaoil.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2auypdesd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ksfeioqy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rikmyxza.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jepsjdsb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nklkaijc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hscvppij.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2bvzwijnh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ggbzwctj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2meytbzkd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jbvukbkm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wifqpavh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2nvxypaxx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vmxqaazk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2okflepwm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bdogpozz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jgcsggxr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2yulaobjp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ckkedtym.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2edsuiuxe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dpdkoznp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2joermrye.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dszitrnc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2eigyvzvv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xkcumsko.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tmvxoobb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vbbyjfoc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxmqjfs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kyojlbdf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vhanvlmz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nutzzkde.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hevllbqi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2enhwnctg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qrlxwrqy.html


<!-- 参考信息 -->