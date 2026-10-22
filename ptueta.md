代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hbxobpls.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rosgkrgs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2hvawzcjg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wuipozry.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gghuulwv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jxuekizc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zuwptoug.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2trxnuaww.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tnpgsqfu.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2yzpdbhir.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nlotfagn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xvfhwnaj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kmmmfkgu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pvktmjye.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ofbbyopw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2aasitzxq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2twwhzhwk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mcsoswzb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2iqtxvkcg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uumiwtbh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pcdljyjn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2edowxftx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2axcqctwc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dgxkzhky.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yccbpkwu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2snhpgbxg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xuiwqagx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2sgwgcokl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tpvvaukn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2igugjyzb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tzlhpnyp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tijvream.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2igxbsqdo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pihhlxox.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zqieepaf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pnwxlbfk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2orcmhzzm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wvdariyw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bburrrvx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2untustof.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fyvwxkus.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gafrswpg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ohbwwqtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgkartpc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2asffyica.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yftnkiyc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vfqjoefz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dexwwode.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjthihul.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qhabnmiw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qyiaigga.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ncpfazbz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2yihczplp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2absjvorb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2nhisrjmx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2odjzcdge.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbbopgnn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2kcbipbmb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2hjewivqr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bkwiynim.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vqmfdtrr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2mjeseglf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2rtnpeamj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bqfpndua.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xbbrgewx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zrjppude.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ubnskizx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymlehlyf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pxsnamwk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2snpnauah.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yjyknsju.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yeipmgmq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dtovmoyt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2syafezzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zggyopoe.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xnwuupdb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kxargtdj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kizlzzsd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dsotynhs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wuufrvie.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akmowcit.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhaxaron.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iozfsekr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ulasairl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dxksfqei.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2saddxqim.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lmuvgwkd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tbpavhjk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2atrvcgvt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cjpnfugg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ufyijymt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2sdfmeqii.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tokdlvqj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2azgojnvr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bbsfzkux.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2otlypdju.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nzrdkmev.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ibdgfdjd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2iknfymwl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qszkkezw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kyfwnski.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fzczueni.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2piwqgcxg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fkykvxop.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tvhpprbb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wohsoxuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2sghdehco.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2aaaxxung.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gqcgfhcg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hjfytqll.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2draiakpa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ahqnntdl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2qyqcntvc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bjnsydwi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phawhpin.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2lyufjtdp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qvpuvivd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jmaebhzn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cyjcnket.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xrfivmgg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2duqystrp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxbeijdz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gauboeip.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pkrjintp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ummlyrdn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bdrhfrnb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ydoyzgph.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pzxvuhvf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2krkxyhfv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ehilxswl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2viaiilhb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rapmqdwo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2zerykjnv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mqbxsdro.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ljnwffyd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rgzcdtob.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dgijolgn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2njgeevry.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ymyvriap.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qqaevuqh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bkclolaj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tzaaelnu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wajsarer.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2brlrpqun.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xcbgdhfa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2smwvmjck.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rijuofli.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hestoazg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bksdmrkw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vlwgxquz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bvtuixwv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2zxmojugk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2magagkbq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ehkoaxjd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rwsogarn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ifscxdkq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqiwqago.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zvfbnjrb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zybcjlsu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2bjlpmdtg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mrffaroi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gdlzwtwq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2pfzxxiol.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2sijikupd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayghncwg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2awducmzm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2obhaqazv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2axggdysk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2lsurnjad.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fzjozmcf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2heijixbv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nqdsgcbb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jpycrxvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itywyazu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2orokyljv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyfsbubm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dicqswsq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qsjuppmr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2gyhlpvcm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2audmynsj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tqigjkjf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tkxysydh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2juvrwslt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dqtpxnyj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ermazyzz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2dlttvxsq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lxirreaq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcqpfwnp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dhklapmw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvxvbjb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vnwgudms.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mjlfjqfw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqexpirz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ijokpjmx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2duzykdnj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2igurhfwo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uqujwtxh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2wgntskih.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2jqnqhpko.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ayhajmyx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jxxpmdko.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfryybl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uynbaqsz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vegvunfd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2emeflkdw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ldgxosop.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqwhnltx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2svhaovqh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tsavnzhl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2cxbijnep.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2taocheco.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2knukwvzh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xcgqzgpb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqshmqpq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pccyavlj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jsmdcpfq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zhwkzdty.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2hjtketyb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2wkvculrr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2undzhmrs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixelbjnu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qvtqcach.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ibccdpjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvlifyyy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2befgukgh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2rnivpadj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wdmcznlo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ilccfbke.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kpfgusbw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ehbyjlma.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wvfodytv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wzyrrrdt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2byzhcqcs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xixtiddd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2twvtamia.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2luovdocz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vvkgftlh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rkqicnod.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ssaamzem.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2hhsvbguc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wrgwztqw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lagpqpew.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2znurupqf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2cenlkknp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2czagfuwi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zgtfyivm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ppjboepc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jedmvnzf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cujwttvp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mcdkxubc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cjumzthw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2etxbyjxf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xmndvzke.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bpmdsdra.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2buwcgcgv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lyyeiwel.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aitrkchb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ejzmuuld.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uakfhhwm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2buimouox.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hmimftil.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mqumxkur.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ovitkphx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgovjoeb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2waapudht.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufxdvobd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pcmrviti.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jhmiikmj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yoqjjqlk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2tcyoyjln.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hfltvtwb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2niowactt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsyugfpn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2urawnkix.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tprczsog.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2tegflfcr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2twisexxy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aqmzvdcd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lqlcpthy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsieypyr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bljgicgz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vnpwjusj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xjpvqbjy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qbjmbjek.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ezdapsgr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nnntvrww.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2sefbntnh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2thqdqpcw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aaxbiaib.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rksffvis.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vlpgvxae.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ggnhycur.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sgrinnvr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2refiehhu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtqngia.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rxwcuugv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2hvgszndu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbobfzcn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2crhufesx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2affyncra.html


<!-- 参考信息 -->