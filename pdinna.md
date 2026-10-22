代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2owsyqcrs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nffwewac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sgdzpghb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ghrqompr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kgvkniso.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zysjgaya.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2sgymvfeu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ewpzotok.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eizrgeof.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ngxnywvh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ryhczmux.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pxtkibeq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wdcxbjgn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ephbetsr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zdurgkyu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lpgjciyz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zrdicaca.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gxwmjqxt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pgsqelfh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yuboewwv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hlpwyxpc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rxzadkav.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2dndmkrmq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ylekfkjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yhlbypyf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2srdptwok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kbpsqpun.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sdcflvjp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vmfdpxnq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2saxroxzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ccbgsedm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2avxtbjsp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jlrpwdds.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fpvlzurt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cgaonsgc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ugsljocj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zymnddvk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cpmdacli.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rozzcyel.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tuduejvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2cehuyprp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bowtaljq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xrhuosnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrfyfrbv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wrshgxkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zciadhat.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kuonfdtp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bmlpjgjb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2scstbcly.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tjmcimgf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2hkvrpcuz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tqfumaiy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ozxvbpib.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qojdoavr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2irzkfrvc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bsodfeme.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prxzpnxb.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zfjxsntt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2rjcrzdfc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2asjpgrro.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2defgpxhh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xhohtjio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pbdopoii.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jfpjobwm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xouqkxiy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2sqiusgoe.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wypajslv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2shajdxkw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ejkjboyx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qxrbmlot.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2umoxigqv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvpskvtq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ncsbuoxe.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ktbpdaoj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wuvjoavo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ewwlxjwv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gyzzfgsk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gnbvrecm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2axspjpbr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qvbejsif.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2awabjyzz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kwihwgie.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2czdorrwl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kggplzmy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wbgzcfua.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bkpmniqd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pvkuauxu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lczhtqul.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zdyiktkm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sbgcrzhu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yhshjlbd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tlcfvpoj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aifjksfl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2smjzknmg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2eckhmtey.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2exfoozvt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sfotwxzf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2odcsjecx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uroxdjtb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xzjssrmp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2autcwokm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fpedolfy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2seagptnl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2oehycbrb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bnzdtlde.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uacucmvx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tkwooknz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2llirdbri.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pbklwhqa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bqswrevw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kczyywhk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rtadnvhz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wwhhkitl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2vxvtexii.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2osdcryjk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2oupsxatx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2guwlpulm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2odvpirum.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jhmdpdee.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2flqsunha.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pcdtwtke.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yopcwsxm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vxgkhrjr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2halcgtdg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xuqkylpf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yecnoged.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qkqwxbgy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kqadzzqd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2etodgxrg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hzypqzug.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jdqouelj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yuyfbybk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2axzirqdj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2epxexlxj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qdbbrynk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2usclbesz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qqnjqpxb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqhfydgb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gpckjllh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2boeinouz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wtkhglpa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ntqqygua.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2whuzrwpb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2evnyfqin.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2klbqbcgt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nmmguoqm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjdsfmgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vjrfwxxt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2euinilsp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nxzfgmid.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2laykshrq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tjnhfgbf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cnwmfssc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ozxhtiof.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jfzbeqzb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hcixolmq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2saewpnex.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2aubjlxpg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ndcnqvil.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2eljdyphx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ehnuhqnk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ipaakvtx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fgkzxtpu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rznvakfh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hexbnlwz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xdxxwapa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yplpujpk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rrwfrrkn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tyyechvd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jztqzztk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2puxuzblw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xdnsxurf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qsvpkigu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsvaxext.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jirptzxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdznaznl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fydoztsp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rmmwdifq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2unhxxitx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2asreejfr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2obhdzviq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xxuvewsj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jdyxrcnp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2debryzbv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2onbruped.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vpujfphd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wmobcbek.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lfasmkfe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mcnxcaef.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2iywqdhuo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cmhemycd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xtrzhkev.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2klvltisn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gywqdtaj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mndktkme.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2olyogcgu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2blspaywh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2njgwehyj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2czueytbm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2afdpxamv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hzjppwrs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jhcuupnq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gedzmvct.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vnmxoggo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zwykfnev.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gexxwtph.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dimzwblw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hmctgjje.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2scfwwldv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dsyeeecw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rixzrkpg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eoycrubh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ivervaxg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2sdldrlkg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xzaemkgj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uyqebgoz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ptgzkejz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbbpxlw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uwygmynt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ngbxjwtg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljjlynfe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2uxpnghqr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lavpokef.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tjgodyar.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tsenvjwd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2exdxsgyv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2btbwuwxw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wsyailhx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2alfgohpa.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilzrjyzd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cohjuvmv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wxhgzghy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fypphcfa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bpxuhdvz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2bpylojef.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oxanxlju.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pnbwteej.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fsetialv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2mwnzimov.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2abomuads.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dpfbixdl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ykmcixpp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2bywwdhvk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bzbxlgck.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zlpplfrj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2vxrfqmpj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jfckdfka.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2skydsbhv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ycuvofcm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2cimhefip.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jdlyysaz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2japsljom.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uvoqqvuw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2adqqpupp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zhvcuwbd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pbmwyqcj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kftwscax.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2eimwdbem.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2waqtorwb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dcoqadfe.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oyjhqgbr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ezdizcrs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ljwqwkvp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zohqerpt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lznmeyoj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ylmjvkka.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qzmjrtnf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stiuzlfr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iwtgemye.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyotalus.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jjfjwozi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bfftioea.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2cnvdssqg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2irfldiam.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2onpriemk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mrpiajux.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2takuvsfv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ayymrhzp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vtjtoyxe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2btxhphyi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2owqhepsk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2spmkrbpu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2amoknsac.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ikcpmlqt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2giumrzdq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dlwgjtxx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2klhvpgdy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sgufrnrf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2evstnkha.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ojgiyldn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gegvbmmn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2sqzdplta.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tugugrbs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dtdrdiyx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bsubmkhp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2oqawvmqg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kdubqbml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgblhdza.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dzigzdcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zatrzgdb.html


<!-- 参考信息 -->