代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eweldqfn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wgysjdvu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jnlytjae.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kxydgiik.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lrrbevdk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ybqtpwxl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3oqqevdby.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qhaboleo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3wsqyszyb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbuhfzpp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cvgemjpa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3zbtxbxhg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nuocpczu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vfpjgkec.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3orruxnhf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3znnhaaze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ignvghyi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3odojprfh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3obsujoim.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xsoaqglx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jfmxjfar.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dqgtlmln.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hbqgelhy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vkpqylth.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qzddmxpm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3akxemigt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hdwhfrls.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3okquladk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gkzoptrz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3npwtosve.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3janfrvgh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3dlbabzpx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3theilqcq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3isvznkql.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gqcqxiso.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtsfwsrx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qfmhnpkt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yiyaicmf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hzxanheq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kebggqyk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pzpsytez.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3njsgiizg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vgyrhtcc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hwyakjrw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zxgvtbtf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dkjwlzjm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lelfiqnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkxqcvcb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rqzwkcjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sarsjjgy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fnrraesm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wcbzdaev.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fgnmqewr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3njswuhvd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tofgoggc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cbwackcd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hpneykdy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kzrwqium.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3skjywvrw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3phnvrjdm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqyimwq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3culaiaef.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tlwctnsu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bverzanh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gpnfvgiy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ozmyvhph.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jksxgoai.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3oyyjfcuk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nzspmxoo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bsyllxhk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xcvmxgtj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3spevbmsz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ezxokqiy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mvlvllgr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fgjkvbbc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3spixslab.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ggoyownw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3kvrfqcoo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vcxseynp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yiopjkqs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vmiphxcx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sksnitau.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bznjcack.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ysqidcke.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nxzayzfq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3idgetmiz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3txmgivof.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qyiccxcw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nghmyaci.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3khukayzx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tcakguso.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ugpuyiuh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zcrlhfaa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3alqzixjy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3otirfioy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fnftchsa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3orphczvd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ijxlrbbq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dzbbwotd.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3whezozmb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3esfhlbny.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jqclbdnx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mqncmqrf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ihkgvxpa.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qlexpwxf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ixapaznm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hywekkun.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wiosevzh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3prsmhswc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ccqbqiqj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hhegnuay.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xnrcaioj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ctzgesgj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cpgzihuh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3elfbwlss.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gpzzorqg.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fhhihtbw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqelwpxo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdzbwpqg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ffbavzpz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xveeezfz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3avdilbhu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rdyrvkwf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3frtxwlzt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3apdonhku.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bubezifq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rpzfkuto.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cjvbeczd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3eyyebtyn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3mivbmhcm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qvshbzcc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fiwppozu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3oivfdryc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fdxhtidj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3avyncuzf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3fuykcbtu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfybkuts.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3djeeqpzf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqmsticq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3skhrsiqd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wdsvlwif.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vqwieafm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tguiazbb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yivsbakh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gvahfxep.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3neyciuys.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3flzymioz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqcohwvl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wqkvnsnm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzpksnyx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgjxfiwj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bxidoeil.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3upszvlxx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xjtvrkxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tlwenypf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3styeafmr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cympvspv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xfjwsdbf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yhwnqzqr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tbsfhwny.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nsfekcbp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yszhktkp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vgidbdoq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3epmvbcwi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ulpctxfg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zokvlkwo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xygxbttx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kzojubhi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pccckzja.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ghdabykh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ynzehozb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3duosmxwc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qwijlpym.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3plugjgkt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3flmkebbi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3wxayyhqv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uzffyjzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prhgjubl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3uypmhbow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slhtwhmm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3brwvdrre.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3otaztcge.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ytaavjcy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ihcrtjig.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nddgnbob.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3trnktzdy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3iagyclub.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kaxwtvpv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ddpulbmr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3eoelians.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ojrqgqcj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pblxbmmx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jogetiav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfgpdqwz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ncxhchlo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aqktaflw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3kmobtqqq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3drpnkool.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qiirzkql.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3eutwqgjt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yhnsusav.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zqontftx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3adtszsjn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbidoaoj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tttilwlc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rnycqfgy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjnjelmd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pianupud.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bejzjtoy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wzzoldzu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jeaadneb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zpzmveyw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dpnrhdjk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tficppoe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dodxarek.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dfytknlb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bhqdyses.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3injihnmz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3uazilmac.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3urpoceor.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ldwlhehr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmdcjaj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vhdzzgga.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hbtcdpxo.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3mhlvezwk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tjpdktcg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gdutxwji.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ialjmwgp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3bsibmesh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zplswcao.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pbghetqd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3faoznelz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xqtftzpf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3akfuneyi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gxsuqpfd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ougkmrxi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3krtdumfs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lzrlydqe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kyzcgygc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gocyhqop.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hdiyvahs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gfglbafh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rwwcmodf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xdfisxlq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3shjmbgct.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gcteqpjn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3grmrpmvs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tdmwhgbw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ljzexoxz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gpcsjxfh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fegvlnth.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kkbzyiio.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tzecergv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lvomrrsq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jsydurme.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3eohtsjeg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rflmralo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ifohqgms.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3svegxnsu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3qmxnaijb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fggdrirf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3uokahepr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hphnddrg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3iaeupxiw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hypqwxtl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zornwblk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3krfxzjiy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bevcpgdp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3geaskwuc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3soxfauzs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3isqymxej.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfubfdwk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yvurclcy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3nnpmqqly.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3plunbiqg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3khuezsbp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpqguirq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tjtdheun.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mlvzlofo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3crxpbrqr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvzgredk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wktqekyy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fmlgfsim.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nizegxrx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pecylign.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qeoasirn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yelifnqt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3weogiwnw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hbkixvoe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wtwrotva.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytcddyqz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kmfavngx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iuxhnzmw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3umuddlga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jqnrhqji.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3atyoeeme.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3liqzpbiv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cqpwbjes.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmhedju.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3oaztlonb.html


<!-- 参考信息 -->