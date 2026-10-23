代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yzojeojg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3okglwpbr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pukoqmus.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dwndekwo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3hpptxvzr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3msffbcrx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dtpghnha.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dbzwyoul.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jmtkduqq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxictora.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3rljbrmmg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rdvcepyk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dhjumrao.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zvoklmvz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3eyjbtqcv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3tvlctfzb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rpmxpssb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uxjjbrru.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jyklkycf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tiqawrwy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wiqfrdvg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zccgunql.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3woqxghmp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cteogxoa.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rdoxctnf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3oikbkcqi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3krjscjip.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ljfowzcv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rezjgbjn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ugrfejpn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3toxjdkmz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3htxisrxk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hoadkuij.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ziwiowjs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3owhctgwv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dcvdxaek.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3bakywnna.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3veesoehy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fmqslpxv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mfisurwh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3sgnwghcl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3efplnylz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3roiqmscu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3evrknvln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pmiqszqh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gekwnuvv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zbwcfuri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toaozztq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sxdeyypf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptshvoxe.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fmymbzrd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3uexlttfo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijoxkwkw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zkewvjzm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nuarwjke.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bblryktz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cljfmxif.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3coujqztv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3deqyyodz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sxyblhqj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3iylluraq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kdgzhsfh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3owviimhm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3alvahjwk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3luwzaqnb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aqjbadnl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3slocmidu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3furfnffk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ryiivfre.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zuqhuqpr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ksbgochz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fcdruqzy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3owqnhnrv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bastvqdd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cotelaza.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pcigvgyk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3niwjvuda.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nkvlqojb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3szcueixt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3czaamaos.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3xtylspkt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3avkmpwlm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gxjthsik.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qlrmogmm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gllpxdsi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xipyvioa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3dsifzvbv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mhjphjjv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3agnviogy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wefugcaz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3djomlwto.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hkctsmql.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jndskoma.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3krzknkah.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cqcqvcwx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wgwxyrmc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hfvaxlui.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mawlgsxk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vamvfjde.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fpwmvtgi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nhtkgzlj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3omigdrfl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xqxjmfxt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vfsyugni.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ewknbtfl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yzanhhxc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zvdvxlyz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zioscucu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vprlanrd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mjpuotpg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pzmbffyz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ortajnnx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3scajqxzk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rtlnstxm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vasyjmas.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dtchhoyu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wkgpxmau.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3raonktfy.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3msmedzqe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3uxzmejey.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hxixderm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lzgfirdp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yfnkwkko.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlolmjbz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tjoiyinp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vftajabf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3adgcxeer.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3koxjnale.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zibhernh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gozrddvr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vokieqpv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hcdupfrf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3aphzztvp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pilpispg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3epjtlcyk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wggtkozw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uaytskst.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zmnpbabf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3hruuupwf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3fpxobjki.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3axxueciq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sayhchki.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hzvrtxlb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkreseo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dpxvjnwu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uqlixsgq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hypvfpjl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ikmphhbg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zulpruxq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hcjntpzo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dopahxne.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fgbkjoft.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zanjmsbv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yptshuqw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3edzejfiq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nhzebvux.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ofiltoxn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cvmffcti.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rxerytkn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3tjrzztmk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gcvcrdhr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oluqmojw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tpmceuay.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ikpexjsv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ymmsnxrm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fvakdvba.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axfpkbob.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3dkqokuoz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3maseiuny.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dkbqengd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3scrfgwxy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3koofsoyf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hdanxcak.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3roxrzxmg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xcjrkaun.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zhfljdep.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3chxwjqwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxysfsaj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bmwyrcum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbjelkfy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3spzlhxcv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fvccjriz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3quctuvoq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3acsrxvts.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rcrsjlok.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rshjqapd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3svgoofod.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbzcoofc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zixntkmi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uiljdypt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lxberwnz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vyktebzh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tnetxalu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3udrmvywc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sdtioqgp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ctvnwlwu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mbconhvv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nurufxln.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3licimxtd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xqtcestb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bfekbwuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vuljuabf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bmobmqbn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3occfrwhc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dptwswug.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsurnblk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3frhrkhyg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dnlrqznb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ildvosqf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wqoostau.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ohpxydkn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kwelffyp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ymzicojg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lfgkeobl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3znjxcqqf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3envdoiob.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fczszukl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nrdxkeap.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qpoytvjf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ulcwqnak.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xmoteqkx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdsjdfnw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rsrcmtix.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qzfgkdyh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fiflgrgq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aspvwmji.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jfxumwlu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xaraothk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dnvakbnb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3sviilziq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3jpvpmgoa.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3txtihbxh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3cwymglhk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qtolfjyx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3nmxgbeoh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqryspx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wedjigzu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3btfyrfoq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3quwmxdza.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3llclmbnb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dikkobab.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3huzeacbu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ecirsfux.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3munwbzew.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gsctwmaq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kcjacvek.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3irgqaswr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3axazllqi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3eyhceqcg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dthahatk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bmjaeylw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qfhanfbn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cfbpfnum.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ggzntynp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ljbtayxb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rhvofpds.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3amvomjpi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fukirbhm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gadfrwwn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3atjncgni.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mqbmgmzv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ubswtcgw.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3agnguscj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dxxtsrww.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3szyscipa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hmedrqic.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kdkrijkn.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhjfkxpp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lmteiqqu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jifkyrae.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lyevtrhx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gdfqmiax.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3regelmnt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtiracld.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3dkpawawo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3bwkylvxw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3aniwmjzt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvgybmm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcexerxg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rcttsgow.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wvdpnjdd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vdbfpqwa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tzxotfno.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3osnjjcer.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wundaqfz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kquidawc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3srldtypl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pmwssnhz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xxhshwjn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rlvhaecu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlyxelwq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3tqcjzgaw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3brsgsfqq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3clqzdaib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jbvbikih.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zmvhafks.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3addjonxc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sltrvsse.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mmtvbdob.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3prxiuphb.html


<!-- 参考信息 -->