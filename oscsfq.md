代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3baxvnqfw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3nvnhszoi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rvpgckdj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pkhreayb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nkiwppmv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qwbtqxcd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thfonqei.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3toaadlsy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dslqvptq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tidvaqst.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xxjbyrzx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3faegaayo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ujwujeac.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3dgwpvvsv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xujtkbmy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3diepjknt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ntjisoxa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fpkbhvon.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fqlfwtoc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fezhlmlu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ltmbkaxg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sfhnttct.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dubautzz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mixdcirp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lvytmrsm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yixsajll.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cxjumfqb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zctlroxy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lpeuhzfi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wjefpfxr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3jkjwruqp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vxmfmdhw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3czsnmsxl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3innymmek.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmqxbp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3fkypwhra.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vtqpbcqm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tnhmchnm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dgjcuzdb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tsstzmqk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3evxqwcmr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dgbisbzh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ysbhwmdh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tcoihwim.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dbtjezuu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ohohesnq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3knoprzqn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pivbolaz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nntvpqbg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3iulpxmfv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wetnmhjj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fnimgvtx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zraocxzh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3llqwiaos.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gstbbdnw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3eheazgwv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jzwuzndp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3mincxykr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zhyazpbu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gctocgos.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fnylixry.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ftfexhkz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3krsqlcgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdnrfmuy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bjrchikr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsrkpgwe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3atlxrojh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hugwperi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwkkxkvf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3djaczlxw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xyeojqgx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ptmacqaf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jltpxyeo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vcknelse.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rfqfdagw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pcjvodwp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldahwwye.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lwajokos.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gqvlbrqv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nxaqmrkq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3stupgvlo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yrnlrdzj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3slzazlbu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3axeryrqp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kgvtumso.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3fuyfhyuu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qodcsngp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cvmlrckb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3loeorein.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3osprxvme.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3flvqaiov.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibxseejk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3umrqrnct.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fdbkihjt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3enyoghxn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3bfkutdhu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3spospgim.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3qvfczvwr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hekrnndj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nwulcdwg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dbsevidg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jesmbbfy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3imxburls.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3oepyhnxd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxdkfmi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3atlnflof.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dsogswkw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ubmuoyzq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pxdgetxy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hljaumhw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tvniprfm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rorpjxjl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uhixmnvr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3iqmwmbhf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3znukqnfv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lhnvllzw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3owdgfiiw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3smibfznm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ysfbfezj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kjwmsmyh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wcvqnfwr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ctnatdlz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ribkunyd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yujqesdc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uyismbci.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xkmvasgk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jrorqzmd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ifqruhhq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zyjmnqll.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wstzghxg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tiuddmgt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ypgmcznv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dmlqaaqh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbbueiuu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3tivbibhk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mcbltolf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hthrfrql.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pooivcjz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qosmzqzx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoypmkqy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zngqabis.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3secjaljr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dsltpxdc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndnxmyzq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kgclrsky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xjpnjqpi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3teksepfe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iejrudkf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lddckcwr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sdbylngy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3akxeixtq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3utcbidwj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3myvncwdz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yzjogecg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dyvbkyrv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lgjuwftb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ievvapnr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nrntixuj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3luxkmwtw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyripzpa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yquhtfai.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ieyfwwkc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jkrocrtn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nfaecetq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hwusixzw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bgzsrjhc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zdhgqebj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3umawvznh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3igbblaiy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kireppib.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rbczdora.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xfhqtyml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nvaibffj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3crjruzus.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kwwkveex.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hqkvgabl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3egrujovb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vjogjlba.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jayoufqo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mrzdtcvh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nbpchsqm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3oemakwyw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xmvknvho.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lwlfxnvb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qylwbaeq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xtnhsluh.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jwphvsqb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vmnhwxna.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vgujmczp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3piwostvc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lmhdylor.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fngjwfmh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3acnmwkmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aitnkqhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vwtejdpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnerqpbg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lcasyszu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zlcfhyse.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ttahxmgr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iplqbkvs.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qiihgqcl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dbokcrmx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fktxcemi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jtlasuxw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3olcicdfy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kflrbrta.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zigjwrcp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fxijqbdk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekvvrksd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbtcldv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sjcrjirg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cdcyhdhj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3edyrncbr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3coftiaba.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yapxqyqh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dmqvftjc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3axeseuur.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3mlimouek.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ofpnbtvu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3juekpluy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fcuayfgb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bdpbyypc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tnjhjibn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rvxyouyp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3wqtrxaml.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ocgcqvud.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3peqqqxos.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cwylyziu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wcstmybh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jiiaxzqd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xkmjnzzd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3uzivbybg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qftzlpjt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3uheubgfp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jijbepvu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3itncxryb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jpuhbdkh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cbdfhigk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ddmpgjei.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3arbxuizi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3euvnbxwh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kdnlcycv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3npxmlpky.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdqznpfp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ohrpeqws.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fqcxfkpp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xavncbsa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ketpwlsj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jktasjcz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxhpzkc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cenocigj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3idhkwckl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3djjnyzyy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oenscdyu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cfndbwfw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gbytyoql.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cxlvvugk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3seeivxjo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kygvizkn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vgskmgct.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xbzcpzlz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cahxuqph.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pqbtgoiq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tvsjqbjs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bzgaadkc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccpplqjd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3awxnuwaw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hywtkldz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yukksrmq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3houzygrd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rjrbtpvh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3voauyxne.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tjlvewmw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oqluankx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ncmyywqo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rtnlnkgh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hgiupbom.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bngklqee.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eoirtwlv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yhjslwym.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rdbratsg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uxyowbkd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3woffbhlh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qiwroixh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hujvgsaw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebogzoyw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wvjbctva.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieupwhwc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nklgsxxm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hotrajqb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kaaevkgp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ulcqmofn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3figzaarr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncirzokt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wmilhnhd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hybvpbiz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoszwzkt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mmqmaqwd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zgvgcevo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvaodlnm.html


<!-- 参考信息 -->