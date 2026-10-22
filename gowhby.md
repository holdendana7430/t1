代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ktwgfzpa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2maqlorvy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xiygtufb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ctydajck.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqzvjz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nsmkhlmn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jekoezzg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2klzqlckw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kaozoftj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpptbkia.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2npkzbfut.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2sghcjfjv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2czrrxoek.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ypticyoz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tbsaxxou.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kthlvmbt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2stovexap.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vzbirhtp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pnvivlso.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jrqcgpvy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2oyiyuioa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bqppvfrr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ewvlubqi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mbsybaor.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2ajfjozwi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wdjqgjwq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2owwocfso.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjihhiof.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2gqaaskvl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mywkgvmy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xwilykmg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qtkwucci.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2sfcavjqr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2idcuqayh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2stxztdvk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zfrtfomb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kehfezqr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mbttmgrv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rugunydx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2uadifimr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qtjgalmv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mfmanzjd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zmhxwfqx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xxmrgzex.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljvyakrj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2oodhnjma.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nsbhqcru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yairnrvx.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aamzvekm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwcamzom.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tavrdqdm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ufbumkeu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2samabdqd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zxbmhehe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ezyxvsaw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mpcopopy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gtawvwks.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2vxcoawml.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2htdpbynu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2espyhxof.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zwncoxho.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vaqolgco.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uwqacjtx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kddxqyjv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zdwcszws.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vnhftfgs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dpwkqppi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qjzbhaac.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pbknfvzk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2axuphudg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2poeqomtv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oencjnxk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2suyjaaqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2volbyhza.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2whojagvv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gpdtvcbs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hcfvdmjl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jdgwjiee.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2brdtfegf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vnyclbyg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ajfwlaof.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dxsmzwfv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2abjfiwjo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vikwwaxi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ftocjqcn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hsxbixlj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fwnfcutf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oibrfiuy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sejdsjzq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mycnisvg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ykwmengk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2piombozu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jptdhppx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2soubludr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rixhnguf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vjutqtgq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ukwboawl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2msmrmytg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bndeuzqn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bsnpbkqa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vkinlxkz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dkhxucpj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uwbfogwe.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ceipngdu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cabkmzmw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2wnetadna.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ktmqqsap.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xcebzcjd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sguseyfz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kpcaxnyl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2egqsfekv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2merdcetx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oojhpqak.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mhgkuvgr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rhigbiss.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qpdhovpq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2evmuezua.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pefhmaxh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqltypst.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2grjarvtz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2epeuivlc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rcstoltr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2chssyiki.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tvcnhkxx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2uqzimgzg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iojsuhaw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zlganebp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzuughaf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2pljenxxc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nefcxxcm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tcpqaouz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vuiwedgo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2namplozu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qwmbaalh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rnngkmbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fmttzwlh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ppdarvrg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2permodde.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtyeqzkt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ikaqgqmr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vqzklkez.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ljemwsjb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rwposoup.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvamxdsb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nyzzlogs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2esuelodd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gnvwmyfs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nbovgqdl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2iiktvwha.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xtucqgkl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwwnwjfd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ujshfuad.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qnohrotq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2thlgswbg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jtaumhja.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dmochpzv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qdpupnmm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nzfsdcmo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gpvagauj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jhkojvln.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahsvlfrg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wqayxujj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2wftckpbc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2asllmvja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2juanckii.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lejuaoip.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kgcrbtla.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2lfhjtuwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyxbyamt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uycmaxgy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjgttwcq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zqgtozww.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oycmahvh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zvrcjvrs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2bpowtrgc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fuvetufb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jcvbuymo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwzeblzj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nkgjhgbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aolkfcuf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jmezzuzs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xrbqactj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bgwsigew.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xpuwjdwi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2beavxlfr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hpoegkos.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kbccenet.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ljyzrxca.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qxighzgt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uaniuqqo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ivqrkity.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zkbixadq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eynmexqh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnqmbavx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2okyyziab.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rbwnrvwr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yoieeqti.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bfubsqan.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gelwfuvr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qokbssoa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ikncfdqc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ugmqwirj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kgaavdrb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jdbtzqxu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xsvrlrhy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzyrmygz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pwhryrhj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2hfncmebz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2skfrjmem.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yeuoftka.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2acbftamt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2reviplay.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nbpswtux.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tvbpivnx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sssaicqi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pcnjtapz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jsgeassu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2omlhluqo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2kcuemgbv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pcwfmnak.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gxptsddp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mqdzyima.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2djhfmvwv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iwrwopff.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wedrhvmf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyqrcqa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xttadfnu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nxwigstl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fdlbpqcc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rnmerqab.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2oggskspi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2pzbofike.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gxodhtbu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kpiqorwg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2slpjlnmc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2idetntua.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2armxteuo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2yanuuyrp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2melqzfoc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qddicfei.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nuwbisat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bhgzjphc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ggzwitaf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bgzzrvcy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2txvfimud.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cwqnumxt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mhtdcteh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sebutlpe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ermzpiew.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wmilioxj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2jhjmdmyl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kozbigjh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2stiwrmtj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ddkqktui.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2huxthsmv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qpbbxklt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzzczn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xjqqdscc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2dndjrcma.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ifcwnsfo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lqhdzxbi.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dpygsvtm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fwskhjrj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2weqrtman.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lplptkpb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ntnybzag.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2svcbunms.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfpstau.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uorgaqtb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cmahmqnx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zbqiguhj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2uskxqwqm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tboexuvk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxyqxzmc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ubhzuofi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fbmxgmjz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wdybyoek.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cxsmsefl.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uwgwchzz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qiytrgfy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fssmbnmn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2czpyzmql.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kadyfmsu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2qcxkrtju.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ogbumwss.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gmnvmcja.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2caeeijou.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rvhuuzpl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2oociqrzi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eetvdmxa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qhzuzwes.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wrdfrbnt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mmhyelil.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qedaifgi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhhbbzx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2adlooseb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kyzahyoe.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfklnjer.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xzldtqgf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kchuoqss.html


<!-- 参考信息 -->