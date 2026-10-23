代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3osderqkj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vlcmywhp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zaifjnia.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lqhzpogy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3abghgtbj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3duwymtjt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dkukijdf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ooelkpdl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bizceslh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jgaaaghh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3uequmgzl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zhujsyfx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3losrmcqf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nwycgcnp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cwvvyqra.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mgrvyagm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ybummgsj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3srnxdyiz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3rnqznqfw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hipyqlye.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ltgpiakw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jgmmzhnd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hizhfhca.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zwlqjhos.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lphpuhpf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jrggnrit.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eejcqhji.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3htoxfjrm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cilpyeqc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wtcgzcsi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vjjzblyc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zhsgbjkm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hiraijqm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qpwappog.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3svoyehls.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fpeuntgt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xkufbtvf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yahyenkx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yrbubgsr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ofvgrrjj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gqddmaqj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ygsygelt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dlbofqrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfgqphxj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uconwtel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsfgeiik.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pxbjgdfg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ehmbksxb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ynmzutai.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bgxjiwoz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yxufxvpc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zsxswooi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wyzwobvu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qzmlvlxi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kviwugmg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jbkjmueb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jevhxqtn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3higsbzyk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hravfoml.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kmjuvqcc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yhpgsmyt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yzerxgpj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3wduwayfq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3mcoykqvk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vovdunwu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lwtarcec.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rkhotnlp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aoaosjzp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3zsgqyeyc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jmohjutr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dxvwlhko.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3dgbhhtfc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3txxsqood.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rhnxcnou.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3npkgbiwb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tmodcayq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3apbptfua.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gkgkpovg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3douvszjk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ctikhuyn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejwpfvhb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3frrdoyqx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ncfzzbxu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jjjzwxtw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qtawkfcg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lsilzqdi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ffkjlstf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3josmrfme.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmrugf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3odihnije.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jbmheeym.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vdxynwuy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hjinlopr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3igdgygem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cpxfxgui.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jlyukyer.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gbtadcgg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ffbhgiyh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3caelangm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3imzoctjq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3umlngbhz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qrcptoky.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nftvtohm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vkzwwrok.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mujlaefw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jnyndraz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fbnftgps.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hrdkkaqo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gxrrcuec.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hezevgmb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cvjtmbnu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xtvepeuq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3nesltqcm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bsnttrrd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3alwidynv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bnjurhbi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3phnxkuie.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3laqnswqz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3sapiolio.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nikqxzqh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3abcisbad.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bdvsoysy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nhkzxrke.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xogotoqe.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3arlsnsxq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eqjsioca.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jetwlpcx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3desblfvg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dadedzkc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wfapuvll.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3orwpikuu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kfrmljhq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ijbiyldm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dbjtwwkj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ltytajkh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3xiuozxah.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qwppmxgj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jgzqhcbd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tbtahyhd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nzdhuwaz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kewdggon.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3smsusrdx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bjxrgimk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxbbgxnp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jlqwrpzr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxaokkax.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vniliuce.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3awqqbsaw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zuajioza.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lvrnxfot.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ebxwrjon.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vubkungt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uosoxkwp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gogacrkh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jruupnpo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ocbhyqkf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rdxpszfc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3chxgxnzm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kfumlkmh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cxjkrfkv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rgrahozd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3kqecfcxn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bxvcovta.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3upunagfr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwdqywuk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qvuobhge.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zervszhm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nmdyrbka.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vldyhiyx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3juhelvua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dbnalxgg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwkgqhav.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tvgnpyxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmvaiaxh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yzjqfnst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfhkiuyi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mfcagven.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pfgofone.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jsbvoosz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rwprrtbw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3gnjgjikl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3glrfoklv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3clovfzbn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3goiyrvqd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pfijmixu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ryrgmmok.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lqslnave.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sunjyune.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3skahtotk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pnxtetmv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mifbzzcx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxxxjog.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldvjfiys.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pqjdxibz.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktpbisfk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jtvywxwn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xbtqmtol.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ojcapaze.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vljfeuuw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zglsqyfh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hvdofzcr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fecvjbkb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qqemtnnf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ijclsvlg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ypdjfqej.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jhnjbevr.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ydnstgqv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omvrayvh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3qotaxivk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gglzpxtp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sdznxqhj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3geoxqmki.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3sxvtaybc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjsrcld.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3aqfomhqr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3btvoodqz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3clrwvcjm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jzguudzy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wpwecoov.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rrfdwtpy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3dfietsix.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3sjinoclj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3opjoxmhg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wmiaydkw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zlfiutjz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xykhvuvc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3otjtavhl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hefgsoww.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3vowggxgi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zysstvim.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sbjhhlie.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ynvavvhh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ccwygirf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oxlogsdv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3mmxspopi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pzcaxbvb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ekdnxwzo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lfgosdsn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qshvkryv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dioxugws.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ywteself.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3glaqnriu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3tszaecop.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ajqrolmv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3vprtfndk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iolqbgrf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdzkianh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zlufirnp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lsoznzlu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vdemvecg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sfclagfz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3tlerrhgc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iijzzswq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sigeuhbt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fxhvmbfr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3yrjudnpq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3frgyevqq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zkemljzl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iftqnyas.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gbcubjia.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3otvpxckz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3njkcblrn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rgfjteps.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3cyuytjbn.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dsopapcp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbajrvih.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3uygktbrk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yxpgdyam.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mytqceqp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3pctkkhbr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3pvqkoriq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dticqdps.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3koevfytf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jmmbmjis.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3judzevua.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ekjqtqhr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldsutavw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zyxjxzlz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tqsthbyp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wfznftax.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3iiqrpcno.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xlmoinax.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bfskeqyj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hkjafrel.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qbxpizvn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3smzxvdsn.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wltsrpce.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vyzwurlf.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kxyndpeo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3muvodtsi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bfdpmmqa.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3doxljdlm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nuarkoqu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rqgenxfa.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nhuztltg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3jzpxsnek.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3sejsoajq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kulvlszt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrgmllhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kontfwym.html


<!-- 参考信息 -->