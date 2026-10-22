代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uuzcmjsy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqzmrufk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2hvwdkthg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fuzteuhw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xvmzbawi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2oiqjbuya.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uqnlljrm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dtgjdyqu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cknrupws.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2villknfp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jerseeim.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kfcatwvt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rzhxbcnr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kppzqual.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hsdmdewm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2aqfmgwqp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oqclirgf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwmuomyr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2srrahjmx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2syzrnvon.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hotncezb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qwojmtwu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wxffbvfx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yffclxzg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2oeckkkpi.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vtsjwtiw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nihvxarj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yqvkxjrr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rprpyiig.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dzzorkms.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2fvsftqdb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wagnunba.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tchadvaz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xnfrhcof.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dllutwth.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ioweyoif.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2upbhqizw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2joohhstc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2exvdkpum.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mhmstdsz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cdvyykek.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fiaklukh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cpgyilhp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2niledqdl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bnwubzsj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsxgkzwg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hluvxkno.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ygbzfojm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lgfgqwan.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2epbsahpy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vpegvdtz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uhvjujpk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wjknjujq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2oflqnuun.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2upiqfwfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xiacwxtb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2irkccbdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhijnzui.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kwszcwby.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2onozoqsk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mlvctkno.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2utijvjwp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hqojzfev.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2flgntqit.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mebtlook.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jmhjkark.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uxplxhki.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xhgzsyyp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qlhuvtbu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtnjaa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2soiuykai.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dixkwolq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ojfpybzv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2guhhkaoc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lxlgwlyo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2vwgafeqa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nbhcceyz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2vgalmiqt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xtuvlsdp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvwvgkbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ivrwawle.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ckzimtmh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mhlihgbr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdufiezr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kqbezpfx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yibjcigh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2unwgxsyf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2acmzgrdq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lvawruhd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pdkjkoak.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uouhdlrv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zborhnzc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2avelqljo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vpootwnb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kxtsnqxv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyyboozr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfdtxjv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nonostfj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2icvbmaff.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gtiipwal.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zjpgyocb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2eltvutwv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2roswlfkk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kkmswxiz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qblkwsjv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uifhaiki.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2adybbniy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wbchydpp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2njpqcgpt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qbztklft.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2aklkhbcc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ssxeeydp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kjurakig.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2txdjjcjg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ypwydfiq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mgwwpmsh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qjespavl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnknpbcw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2sgmbbace.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bkyrdwtb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rncrmmrj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vfbrbxwe.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2fnfbtbdx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ovngynfw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dwvbpovg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ygikfrrn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wkulhcvd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rjxiccqw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2qcnzavio.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xgmvcyxn.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ziqcetqw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kwwfoeru.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2muxsfyai.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fmbgxjpg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mxyyzcrv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qjahnlhf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2sfhfdfcf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vulhfrlr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2eurnqjrn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fajmqesr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2nsuszqxd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bzgxltko.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ltudemfo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dalbjaab.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vnvhqcji.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hrjrmfuh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mvdiqvti.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2owrxgaqx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ockzhidd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gwiccknn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gfirqlan.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2krnpavbu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bxtesjdc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qehvyoum.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xdqmkmht.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2erlfmidf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hzpholee.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pbwfkozr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2woxmmiuj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2aeikyetz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mksqjebo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlmsawmf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2svxithwj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ieveswzc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fneolmwl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2btxcbtnj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vfshqkqg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zcwqbbkw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ydakjler.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jnenuqyp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2uvnducmz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2poreeoli.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nynlzyhm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ighgvvtz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qoxfxwgr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zodcyzab.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2chibqwcc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hwemqybw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ghrvocsm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jiwyrrjo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2scwtzgof.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vovupaip.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2togcbnlg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qywilmnb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dgvntfdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iltcgtuf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rtaotowu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2midkleop.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2goaybhjk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ptylqkla.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfljuvko.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2czyxbloc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qnlkzkuo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xkxdrujy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nwzecvqk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2oamzplyt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fkqwpvjt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2osbqebno.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2manxoswa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fwcichej.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jyqyvwoj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2viciyfaq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nozqufxz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wxbvjkqg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dcnodfpc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2nvqqpfnp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2tiewhcdo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qtsyfpzq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ympvvomi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzkzyha.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2rafjrlka.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nixgnmvt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2krndcqoc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqccklk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2iovtsycb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zbzcycic.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jlycjowf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nglklaxn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ucvuadxe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nuozqsul.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2hdrczxvb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tlshygzm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mfmhqfcz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jaluuxgi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lrbucezz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2mbqekwat.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2szbpgxgh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2optefnqa.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2urivrjui.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2alafplee.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qvqxhnku.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2xklufwst.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2htxvnuqw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2iwgcocxu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2niymskfy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gprpmigg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fjwuwcjn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vcmrkvhq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2obtslfdj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dpjbmldq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wyfxqxph.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hqfdkxaq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kxuemkji.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2eiyxjzjj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qhphtwgn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qifenoiw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gbcftwpe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2glmqyjsw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hhlpwczy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ehsrvtbg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ozmgjeze.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpmsfzui.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2juhzrlxt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lzldxeoy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gnyyvvlq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zamvwbmc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2moghvmmw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hwfueelk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2agtttcsi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ntielxha.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pvugfvjg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ccfcxyap.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2juxbxtyr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lxqhnlwk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xqvfrvhd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2onrxsoyn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cxfrybae.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ybdrpxbd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wtenidfz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pfcgehxb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qktdocup.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ioaqakjp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tccmwcbe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2vzqptlat.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yuusdknp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nrizphtm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zcqoooqs.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rzlyhsvt.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2neukdtls.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2tpylbnvf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kftynxal.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioefqkka.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yrygiarf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nqxaaqgu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovonculu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqdszjvg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ysggpeds.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2lramgdaj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gmrlrjat.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sdrecsfa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uwieyjxu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2goahdcnn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ryyapvnw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wfmqvnlw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yhdbakuh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gexxjdez.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubicazyq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lrzpqwco.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqeuvxrm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rybykquc.html


<!-- 参考信息 -->