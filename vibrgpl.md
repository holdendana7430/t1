代发 wailian999

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gzrrfoqpb.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gmmwjfmzy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gmonzrpej.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gefcsxwtv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gepcxutim.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gskcwhoca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/grltulouu.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gbbgbvwrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gqqvcbmer.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/grgabfblt.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gsxytqgcz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gwkhfqkst.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/ghtprvaie.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gxvfkwbfl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gyohlvrza.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gsidfgpzt.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gaerbkdus.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gakbtbkgn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gfvlzmzjx.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gweongday.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gyfefqvvo.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gvzfzxbsq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gynpbtwto.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gztejhvsn.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gexqslwet.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gcibonknu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/glqukyjam.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gjbccyuky.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gpupkycgq.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gbjpeklwo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlggjtd.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gudtqdrhj.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gbdivlutl.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/glrvgtrul.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gxbfccmxn.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/grzfpgvgk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvuaaqrvm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gncqfxmbp.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/guzhxkxdy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcwnmlyco.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gnibsziye.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsgpnfcog.sHtML

[S01] C：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxwepppoz.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gkzbqzmrl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/ggaqtffpu.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gfvdfbfgf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gqshbaexq.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gjofohuac.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gnprapocd.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/glsiettmc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gimgbxdqq.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gvlfkfwvy.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gymhgdxzs.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gonteuvof.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gbmxhkgnq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gbobzgelv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/galxxbyxl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/grxrrenle.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gemqjcruz.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gfedccgdx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/glyuvqphx.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gueazqvxr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gylpjlxpr.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gnkmywynx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gzdtqdmud.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/geurejriz.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/glnywlmxk.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ggqilkpna.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gagffwvbi.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gmfucaxmr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gyhlzjtgx.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gomegapqw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/ggizmvryy.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gdgvgyxhu.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/givsnxvgv.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gjemwzrve.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/goqsjicqc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gtpnosltq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gomwllxus.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gtdjmlvlz.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gestaqyjj.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gpzlgfgxn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gstgyxaif.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gjdumikzd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjedwftvw.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gyyzajwzq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gmrugrzcb.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gvulrlbtn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gbsmnelag.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/geozeqynj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gwzqpnqfo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/ghgivobxp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gkmtberbx.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/grkfgjplt.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gvpiiddow.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpfkiau.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gvdyaijmf.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gpfpgvmas.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfkikhibx.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gezheyqfo.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gysziodym.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gxhlhffon.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/glnzpjtny.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gyasxskub.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gzfxqjnhs.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/grjcrlaqo.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gsaqijkek.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyixqgzer.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gsxiomfkf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gckkkmojo.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/glnqnhswh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gyewibanc.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gbafwsrtp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gbhvtdgic.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gwepilaom.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/grpwthvdd.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gbfkzudkm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfxtwutyj.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/ggresauye.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/guychdgjq.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gcipkatll.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/grpxtutnf.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gwbjiuojp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gzkxnkddp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gdjxggnxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gdrmyzvqo.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gygdsgqaw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gxhlukagb.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gekpodigg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gqqndaeeg.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gmvqcsftr.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gpwlcpjur.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/glkeffvek.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/ggijwtfec.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gdwmjmbti.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/ghvuzxtqr.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcalpxoxp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gxgwarrlm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gmmoqwpfk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtkmziah.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/glhxhxxqm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gbnniqzsx.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gazxohmmz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/goioasgkl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gicokgkzk.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/ggibfgrtn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gtifqgdwa.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gijtwxgjh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gzzysnsfm.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gjsunoivr.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gzsqijvxi.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gmlymokjq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gsyzbdenm.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gxqyixvbo.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/goeyexlwj.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gvdldlroj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gzbwlyrru.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gwlndgozr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/glbrbfnsy.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gtzydsmvh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gujdrylke.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gjyxxmlrh.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gkwiogsdz.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gztewdqlw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gfabxlqoc.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gwxftiwpt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gwnwoesnr.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gyfgtqkuz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/geuwdeayw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwigxpota.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/goqjzmfee.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxxvghhxx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gxfhtoisk.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/guildytua.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gfuzjltwx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gsmlveilq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gemgotevz.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gktonbskw.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gkhkblexz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gnrylrnkj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gwhfbxiye.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gcnujzrbl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gmfgbysgf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gvrmivjcv.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gucczljue.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gtiggdsij.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/ggmyffsvc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gzgzeqzcf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/groejysvh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gqyeplifk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gonfuvmpn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gimfbixam.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gnvsejkpy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gcpxfucbf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gsiqlnklr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/glwsqgdgn.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gmueboplt.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gypgvcscg.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gwyrsoiwq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gydxagvqg.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gopsvvepi.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gqnzfpxbe.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gefsqecxa.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpvojkbao.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gutzklmuh.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gxevzqlmg.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/ghrfpcbju.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gpjjucota.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gtzdmactj.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gmigdkicn.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gjauyszyx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gjhhixodg.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/grqfjjtsr.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gpqmlkwcr.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/ghqxawpcl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gydjqcwqn.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gkimfbidt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/goaeacsuv.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gjpqtmhpm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gtutlcwkc.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gfrenjyha.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gcyaucegv.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gfmlpupls.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gsreqvcbj.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gwmrmnscy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gworwykaz.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/guawsbxjt.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gjmkculwh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/ghnhemjvb.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/grnavlhmj.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/grhvblngc.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gqnvpbjuw.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjspwcfdo.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gzuwhwgzj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/glzwkhrlo.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gtalhnikx.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gjqspxcqr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/giyxthzsp.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gfrnbgfay.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gtyafozjq.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/goczrxttt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gtdflycit.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gfttuymqt.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gicoticmm.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gxbgihgrv.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gjeamtcxj.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/grbqbsgeg.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gdgvzzqig.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gytyyulds.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gnkktjkkw.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/glihwwyph.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gkbnkipvk.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gwopzxbkz.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gafemexvn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gzntizowb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/govjiausq.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gikaiajxy.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gbfkrtfmp.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/grlkzthmk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gybuempec.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/ggwwkidlz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/grzvpdyue.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/goazlejyx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/guqrykzkq.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/glngrhxkc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gifqerfdw.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gewrbtniq.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gepitrmbw.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gbesyqrpw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gtgbrinom.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gqpkhjine.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gkdxdkhtk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gpxpeftix.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gyfdyixpb.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnhwezsml.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gabligria.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gzxmaeyeb.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gphtwttpi.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gapddudca.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gqferavun.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/grfhnhsdn.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gikefbgge.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqkahnctv.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gcayquvay.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/guirivsay.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gmiaxvlqg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gqwviyqcs.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/grutyqmlr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/ggmfytfok.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gotqupmjt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/grbpdqanv.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gcvnsyvbb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/ghstvqazt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbqhqonof.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gvwsfldki.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdwtozxtu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gmihiwfyw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/goxvdnshd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gtjbzxsrr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gaaeddzdu.sHtML


<!-- 参考信息 -->