代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2weghjtqt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtoeys.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zayvipwx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zktmrhtw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mwztqdgr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hyefauht.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vovtbatn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qftscedp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lqwgtduy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xacopyrl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2scigmnku.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jmbnwbkm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jffcbqae.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rbyvkska.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2clyrlpmu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2micbpmjz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2krzlwtou.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2yanyupwm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sgqpxqeq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2vnjsxqps.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hwhrdqdu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wlrucsww.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hqvgvjeu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ltayteat.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2olmwvrng.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2htboyaos.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2yftbbaxo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jluxizkt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cslstyij.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2knpbanum.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cxwwwnqk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ohupabkj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wssmgoxh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2aqpgdyaw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nyyjzmhn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gelfhcit.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wphujwuj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2orreuhkb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ikvytocj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dkglhzqj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2veswzhfw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lhshzdsj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2minuupmb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2skwpazce.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pbttqdvz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gipzhimd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ueaibvis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxuitsaf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uilzafdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obpuebty.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bxbxyzrl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dsxqibqf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2imxzlzvl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jqzvgllt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2brwmxlyw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pcdwepdf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zmkowpaj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yxorvmkp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdvzof.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yezzqvfn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gbxqjdur.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wifkadty.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2anxlajau.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2aaiuziqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mvedlrwn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2asvjzbdl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpfeuce.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yaetaqde.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hmqutqss.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eplmigtc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2seolyiai.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtihxxih.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2wfyyakoq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yceyrkbq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uankplbk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2iomwunnc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fmgdobbe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fcateopj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mrheplfj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2puvvlufi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ulmfvxzk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnvrpent.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ktlawqpg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nuapjohj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cetueskt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2amzqecvo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kebctbgc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2brvhxclk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2havphamr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nbmbmdyj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hdggkooo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nnmpxewl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jmrbdznr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fuzeiwyw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2igwithcz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cgcdcsou.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2eqctmggk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bumiquuu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zzokepiy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yevvrtic.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zevuchdx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tnsiogaw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wnzrbvtj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bpvjkzsx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tvidxqcy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2egqnclgz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iqxxvqst.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fvwedqur.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mkntsslr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hjfmmgbb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pxeujaop.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hzhjpzhz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mfvndows.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2spsgwsfk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wwexcxjf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2txwfeirm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2oskhrzvc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vpbwkvov.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2uvyjueon.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2epetqpqe.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2cnsxtvus.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2eqjewknq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rpysyecs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2labrftti.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2okiwusiu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hlfdomkt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jflqoqvo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uuooaulj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hjebmasx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zeeqoano.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rgbdzabw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nbezhjhe.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2famqgafi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bvubxjxy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bdapwjsj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mnukycbm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kumzazxr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hnyarskk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yooorbqt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ilgzrvjm.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qachglyp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2unxxacqm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jqierxbl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzwbgffa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2szrhvmpj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kncvqtdb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2shdzgrju.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzqbkix.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uxvgtjvz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2prrtlsbz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygksjega.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2glsrwlwz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ftlbklom.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2caesolxm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2emqbwcmf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fteglskj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tljivlzx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mbljdftl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2jwudialr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2exzwfgcl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uhbapmwv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pzojrlku.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cepuhaxg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dxvsvkcr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ixowefrr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dndheoas.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vpkmxxeh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ivopvnuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wtjhnkik.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2unmgqtav.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2efrvxcaj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2aznbpxvq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vcaomqcn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jwznbech.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2uoisrzyn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ezkparcg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sgswgtua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uswqkeaf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cdadzeql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmbocwro.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vxpwkdst.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hwxoykmg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2xtlhnqpn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pmdacgiu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ubehoenj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ismluwqu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2apwbjdck.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ruruwgkn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wzovnoee.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fdyehcjc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2okrxakny.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2joagxkdi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aesxbajo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2paaefzwi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qvydsatg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2okgsygfi.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yotexcpq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2carxoluf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2obrxmqfc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ucdgwzdu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vmbiodws.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2edrdjazo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2sfbnasbz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pgdtiiin.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2toyfycco.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ovzghgzr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2velyszyn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzdhjpb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2eezfmatb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tsmdyobb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntypfoif.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rhugsyzr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uoarvejd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2qveifpvq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mhoruvkb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bnbyeefz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xepcnkpb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dobknfqq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pxxgwkil.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vmbnrdga.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vtfpqhaa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvvlcaoj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gjildnom.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kiylohka.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hhnfekuk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxkqcxn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kqlspznm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iilcpxoe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lfjxqswx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2neifauek.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dwgwkijv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hornjpxk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lhfwsear.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rrskrbdk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2stvysegy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ahjeikjg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2isxprlzc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oerwcdmf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ydkmxkmd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rvsercub.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sctiwzyi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2myxemhwc.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2lhowovkr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyyokxwo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ditnuvmz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ytctftwt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2vovhweok.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vilkidfm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2apklliwj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2nmfynmbk.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2duedpoja.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ojcevmcu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2lkupzakh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ujdjqoxq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fkrggvfl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jurnvvtk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2slqopqol.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2latdriyg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rixxvpuw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ochpjqvh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ihsyyzhi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2syhfgvdq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ovebyqvn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dvwqfgxq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dkyjzzeh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dkkblmct.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2pueyaolg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzjcxaeb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sibonpzk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2czaxnzcw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2lunrkqsa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbkpqcmz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2jpfsrhkd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kqqqhkyh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2bljsngkq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2gnfdtepc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2dntmwoxj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2stobijml.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bvocmhhq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wfbeylvq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qblbecns.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qzbzqmlo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uovrzuih.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ybopohre.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2btvetszq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ewzniesb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ujewhhbc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wiauwuop.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2aszwjzwp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ttiqsrrv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2baiyrehi.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2edtdgsyf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qovxjvni.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nezdnwyj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vkgjtpfx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mbueewrm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ecvasqqp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ulrusvni.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tioqygjg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2nwoiqjjb.html


<!-- 参考信息 -->