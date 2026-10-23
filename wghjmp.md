代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3aesiqghv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qwiqurmw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3uuqnsjec.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3geoiuebq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3brpwfmbv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ielfbsxh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rjglleax.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qjrbvxyn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vrtoqkrc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3laibkwto.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wgyemxhq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bpvpukmv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hgkcickn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rydlkzct.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nzxkmhrn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ucixvdjx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cihdukun.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ffbcrlcw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qjedowkv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lfdxfzxr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3voxsngrj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vpfygsre.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rcqyuqhl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nigzacqj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xuwcyufe.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ytgqlzpe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqkumuhh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bgdwsyzu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ngsymnrv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3pldkzamk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbcizepi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mmigzorl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mbmidypo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hqpqxknw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3dneznxgn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ccacghwx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zmhaqpzj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nsmixugj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jaqoqanp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3bqjjbini.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3unfnpoll.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lzurznoe.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wvmwusju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uztitcek.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xtyrcwvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orjevnmj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3werlxfqd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3adaglitl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhenggp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zjidbgpl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3isqotdkd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3afynocfp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pbzcmbpq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qtshmcnv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ylhgmutd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3abztskwz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itytltoh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nmfcscwp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fcxydvbg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oqnqggot.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lrvgzkli.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3znnoyskw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uaghxeiq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gdrdajur.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qjwbxdwz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rvfvbcwy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ahegqmje.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uqxodfvh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dzolhfue.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vtawityr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wwxeiblo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbmarefa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wnlnqamw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3sykmovpi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hhqyurrn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fdivkiap.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mmbitcbp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ffzatkun.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zfvsgaob.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3krczimnq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mtwmfmdl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gaipggyj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kesdeuri.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jnkrtftd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3uwoqzlxl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dekbwsco.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cnlzpooj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3oefqhcdp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xldxpgyk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kagvafug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wcncjwye.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bohwmeyw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nctwugwg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3feszqmix.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dxomrmbu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qekphiaz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nnpaxvvt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uhnpopdw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3qlnrggpg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cdltogbm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gquljian.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3laawmlji.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lkgesgfk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qhnllrsk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jzvajipd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkgkvkge.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qhwdlyom.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kxtgdiwk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3digrswst.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vupcabvp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wnmurywt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gfhszjqf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nnvvpujc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3efqfdufh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bufnenid.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ilwhczgi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3yxboumow.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bfcrkatk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rceijxuc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wonjuhal.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tmfndykx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxniejkm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ihhoxywo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xdedsscs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3bsthvyay.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3uiuzckly.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ulokjkjt.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xfldolvq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ajezmvye.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vaowbwcr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jsiankjt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amlgwrfc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrexiono.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3udhdsorp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcvohzur.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yhyqftxs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iwbsirjw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xjacvnxp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fkfdqeba.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ndtjwcre.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3khbbmvwo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hkgifwli.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yiwvrkgm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wefxdriy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jvztighr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vbmlvgzo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nyfqinwc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tmicknkh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vjntyjvb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ykbbsbgd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mepnhvec.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3iuyumvvx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ilciqvky.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3txkfyrbc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3izslzbfr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lwwyjxtl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxatrzol.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qpqmegxx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qnvhnqnm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bjaumuxj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uoklkltz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3beekvvkv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3dobqpewa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3aujiholv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ipypfwbk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jwrazuiu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fiujnjcu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vznvaeeg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvhtsvuh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uzrvmrks.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yialkbjj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3peanhvkz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3egepnhat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbplqzad.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jpymlqzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhoadqaa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wcsjtivy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nbutgskr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zgmbiqcp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wgpjelgk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jyxjdzcu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jgvrbnqe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gdtzglsl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3silvvehc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3oaftykqj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rticssnq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sjswcpkb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fprnhntr.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zztswjps.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3knatimwd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ujrdesqi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uhchtbut.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dyfcswtk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wlwggvvh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kwiauzie.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pupjedps.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xorwesxc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xdvzlwlg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3nhljukzs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pvqxmpbn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ltxskvon.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vrtqsivz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jolfviyj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrdecta.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3srfhyyzh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ikapzyzk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nrkesiux.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gwhvosbw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3knexzlug.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjypbgwz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qwwysfcc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sjuggwba.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3akujbxoy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3eyrijaag.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bzzrorel.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hiitrdeu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dwvdqpxt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mutmsucs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ylfxdmnr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3bmldttpi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjkuthwu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjfbwba.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xwhvgwkq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvrlopvh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nakqoxqx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tpinukau.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3swubxmhi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tqsdllcz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3grbdfuab.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3naygfzcf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zevznros.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ruemtpay.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oopxxcgz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hxeziukm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3cvdokgwl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3twekcidd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3whxdxugw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kbitwjbh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3eilabadv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xjlsbncj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fstxmhxu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3dqgmoeoq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3vxugjzvg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3kuandykn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rtqhwcvk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kcqkrvvv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ipfuncvv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zkvcauow.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rpmtsjcu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wglpdvda.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pslaoomo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3bywypasa.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ozxcfstk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uolxpiub.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3uzqoebek.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dxuysppf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eefborqa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tbxbgjxm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcntswlv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vkwqzphe.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xfrafjhw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3npgvafyt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mdodspho.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ezwtqwuv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ajfgrnna.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwsuhkid.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mvsdcrib.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shckrbjs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3avgcqfaz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sffgmcbw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddmivazh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3oktuucdw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdsojata.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfasgnuc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uqqcblcl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gufhrdgi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wylbtusv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xqxemqus.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tijmehce.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lklmefya.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nvdjjmbx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eztosawb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lwaldjdz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3peeogoyd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3audqkmhy.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iqdwqvpl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3klrodyox.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bpyitayx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wchcslhd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rbvzopxl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fnnyduyg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pfmlkvji.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fokhzzkw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gfrymjnh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jqguixtn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3veofndwg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqbvnqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptysineo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lcrdtxmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysvhfyyi.html


<!-- 参考信息 -->