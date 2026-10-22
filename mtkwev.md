代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2veusaxfy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2qqelribd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hysewlrs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2arprqekw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hcinaxrm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wodeojqp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jcibxmyc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nkwcutxp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2zenfufre.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xchkrvzt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jzpmegcs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ldbumddx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kvdpydwk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gzkapffy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2qtcerkob.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2whosbiuq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wxxhtzdn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mvfwtpue.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ljnnpxam.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2qvqwiytk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rwkfomqg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gpcfurpx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zzxpdeiz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jhfmrwro.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bizkzgdk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dbldvqhx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cgpsqvnm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kkszpadn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2tmfawslz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wyutxkzn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2moerzdkt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ieabsfwj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gimeimoc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tykauzwc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2unudolcr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rokpiigw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2efkhwupq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2stmskhbr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dlvtelgl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xtosfmoq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2npuxinbj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jjpageka.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ryoagrya.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cxzuzytu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cafskejw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yujxdkza.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nfsnqzqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovlktedh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qoghgrym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjsisvwu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lsziaadt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uzqjwnwi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hibqyswj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pzbewrbk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oqasatub.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yujhvsnu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2icrlkpzk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2eebsmykn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2joiqfrai.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2eeaesafw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mwmzennj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ranvjxuh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dieyprrf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2szdwhnkv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hjwmabhz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ztwfhbnm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2szhzzmbh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ekqwctst.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fvvhdkio.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2jlchrmrg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rbcrbqzm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cxjyhdto.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2obfusylf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zlnoabxz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2netrhqug.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2omwlczoo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zwmlphuf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2eonuimbi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bfdavitj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ngbbhtst.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2utwwkmab.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gztejedm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qgrhnohf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hebfewex.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jjslvfko.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jtebkctj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ocgsepof.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vlffesch.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbgenoc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vkojhdrx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wupleivb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hedtaybk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2isztzlfr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qxuopmci.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2enghaxqe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wdgyntlo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2graxsudw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2thtcoqhx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2vhpzlafp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2nuvbfvip.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jpembpkw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vnpxsjjt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2emgljhil.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cvxdykhd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gvrauydf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lowmwwim.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yupqvogx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pngjhyfa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dnsfenjo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qqconhfm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2feelaaqb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2muiqtdlw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2coroovck.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hidusesy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnllye.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gkgypfag.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2xtndncav.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gqhjakly.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rildfaaq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dzwgloah.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2slblxnlb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nezomjkd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2zsaypszi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fujvzwyt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2kacomkbl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xtscyfbj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2dqncwtuu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hhtgfqaa.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kidckvei.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ngarvyvy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gxcgrehk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bklaefam.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wmkjelho.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xarzuccz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2pmuwgyyn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ypglbdmk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvblhnns.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2eynpxrys.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2bxvjpxfn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2szrbyvig.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2razmvdne.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mbhhnfum.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2afunggyu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2eswsqful.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dpaomayp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2uybxxdkl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pzxvdoas.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqjqtxlx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kylyfmzb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hestvqac.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvvrxp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2nhovgdwf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2igywljxz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mmzheapd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2haxlxyth.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2acamizmw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hxygkwqq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ysvtftwp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2iklsjaoo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xrzfwsse.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xiicmwxc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2knggmwnp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2rubxpdwn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2opxhakzb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gulopqqj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2eocfxgvt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gybzpeuq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2cajjjadj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2izzgnhvx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2slsajyuw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dppiwedz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2yotdutwl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cskeixga.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xolfhbub.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vznegsqd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yvqnoisi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2meoyqkqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdncfjbc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mpvvjddv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmmcpwzm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kvqoviar.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yucumupo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2zthlshrf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uhxjcfnc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tcnqxuyq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fjlfvicf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eccrcdji.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lxqyjyxr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zfeyysaz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cmlxvgcg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tyhxywqk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2shylhurm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sixjupre.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ceetdmem.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gnmcomhk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ctpwfyhj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mifmbapx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2khfmuqgv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vtyvjawx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hkrhupbg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2itwfdghw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ztnnogpf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bszvcdzf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruzypgcl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hxgrhldg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugylswph.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2faaljnbl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gacahfre.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnjitt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2frfpepzx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dkgyyocr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bbzyejmn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bgyodbhv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2pulwwqma.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rkfdctha.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kylpuylw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fichuuje.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jrsliktq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yspxawnk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mrwdjwci.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2savziags.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jjulsqlo.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yajrcysk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kqrpjwsx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ofocidux.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uqbkjvwk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vdumdvuz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ycdgoszo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mxrluogh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2nynkhibc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wqgzyfia.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2txdueiqw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mzlrdwai.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ugsuinyk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jcnivrlr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2leirazgh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2roauowoe.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sfhqujcr.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zewmmmxa.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zumgdvhg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cgxkbcxy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uffmigsg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dvmzckvl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uoqzoyxe.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tmynimfw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wdugvxio.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xdlvhypu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sxjhykrb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2spnubsuj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2luncbtoc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sodcapwe.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2urrgbuno.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2krjyoatv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kngljcas.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ohwmruox.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2uvmejfdx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vylzrngm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2blkcxxps.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2lubuzqes.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2crgcsjvi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pjpndvzh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wsnvgeap.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2muqquqqx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bgqendbb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zizmkcbf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tnbakbvx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qmclfwkz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2scqhnlfc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2saayrgok.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ssjbvsnq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vppwwowd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eblwwkek.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sofuuamg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmwtmsqj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nicjfvux.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lndgzvgu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2szourftk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hloaekvr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kafgydnq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lncbpvkg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ibianavp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zjtxshnm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2baiuaxmq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2oginkkfr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2babzuknp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sjceikdn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uiwclgpn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kwsegmid.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exdyxlag.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mgqenblq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pmdwymay.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tgxzvzwh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2yjndmboe.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tfjthniy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2apdbxaak.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2elmhsodd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2btqxnkqa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2srmxktdm.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ignmlthl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kohzbdjf.html


<!-- 参考信息 -->