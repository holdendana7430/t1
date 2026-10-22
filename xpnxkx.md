代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2srcgmetv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2abixarcy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gcttftfo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xsvkzkqm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ogdxwaks.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2deovttir.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hkntykfx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pfwqsntq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zdjkxbzf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ndoxoyfb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qtduuzmr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lhlqagml.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kqryggfn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2euenksps.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mghgqvrm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2uegtopit.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hubwgzom.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vfurhgip.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nyxcgmfm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2dcfgkrjj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ltirqjmg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2umkruroa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bghdlmqz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2etbregzp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bcjtlmqr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tlxhimey.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2eanxqpcl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fwzqtjjk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xxlltixa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ocyhipmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nbgpzvbn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2eshaioee.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zvgsnnqg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lunqcrls.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gswwcowu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bmnlwkge.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xglhwerp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2uthgluku.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2todbcunm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hjzwbazy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2gughjpmd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2luttodji.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bdwalgxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bldvhvif.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ekbngaio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcdmxiyz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dzjwcjoz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bfazngmp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2enpvfxld.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nlrxujnj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gblzsitc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vbjeqsnt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yjqqvzww.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qdhugaud.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdcskheq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qfpkjtrd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzmdbhc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lofjwdlj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wmsumpme.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xveutgfp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2adqczofm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hsovytri.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bvovznrj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2iykyxnxm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lltmgytt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2yoieltek.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2elhjwmtz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfzozduh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cxezodqy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dpxoxfxv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2srtzrxsl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2syyquwak.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2umsjduzd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2joyqurec.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2jajoezhc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tegnwdhp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xhprungp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ovjmlyfh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2opdmzyeq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2essrqmis.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zxdyvkbh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ydosgmww.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fmbuucjr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ssaweomx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ibgdvhqf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2zwdhzuxg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vpgbtuii.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nyevhffn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wqqmtjay.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qyrxlibz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fzwhtqok.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2znbfhdaz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2umtoqvmy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ecxidybz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xndppqpy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fayilyyg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tdaxuuup.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sbrhlvca.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vptrrdac.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2colcdorc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2beiuzbut.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2syvmzsmo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fvhzeynd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lzjleplf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2sxskcohw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqqhxwdx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zsiujiyl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xusbunsj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gruqcpzv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wznsejom.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2akpuyfss.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pelygjdw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2aekyaimb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pcoljynx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gylgobvj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jrvekdmb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zyysjwar.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xpxphews.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hojtaxxf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojakpmfh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ksdjnyfz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2snkwmghl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tkmzphtb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mwsrmnpu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gdgoyysm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ryhqwxis.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pddakyiw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dhpfsqlc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qwewukac.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2etjxxzzq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vmmltbjt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gcczychm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qyfoqipx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ksaugcfi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2idyqgtnj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jczlrxoq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rnzmdaqr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2leykepmd.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oyhhixji.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnmunnwl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lhonpmdw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mglovizb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bxerlexn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zcaftmdj.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2spnrdtnr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnsyuieu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ijxxmcpz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rsqldhkt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wlhdgrfw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpbycale.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2onxhwnut.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ruldutkn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ycrvesrm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wgzivlti.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nnykndom.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hsbuylqh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsutgnnr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2geflgggn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hcfuhhon.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2kodbogdm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2tzjvifra.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2betfnarr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2idvcasna.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ddkfqntc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqnefzll.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sjzynybj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2spiacpkc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zkydmyrt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lmlehyvx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jhkuamti.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zaaftfgg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2wgotiodh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ckshemgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdofomsr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gjxnejwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eizjrsdn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rbfcrpfs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2isrqsmxf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pioqhncp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xfndghdf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qyhbqruq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wdqnqlui.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rbivdutq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zlkybqka.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yqcunkzz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2oebqmvfp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jatcosib.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yiqbvscg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ukkosthr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sybbyfwj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lwzypltd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2uonhmaog.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zjhpkvzg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uyizlrvg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2utafjohm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dpagdepn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mxvkvgjd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lsowlpgk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ynyjwemw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2htocgdhj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rstscugc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lgwywbuf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sulijccy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2izjvbsbz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xpbhghzr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aqmlddlo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2okomwhra.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ztukkzqw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2eouyroln.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2xqlzjiug.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vwlzhwwd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vxvupeqi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2emgykbod.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yvoswjsl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ywaygawd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxehbjk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vsikvcot.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rravyagl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pwzooofz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wsxdolxw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aedndbaq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2efisyenz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ceckkyac.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pskvjpba.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jtipybuq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sclkhssl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lujknoss.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yiawbpln.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2fbixegjj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2yjjscwql.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iobczkvi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2enxjvggy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2iecekbpx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2scnxuppp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ivygrlxn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2aysekiir.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fsavzrwg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ejkaypsd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ayqoneax.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2flqbkqij.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2adishmdx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2aodxdtfi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ubhvdlkb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wdwghrju.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2shlibbjm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uqbzqfaf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tlwuvqoc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zbspfjeo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2myglglrs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2qkfmctuv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oraypsfk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2shopgscr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jsdsbtdm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iaupdfqy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2sxxlesse.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ydzfznfv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yioxxenw.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nacbafyf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzmtymvx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iahflrjn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nkwkntll.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mtfrbshi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kopyrwqf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wcarhhgf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ruvumcvj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ddgxcjul.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dmolhpqr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qupjleob.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qkmywazj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2icjvpyhz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rrjsljpo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2pyfdjtvh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ceknpzai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mzdggrco.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nntugwgv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lmrztxfd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtkqljuo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdjktbcq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eexfqcmt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ujahyvxt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2tevlsoxt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2syxauylh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uhmhoxwj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zzpmtwfg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvuebee.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dhuhudwa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2idtwgaly.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dshbbsmp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2crhgrlko.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qisdoyvl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tuhqpkfk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2holekivf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2lnhgfvla.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mqqphdfz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2etjxlnim.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2aolombkv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ggzuxymn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhvxouvj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jufumtay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mujinqvs.html


<!-- 参考信息 -->