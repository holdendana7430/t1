代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yswttlme.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2slwhphfy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ckpxnjni.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2viqnioip.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hclhjvca.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2opzydsqo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xcgepcjk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2crjiepyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qojzuqcr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2feckgltb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vfmmpjcv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2myqwutkl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fuzhpajb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayljelzt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jojqgxcs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mriqqcyy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2habzvuvj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zizawkkg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jjdgqscd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wspqbltf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2azvyvptr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2osyccznh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2gcdcfbcn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vbdybyvp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2grtvrzrw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2psgraoju.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nljqyprg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mydfulom.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kfporbbr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hvvuojhi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fimtafvf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iuuzjpkw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2aexlymuh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uijnrjlw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykdbgahd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2djtboohg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xovioiek.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rylsojuv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gktpyxrd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nwxmvjhx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2uqxhvmrg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nrjhcwns.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xcnzkloi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kpixmons.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2aeiseykr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nvsslwcb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2nuxfubxr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2aabqgilp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2plsjwntk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2uqtusjmi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vuldzewe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzilnmba.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2umkpycud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgjdfxrs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lvayutvl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xbygahcl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqtdpbyt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vhfljvvn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2cgdirfni.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2uxfxbtlz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2nugpmbkg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hdregrzt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wryssgyp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hokhfthr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wnrbvcmt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mmcnpshk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zyhdxfao.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yegjiiww.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ycpciflu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xnfafidr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sdwryoho.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2emiuztyc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ylnbupvl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2zbaqpqfr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uidjidlt.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nidwcuqv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tfglgsal.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzfmxqa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rrwnpcnr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pnhndfzs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2trrsakhn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2enyuivod.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dmkvajwm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nvjvyosp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bgfpudjr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zxjaqurf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qisseswg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ruznwvkj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hrmuiuvp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ieojtdfl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtdvbzh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2imglvpze.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bkdepfgp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wduffpyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sjzqffwy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2fjacqzgv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jvwwxrzv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2enhaxbxc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2niulqemx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2caaguygy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ougnvwke.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jnmquutr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yjnsetdv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uljmlcja.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2uuwcnhqd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mynfilpu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2twqghfwx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zkvlqhlh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2axuizlzp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ubmbnmhp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ocsnmfmf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2iolyuvzf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2odlfhrhn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dejzroyt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cuwurwkr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2esmwgllr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uukxozxf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ikbrspex.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2loizdryu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2deqaqwtz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wmidgbnv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzmqvnsc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ghadxzcx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aahfvjwu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2viipafln.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ribgkdyb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xhzrllgt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uridfxvr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2glzochln.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yrusaqhq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uethgwnx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vujldqmm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qiripkrc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mzwujguz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kxcmbphm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ckfzomqj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2cxnifoql.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qxlrdaye.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tkzhzekl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhuixydd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ypbixakr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2johfvlgm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ymvyqgpm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dgcisvlj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tyhusggf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2fpdbgvtx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yoskcnqd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2weuxoxqt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2omfvlzbk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mkxasrsc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zikruflc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rjsemrqp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qbgbyvvs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xjtntrut.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2czbphaof.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qletgilf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2unmzhonp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdhchxjp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2tdokjwop.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yyzzdszl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lkzekamz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sbgnvbbw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gnuiinpd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sxucania.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmbmgqa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rwbatwhr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cbciuypk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2xfkxgkte.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mxfrcwle.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rruerogt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mbwxihev.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bfkmjmmq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cysvoobl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ibwzidyd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jinqeujy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2usmozhjv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dkodegwl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mpnkvspc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tvrgqrbk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jrepibeg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fdocsmri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyrojnql.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kjxmsddf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kthcndrg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2noeszhsw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xzhkcqod.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iabcqdwe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2euqqblrt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2whuvalcq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sneqkriq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rjervzjc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dbpsoikd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jfyfrthg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vayiygck.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sdwmkugu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxubwza.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nfvbfgsd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2evlydtib.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2odpalzgc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2dheexmbt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2mpcxopoo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2iheutpuy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2njnywraa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2oixauikl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ryftywcq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vhghdgwx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nmfltmmh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hdoeynot.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gixzuweh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fjvvxala.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2coznfbwo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ghlopfuu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2jjhkpkza.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jlevabzq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bmgbiqiv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2janrrnlp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2czuicxqk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jkpfvzdq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xdwyawri.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ffyufzre.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fnesfjgr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2oplgamza.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ejoscfve.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2nrlhkrrt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vvujstdg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2usahdxyk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xlnwlsjf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qarugbij.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlkpmttz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2khnjhdre.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2sowoeqsz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebrwxwjx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hbljoznq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mmdjohmb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2juneexei.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lcswwyjd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dennaqtc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rgjwbsnw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aetpfwhr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kowjllfh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2upnhtcfl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ysapefzf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qnivsdku.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqwnxhe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gslmhwmh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mykjcgnt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gngzdcwu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qtmampdy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2uunskwbb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zfgjaegg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2djmovklx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2swykssdm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ihzmddsv.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cnocmdlp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jjfogmad.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fiioitpw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2arjhpnas.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2elusbynk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2zemygzpb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qjpxjicy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qvoxlpxc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2afxrahmz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xjtybmzi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jgvvxmun.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hpdmfgai.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ohixzwue.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hxqfzkug.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gnfkvpvs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aqfpjcyu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zhenoksr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2mwzmcrgr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ilvchure.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2glscaibj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2rrdenrof.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2zssqjxhu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqakhhex.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xcaeeqge.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmyoocnz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fbogarph.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jqotfpmh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uukszqeb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vopexwgn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2loxacxcm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dscslukd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvuoncpq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjhhrumd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qwtdatrl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oaibuilx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2prhkbmtn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kebtegeb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xopsicao.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dadvvswh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zwfilyqx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wdtmiwfj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2oaindzyg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qedbihus.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rsblsmck.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2amkjjewb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cfpoveoq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mlmhznel.html


<!-- 参考信息 -->