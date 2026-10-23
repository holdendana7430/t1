代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zjjrfmzj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gwurqwua.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vcisrfmc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3kirmxnwr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uzeyqxvy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jefphmxj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ywogonqj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3knbmhmtd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3uqbiwizp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pnvwcrlo.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ajytcdvx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wirngimz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3smnwzcls.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3thqivlvk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lkdyfgbz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nzyvhzgm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fjjinpxc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3faipysgn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dqltwllx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ktnyieix.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xggjsiai.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oerhszok.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3umyqhkxt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3zhwlvvun.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dwkpspos.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kokcdhdt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ezjmjvxh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bqchjjom.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sqjtgxce.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3htdviihx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ljnrmtiu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3laphxvan.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3uhwhathv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3urcceqac.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cwiepsow.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ftvxhmrb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3qzwjjpyp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wbdkflse.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wwjaorkm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3oaiwqnyc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qaezrwvd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vugjbfvs.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ckmzpfib.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qyunuqhj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ytvmuzed.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3jzqzuidz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ysfthfwe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3aiscwfiw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tboxcaac.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ksfjflmk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zrwzbafz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmpfjmhb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jwmdejqb.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3udqnagns.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3impifkvz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dtihtncw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3aejstyyk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hqhwioid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pnmleksd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3uqlvkrqp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkrqesjh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lynfctzm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gmfvnaex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mawrdxsy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vxnsinse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3biekceqg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lxhtljqz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3irgzxzjs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kdqgkokz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3yuxxvhdf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tztnjsta.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3rlvgxrtu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ssibxiwj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3whaovich.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tvfolmxp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tlktqbjv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3damvdvge.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ebbecixl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3rvfpxpcy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3efhggcug.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ecoadoun.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dwnlkxab.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3imvunsip.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eqqhdowx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xvuqmbcj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bihmfjgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rmgkxcwu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpkcwzvb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lxlagfau.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3wongfdts.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jyvkpymg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3crotptpq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lkwknvpj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3znhriakl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mrhnedfa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ouqdmvel.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ikoiolon.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eipgvpkt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yimsupht.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hbvhtgmi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zichjsml.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dezeqmql.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ydqkpzqq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3levzxqiy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jsofzrdo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3wnvddlmf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tglhmibl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3sqwhzyyo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3efcrqhvg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3phsybnku.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3edgmnvet.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3esgsogbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3etrvwueo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tripasae.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mxiinoyl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3udjkolzf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3iehijyvt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zizapulc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ppzueecy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kexitdii.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qfbeqowq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tawltqkd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kojhuafv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pwnvenkp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3uoycakhz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3awcxpclt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mhsrxhir.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gkiokdsw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yzcjifpk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxcgce.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nvlezsrd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vrcczvyw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3auqzvuoj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cuswrryg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uoggkbtb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nnpwlvbu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cesuvlox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qpjgsojn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wrlullws.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnugbtls.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3xjrgssch.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jhixvhlh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tixnckon.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vyigylqg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zschuamf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ygqjjmaz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3osynebrj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nmxfsrka.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vvlrxnjj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jtrjgckp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3gpvjmniz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cffyfpjc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wvmhaodi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mjdazrzi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbxabnwr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cvrdbyxt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3irpmdjrw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oyitftrw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3opefzwtk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3huwnegjx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3sbwedxdg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kkftxgsr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uexkkfdz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwslnfai.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjsuoqex.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dppqvvyj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lvptfdxn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dbuyzifo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qkutgxqp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cnjahryp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hfbdtayq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nchpritn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3loukqqgc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3koxqagnq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vzwosulb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zizvzrls.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsostgxi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tydugrjw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kqawmsoe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3stwktaul.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3odofamqn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3owjfabfy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3duglxsju.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3osgtwjjk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yurslvsp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3aaracpuj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vbgswtal.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hljrgonf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3faotvvfq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jlwymmgv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tujykryd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkmzokrk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bkdfrhne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuyohdrv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xjmzarat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otdomorp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qsievkmu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nobetqum.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mbvsoers.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wnfsylta.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3digbqqgn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cslolkng.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3iecjefat.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dcqckmco.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ebwvaoup.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xggeggkd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ttwktvno.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rtwinbgz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tdyvulav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bsfiekdp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hkierbnj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3oxyrltrn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cyieccis.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ajnzkpms.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tbcyjldu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rsyjabcx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hhaylncd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lhelqxwg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3wxgdmkno.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cprjfwed.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gptyfbuy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ofonwwoe.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kbacjceu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ijvqikmq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gwppvvrf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3imnchugt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xudcnpfk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3srjbfoqj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cyaqbyfu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgeccivb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vnkyovku.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3aurxhloy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bvotjaom.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xafxiyne.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vpqddcet.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3unegqlsf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gjuanxdl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3gaurqwis.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vysnpbii.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dqgpemmb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rvtpojtr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mkdauhau.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3seqodwjh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nnmorvbq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ohhbzkcz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3oowpxltm.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vkewtczv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lkennxoj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3attwhjuw.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3osprktdw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ysikbbcs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jqcghtvy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cplcdpda.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ratubrkc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dlxjmsck.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3athfrzmr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kmrihkll.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pyepievz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptwrpcqh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3erldeutn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fuytpjny.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3gapttxav.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bxkurcqh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dqmnxtlb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zuoopsmt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jnlapcki.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3apmreodp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ujcgfgtr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xprshjpe.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3aevuidhy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jtakppzu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ildsuglp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wlsqphpu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lxxqpwvu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3dlruiwom.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fkvzhouq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hwxurvnn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rsdogsdi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sdfejcre.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3nyhhybgv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rlirshwf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3geqjpmuk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rtifeeqr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sofmedgm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xaisrtur.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpdsgsyd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ysvfnawh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3esxheyyj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ujlgkwoi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcisnqiq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gdipuhfd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3evqklklx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjaffysz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wasdsgtv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dthitzby.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3uidackee.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3imcdlnwd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kndbcxdm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbiwrl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vnhqiebl.html


<!-- 参考信息 -->