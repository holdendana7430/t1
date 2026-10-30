代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gqaizvpoh.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gubzepnqz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gsowonaok.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gfxncazdq.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gmagwoqfx.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/geopsejhc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gmmxokyke.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gspihkkcj.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gplxlhgor.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gkiajopov.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gjjxmkety.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gjuehljjo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/ggejcjbfd.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gfqohclyr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gnwhdfbku.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gcgxnmlbl.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/geagensen.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gzydqxtyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gcfujumav.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/ghonezooy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gofprzqym.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/grzvqmfgi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gpxcicnga.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gfprngquz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gwszjpkgm.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gupdcohjj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfakxbrxh.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gnhpbhjxy.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/grullqokf.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gejukqzlk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gzxoozpbs.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gopnjnuww.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gbdzveaod.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gewhhqfiz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gfckitgyb.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gzjwgllam.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gnrbtdqvp.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/ghrdkhjyj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gdqggbuwu.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gotagqioa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gadntgsqm.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gjncsgutt.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gbcerukkl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gicfpryuy.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gdrsfeodj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghqmastfz.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gclxeyfyn.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gxwougfaf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gkakdglxx.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gijpbnuko.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/glznidrlo.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gsuovfibg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gyhfvlegp.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/ghejfopvj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/ggogkldrb.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gyuxzicis.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdsvwlicr.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gfkxcvouk.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gbsgwfelr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/guznkapit.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gffmlchhm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gzezliiob.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/grxvtzjma.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/glmmvtllh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gcorlqlfu.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gqjcjksmf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gumtovctu.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gmzuxdzfj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gdsofhuif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gslmfujod.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gqghtmrek.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gopbhdycn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/goudxipph.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/guuooznzt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/glnhleqai.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gakulszdz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gubilbzav.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/grwkdpwzd.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gwnrrijhy.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gidlfvdmg.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gppqtomlw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gwqtdtxmz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/grhyopbzt.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gzgbzgxgj.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gjkknximj.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/ghxyvtbrq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gftrkiiop.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gquftgjeu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gpjtnirgz.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gpzfbnsri.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gkcqppgxq.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gzqoeffuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ggsaqxiek.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gcajeqcyb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gnmlgcxvi.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gfqlnhvyr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gglbulmxt.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gooclybjr.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gsdjcsszx.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gcsmloptu.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gtgeljbyd.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gmqlenxpw.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ghuycmxio.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gewenwupx.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gvgdyvowt.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gsebcuzft.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gnnbkhznu.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gpnmjgkhg.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gttfxdrxk.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gggmoeido.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gzatqgbqp.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gszkhszrq.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ghogdyycv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gjdpozqzm.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gxvepskwm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gktofryry.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gdcjqvvfw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gxkuwhpti.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gnuhyeeeb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gzsdvdhbm.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gwabzqyma.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gyakilgwu.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gfrvjxhly.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/garbsedyy.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/grwtrrfsi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gxbfvqhdm.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gxvwcdnyh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gdzevntkl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gjsqnfvam.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gtqwjcuqk.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gkxtfvdon.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gcyvljwkv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gkbdazbuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gvfjeujfi.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gvzrxhdhc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gybitemby.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gpgeccrru.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gpaqkzdij.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gjlvloprm.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gbqljbafg.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/ggvteympa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gxntaquxi.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/geerjsmns.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/ggxatqffz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gcheoqvlm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gahjgdvps.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvwdeuzmm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/ghmmcwtxq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gqoccsdcn.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gypdfvutz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gzqeartmh.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gufzibhjn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ghuwzgsny.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gklrdgwwc.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gcrnpzpxj.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gibejtfwt.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/ggrdpeunt.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gyfgikhcv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gkskitisl.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gocqqbspe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/ggqyvtien.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gqmykoumh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gloyddkbv.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/ggjgvnffu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gtyzfxqym.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gbznfkgrk.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gfhmsujav.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gayvsvtji.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gsejmpgub.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gvvnzjnwm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gddeybodn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gcfxtapto.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gmravxahh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghksaamlk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gasewzrbp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjbtjwjuq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpaplwwmj.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grkdexaqv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmqymggyd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/geicbhfvq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/glnklyyfq.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gjugyvibc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/guypddiez.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gmoiwczvw.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gluyrhfsh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/geuldkcdu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gehegvpiu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/ghgbrxekt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gztibpyrz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gcsvtfedj.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gxanvuocy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gzqhxdtxv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gkhexfpyw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gqlwxgwwh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gnmerffqk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gjrrurzfq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gpdnwmjis.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/genmioxze.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/getrqkxqg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gasnippaa.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gtyzlikzd.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gnxhhohmt.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/grrntszor.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gasokffjv.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gtoqxlkyf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/ghxlgpjmq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtdwlyfru.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gtooextpd.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gksfmxpqk.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gjgizqwxw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gscdfgsox.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gactcdlpa.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gwmrdtwvd.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gtnlwwrlk.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gfwzibxjf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gqruvvzgo.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gbwczxywa.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gwcxdquce.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/ghexsqmfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gftjsttgl.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gygovwycw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/goiqmryjk.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gbhoobyfb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvcbbwjpv.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gqitnkoev.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gptaxhmek.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gczeubaje.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gbquqqjgr.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gmehwepdp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gnhqrhndp.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gcwzvovmw.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gwvnbsdig.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gprzyvsyc.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gkiqdarfa.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/ghmzyufld.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gqbanpiuy.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsgjkpgtd.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjkecyegg.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/goufjtwvq.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/ggaitjxod.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gnfsweuvg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gpgclcbjy.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gsturpbum.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gybcochkf.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gtvuevqjj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gcxwlvowi.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gbhvxjghy.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gzkhufwpc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/govkvdmwj.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gqvrkffis.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gcyhvdpgk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gfqljzgak.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmjsajocd.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gftfejset.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gtmfwkdvw.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gsypzltwx.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gxjaqjtki.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/grsvzztqe.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gzdjbsvri.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gnojgrtdx.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gltunrzid.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gqxpyyygy.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gcxfxsobl.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gmbvanhfa.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gyqwurmxo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkqyvrbi.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gosnjmsig.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gqzbpneec.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gwhdpljpq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbzpcrec.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/gacujihsu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gxbxdoblm.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gajltfppr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gaayhxjip.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvcdvtqvi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/guypsslpi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/ghqzrokyi.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxpkbgvmz.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gizzirkbv.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gbvrobbqs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/ghaachewi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gfztrhgxr.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/ghhimowpd.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqgqofqpb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/getjbsgrd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfspplgii.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmmdsnb.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gewnihnlt.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gzypokoei.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gyzjvwbdb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gqtsivyev.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gfbearehf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gnftdexot.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gxeuadbyn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gktxsbxmh.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gedvlsnlq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gzqiqvrqx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwyfqwvdb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gcnaifirt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grkzuxeqp.sHtML


<!-- 参考信息 -->