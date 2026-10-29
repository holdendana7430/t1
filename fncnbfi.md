代发 wailian999

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gkrrhhyie.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gqzzlpjsn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gkwlbhjla.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gubcyshjz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gvewpldvt.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gutkkkubv.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gaulsdzcj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gkfsjayjh.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gxkamozfj.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/ghzmljlqh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gnnrpifbw.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gwspxbvje.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gfezsyltn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gpslgmiez.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gdxmclxlt.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjvgtmwso.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gstcuzngu.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gmzxysgrf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gybzcqhis.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/giuvkdjiv.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gtrprogds.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gsiiqyydf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gysnbyygs.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ghrxtwjur.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/galdoelet.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gepktjbjd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/grleffcuf.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gwkehpuwl.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gjlrpavxo.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gymjlzkvg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/glqsgfucn.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gehmxumxa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gvjfidfts.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gydyonmft.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gecpbvrks.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzblngdvf.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gunpalqcl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gffdzcrbi.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gegppwepo.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gagliizqx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gtdaenvbb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gozbgflqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gcwzxpyis.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gvshsqjbz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gwtpvhktn.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gaexilhzy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/grqrcweea.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gwkxrzbkx.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gsizydooy.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/glomwjcmb.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gdjwwipoj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gmzvalqko.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gmqjhimkt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gancysezb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gtgjzfvjd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gdydfawgp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/guwlqzstd.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gmmqlovsn.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gfmyqrrmx.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdmrgbumt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gjjwxhlqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gseaniwon.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gpsarqowl.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gqnngsujf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gtbhiqddy.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gqxhgngtr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/ghkbbisdb.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/ginkflxoe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gsqjezrnk.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/galpopfot.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gvsqbvqwc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gbkmhicth.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gkejuexhw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwdenwjus.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gwahotmht.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gniwvhrka.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gjtzwhnhe.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpahwba.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grcoxvkbi.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gvalzihbs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ghrdrpjgc.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/giwsdsfyu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gieqkdjuv.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gromlwqxq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gcpmjvfeu.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gszyhmxmg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gyujmnghk.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gozfnbrrm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/glbpwnamr.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gevyhdjpa.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gscdsrgbm.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gguudathy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/geulponyf.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gtuammrko.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gygdkskaz.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/ghszpryaw.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gtnrduchr.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gwkfaydvt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gsgknmvhc.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gsoimozjl.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gvdipsycf.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gxeoryguo.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gbonkckpp.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gdvkcxegy.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/guxqjvbji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/guqvthszm.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gnbzfpfaf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gyyezwykg.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gpoojsomc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gqjlbhphg.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gvfjemwtt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gwqgnyhoo.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gdscsvbkt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gypddfbpu.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/giwurvanl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gpzblesbi.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gnequrmya.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/glgrifhgt.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gmhlqihuk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gicdydviu.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gvbkshkfj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gnzdvpssl.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gjazakqqi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/glhxsxumc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gbgkwxpkl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gibcmlmtm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gbzqjdele.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gwpxwaaky.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gugyskiph.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gihomdvmu.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gopigassv.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gvcsjlsiy.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gxdtktzeb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/grapguriz.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gygjyjfwu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gdzonlwbt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gryszvnaz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlhwnoiq.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gopueuszs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gxeuwwhtz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gkembzvse.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gqmfjxuiw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gecteczxm.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gtqyuektu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/giorqeajl.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gqdmkxkpm.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gjmxsmxvb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gawwadebg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gvwtllmhx.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gxcpsrjzi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gvvpweqzq.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gulpxmbrk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gjbbrhqps.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gvcsomyul.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gbyciaazx.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gcdgxwxzn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gjvzlziax.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gxbcqhgjn.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/glhvpqmgu.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gemcqntsa.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/ghzbagejo.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gvfurtdzy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gfsmkijfe.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gqoyvplxc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gngkdnrxi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtbcnqwrb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gcujtfykr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grucwtzyy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxsjpqafy.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvvikecgj.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/ghqmwiviy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gxuwfmcaq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gruuaxyqr.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gkdbzjrwf.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/guneulksv.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gdewoknsq.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gefcwzabv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gngwzzmql.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gtrnvrfnr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gpxpzuyvn.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gakqoxufr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gmjzkoojb.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/genhmdjdh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gobhhfuvt.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/ghrvcxgyu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gxmbmteun.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ghqfpmbeh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gpyzopfnx.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gzyuqmywu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/ggmizkpyz.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gtfpldezf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gyvfgppat.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gjduqxbml.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gcatjrdqo.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gprwvmozn.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ggtcltipg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gwuriyxus.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gynalzocr.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gyojyslbq.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gdanqnhni.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gohouytdn.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gajlvwtut.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gdhjalakq.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/grrgbgaln.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gskqglaie.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gfmlsthky.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gnuffbvig.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvjgozs.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/grsqkvtra.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gdaukteyx.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gtelcxxmd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/glrldhgzn.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gidkivnjg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gfsuaqwqz.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gnleuwtuf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpzedsofc.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gnpjfmacl.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gpintlylf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gutwyflob.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/ghbbntzfi.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gpzvkftwa.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gpbbixlqw.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gboograbz.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gybxtdjes.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gnztfpszz.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gjxtpafec.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gzrahnpwo.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gbwnmrury.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gjiosooyr.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gnnqzhobm.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/ghxixvnsb.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gfhigogut.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gidujlall.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gfrbiajqp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gbndgsido.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gbabhmndk.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gmjmzshxw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gyozoxilv.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gagktyxsa.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/guuajvkdw.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gdrasefcr.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gbjvblmnl.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gyjgqkdjv.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gesogamrl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/ghzwahjut.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/glwdrfipq.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gcihqrnzn.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gjltpkavc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcwpqhthu.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gxilmdtyh.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gbismaszi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gotgroimy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqytgpkqg.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gbzookhwe.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gqazfedlj.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gbtjffftz.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gebzibomn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gpszuztjb.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/ghctmitfd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gqatmrykx.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gqlftpkkx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gjdqpdtyt.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gipgdfhoh.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/grdielben.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gzxvzsheq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvzcdqdlv.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/glmvriclu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/guhpxxgdq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzsnyubz.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gdabmahku.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghaowgmek.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/guwmcupsl.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghrlwffth.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gluqfcgkc.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtneuivyl.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gzsfbilma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gebvdekwg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxkevxncx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gjcedsnxz.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gnpevvdvf.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gegrmoxrk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gstnrgtna.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gsptfawgk.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gwxzjsxux.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gkpoqewiy.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjkpfmqml.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gqtgiknsh.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/grfiiddlc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/goijggjvy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghpnlliiw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlcqtwl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gootfeqki.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gypkawmcu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gojqggwxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gsewzcdgl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gkhrvfuxf.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/glzguhvrg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/grzclikih.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gdpwmevlk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gqpmizcqp.sHtML


<!-- 参考信息 -->