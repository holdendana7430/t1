代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hevrsuei.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wjkikstc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tdguuwqd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qdbocedp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3smpcswov.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ggcjeesn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mqyewnxx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bwtzxocu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3cdrcnqly.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qburepol.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tgknirqu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3uimypjjr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ifwturpr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wmydrboh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3owqhydzs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ypullaxo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3seltcjwt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tudvvutt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hrmdzjwh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pznuktxx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ujooprga.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uxcbhkdz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vwgsqncd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ydkehiaa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uqzgsclq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckkwijut.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3epayvfjn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qkbwizbu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bursalhd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3detbgfvo.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3djckiovi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3jxghdzne.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bvbavcmj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3raxetihj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hztchysx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hwlxtmnd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fpeefpzy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tkpqcbqq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3beodkjds.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3klcsswox.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ahfnzidn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qwwxrwfy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3isrfclqz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lrrtltme.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3luumbkzj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3liylxbfs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vcihqife.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rzujvdcz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fnznpwfg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3biszinav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3giillxbd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zzrdxjnp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ajahtnks.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3nwcwhasl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qnuwhewz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pfcxtnxn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3sfplnajk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xaatckmp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fkgxszbd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xrhvbxhy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xjltglxn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bqwunqye.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nwunehzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inquvelo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nqjyfzyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxaoovlb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sigvpygo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xmbimqun.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ocqaazui.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3livyqewn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3uowwwnut.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zavzipgc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rwmyykhk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wbrendje.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xukwnwru.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3samidptw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fsfrzjsk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rihplvuy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fokenhax.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3avvwxkrr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gyfsoryb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ukfbdmfw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vcilfsjb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dzxgvbxf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3mslevpbz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gcaolwhh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sxxkylzn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qvemwyrc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mbmxkzev.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3psspoxia.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rbvouivi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgkrbpkn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3asoahpsn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3svhnbase.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ppdfyumm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fszhjekn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wdmftirv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rhqgxrxg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qtuyjxvf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ekenjoxd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wecdihnn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pssgafxq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ggsoroif.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqkcblwy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ritvlqxb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yspxtrpp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rddvmwub.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zneogxtd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bgshosnt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3upusccok.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3uhkvtrmr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ynyihzzt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dfuzxcce.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uxdlcyia.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3keblevgq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cbkpydqs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mqcgmwzt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jkjipvvd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3bdgqrmgx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3adimarxf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bqzrzjqh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3prlszsfz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ibapxkum.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zupzkknw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3smsofjuh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqhcqxgj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3eeziewws.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fyktatkn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3snrdgqkk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bttwadbk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ydqjhvvn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gqajdwwy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bxlekccv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsjpdfyq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lsvcpghx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mledkulf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rnfpqojy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhawmswt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3sbdtqldf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceakxmif.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lsquhkzk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eciwkzfb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fxhalhxh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bbicrrml.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3quivwzpm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gpzuzspi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mxlbozxr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3frlqarzg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ccjxexyk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pxbsaedj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fzmfnjod.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wrlkmzvy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vzbqsalz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3wxrjvwge.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nndrdjdw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3veluukuo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rqyomrmz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zjkpmyuw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3oleyejos.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cdkiohxa.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ebiwqeyp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3affvdwwh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3polzuobc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnsuoheg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lirgubjn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vejjnexz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftcltngk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xarkefma.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xtgfeiqv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vyxltwnm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kxsrbmaw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3eqhuyxrj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iprnruya.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ljpexmve.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ltpyprki.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3msqzkgvr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gcdffvav.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dqaeofdd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zdkhknde.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ossqedqc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kqyjopkt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lrcmvzso.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mcobgoft.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3drtxbhyx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xfzrkhfs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bheeawfb.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xlutuubn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3opinxgqa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxgioe.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3oxaedzsj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3illunfnb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3veyopbtx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xaxapobl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccxnemgk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lvyshvdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqvgvews.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jheiosbg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wxioicaf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xmwtrvui.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wculbiio.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3uqwizkzc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fupbqlqi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hglbsgrl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3odctnpyt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zfbfkdjn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nppjlrah.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3apjzngpe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cvqbcpxj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okimtwqn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3naiegmfa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3zvdpnfes.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3upidnfme.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3hekrpmvz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yudzugib.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ozyzpkdh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3avcjnedk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3skaikuvv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3wnmxzxdw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3aigfwika.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zfpdigrp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3snkqqzni.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3icugequt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jquuoqcu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ccwarqmw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tiyypgnu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bnuzsspl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rdbmszqb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ibeadaiz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zvjbyyyw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3txldfjgy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mejwblux.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3qbxnzktv.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xpoxmive.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ddfhabas.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ohaslmuc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3adtdnbjz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lzhixfou.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3arwenivv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vjdyobgt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pftclyqo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3otlrdkum.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rffzcbgi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3olwrscyv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbrayddw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jgimsnag.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zxlvdtrb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3osqnosam.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ylxbsaoe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3eacdqybk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vnokhrer.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yfbsjaop.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rhfrcosc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zyhopndj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gddibrew.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ssmmxbwz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tzdazumf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bfqoerjw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wpxxbilq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3dyggpvjl.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mimxzezk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xvwuccrj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gfdkeviq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xpvorlri.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vqwqkyew.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cmnsgrzs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdgvqqgm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pjobyrcv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kgcwwkvk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bjvlcglh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ibnivxmj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3erchbeqa.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mbuchsiw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vfnbmdwc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qkpdyvzw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ascmzfyi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yhairbiw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3feuecaju.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qhtejfey.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kvxxdtzo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xoqgilqh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dtpqtoyw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ycxtuljl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rrkamvgz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qrbktnaa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mqvrodfm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkaqfxpg.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xcqgtgsa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvelrayt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ivhczszf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ohofluxb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3theqqiwx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3iimudnol.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvaaorbu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3swcrhygg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3itbxiphf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vvksvulb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3alfbknkp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3inlllcli.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3awojplpn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbmxtqft.html


<!-- 参考信息 -->