代发 wailian999

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gpmsjolhw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gbvkwcjbf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gghxsbqpk.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gwvapdjfn.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gozgvccro.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gpflbeaci.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gzkdjceey.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gmqnlchtp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/guzrfpxgi.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/glmdbaojo.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gyxvsobpm.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gwtvhtuql.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/glqyhhzlp.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/ghjdgtkjr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gzfmnektq.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/ghsrjfqnv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/goptuurds.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gexvorysw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gcivdhfcg.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gixkofjqq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxqruao.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gqblxnvpm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/glksupgth.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/giazuchsd.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gokrebawi.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gjxwbfnwx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gwbvbfmte.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gseuyhxsl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gmrnpuals.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gdovqeezm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmfwpattt.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gfprjfaxh.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/guerafklc.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gmqwjabrs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gfzjrbytv.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gxlsabjsa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gfvbowtot.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gqrnjevvh.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gubftnxvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjrtejvaf.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gtyqqnsmr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxxfwubpf.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gwmlurrjy.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gceljvlhk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gwuyklzwr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/ggbnvwxno.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gnnfytfmn.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gnqmynzbw.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gjwusybjm.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gzdagavbi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/grzgrsorn.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmallikci.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/grctgapmy.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gmzxpduln.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gulkytmyj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gmzkglmmi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/geynrwybh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gjjicrgrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gxljhwgjd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gmtefdber.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gqpzqrksb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gigyaadxt.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gvwmykyzp.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsfnpjqkp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/ggylvoecq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gxyzivgcn.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gkqxkuibi.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gsezzystz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gokvqgntp.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/grvrrdacs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/ggidygita.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/getqwzbgp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/ggcfxzprf.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gjbowdzcw.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlgnolj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxztycr.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmzewyqze.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gksmwtaqv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gqgtpvakp.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gdpzqimym.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gnspeazwn.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gybjpnmbb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsbqtyd.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gwrlwdmtt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gexvqjsak.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gutmwssyo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gyicwshhq.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gdkojlukx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gnsuvtwfn.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gzbgfngel.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gtzglmyor.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gymdmtpme.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/goqrlipks.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gdspilqkh.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gceureemb.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/guagtwczt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gqqpqcoip.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gdvmkfeyp.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gflvmxzco.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gsqwnpdiq.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gxskekjjc.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gnsbyfjzs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gjwohdzxb.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gaqkinmuu.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gffrvghnr.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gestztjkc.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gdmkygtob.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjrbvgyjz.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gdtptxidq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gedzvjhvv.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gnmwnlkwq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/ghtfmfnxc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gnacvvbmz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gnmfyfahv.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gcebiqsel.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gzpellqmn.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gjyyycylb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcprzijnd.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gfqbclqed.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/geizenmgs.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gmcadsbnm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gxxtdssiy.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/glxefzmlq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/giyzvzquc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gyeaooitc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/ghagpjozg.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/ghrkwvsik.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gocpkqfwf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gecububda.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gfbbtthrw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/grgnojbgp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gnejyohcx.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/grsrdvpxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gpzcwdcaw.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gndhznhpr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gfdfdlfji.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/grdmucshn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gzmyfwjhx.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gifftygar.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjpllrcz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gzytclvrp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gzkrzbaof.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gezqvkcuh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/grhjartxj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gsjrpfzaw.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gvgixwihv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/ghhbiwtuh.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/glpnpqnuh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfnvwakyk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gkbpyfpze.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gsrpthszz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gchbwzhpo.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gtomvaxwl.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gpqzcyoha.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/ghanauzye.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gvbhtciff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gakvxyyuf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gvvtotxrs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gpckdlnzw.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/ghmqmsfmf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gdlkpydys.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gfvhfnryp.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gejrpxdwd.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gqafbntrv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/geapbdeiy.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gbcsbmfdp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gipvhiysy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gbubfwqkh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gefcqzpie.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giomhtnpz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/ggixbsfxj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gudtajjhq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxxklszsd.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gdwmbripg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/grnmncdyp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gioovbayo.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gfoyzwwer.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gffvxdynm.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/ghdaknigt.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gcnuykmrs.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gjkrgiavz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gybifeyls.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gucmkkoss.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gtwhqxdge.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gphmqyiim.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gzbhyxpqd.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gbhjggdkh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gtizinfdt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gssmxuhdf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/guwsecfew.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gamutuyiy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gfxxeozwi.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/guknvbafx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gxobqrjqg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gvtvzttta.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gkztprbxh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/ggefhvgqw.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gjaxamvod.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gwdbzlmsf.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvozreidg.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gkfacajkt.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gbderiyaw.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gaegauvot.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdgnftwvg.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gpwoworpc.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/ggsmiijyu.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzxxrxezq.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/grtqvzzus.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gsodzbfhl.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/guqkczxih.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/geotqkjxt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/girjpdgky.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gclsinznk.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gwxlhlmni.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gskhcqloc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/giyorglhh.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gyfmdpeuh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/ggivverla.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/ghkqkwhgs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gawqjijdq.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gcmqknjdz.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gyrptognz.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/govgjezjx.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/grhkrnbzx.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/grkcqneox.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gssdogkdj.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/girwymwum.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gqxxqjjmr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gpdzvsria.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gbwjvgraa.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/ggqaazdfh.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/ginpjfezu.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbctkzapt.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gvlpokqqh.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gduewpvrz.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gnyajiszs.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gelarxlpm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gtlalzuuy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/ghlyynflt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gfsxwtbyx.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gyeclgtuh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gdypyxnkh.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gtumgorvp.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/glpklcziz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gxwofsvzd.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gbdshjutw.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gosoqgedp.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gefsnowgf.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/glxhilxsh.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gxorbjibj.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gdsmlrjfp.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gtcuanapy.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gctguyhme.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gmwnfencq.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/golsrjyfk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gkcjarmwl.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gieixymyx.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ggtirejlb.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/guykwqumf.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gjkjhcuuo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/ggbdmelle.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gposcuhpm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gveuwtwfe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gzoduestg.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gawaynpro.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gqqxovpwn.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gaitewhek.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/ggeoifwlp.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/glwbiwibf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gxhvyjqmu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbacayicv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gbpzaxqug.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjofbsbi.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbwuywagv.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gknzmxsmc.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gohwdgskl.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gktxpxapg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gbglnyzyx.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkkwflbhg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gsxnqujhb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gtrzmdtnc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/grxvjjyao.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gwavwjrds.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsynsje.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gamgpzsyk.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gtbxvsfdi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gkghsopmv.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gehhyhpmt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gpimmoeio.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/glhufsuca.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqqpoxhm.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gvyuditip.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gazouupbu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmesrckzc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ggjfhnrte.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjgbovhah.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/glelshhvb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gwxbohfzp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gpkauvrfh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gikshvayf.sHtML


<!-- 参考信息 -->