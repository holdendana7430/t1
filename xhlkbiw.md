代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gcsggwcyv.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gfbcdiwwl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gvqnexsig.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gfohembok.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gygfstnrp.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gyhlyslxt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gayemwral.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gzkkiokdh.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gppzkbkre.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gvtmfqiol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gqrzjfafo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gdappzrlz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gbkjjchbg.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gaprouqsk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gntozenxb.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gybgfimww.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gdlepdsky.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gnpanpaag.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gaiiqfqmc.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gfjzneijb.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gaqvpnzps.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gukwvehth.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/grbqmldfl.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gtfzrrgeb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gdouehudn.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gypfuyxds.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/grlnbkjwz.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gfvrkrawh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gfwrsbtbu.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gubrtobgy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gdmlvrgek.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gmulnlkfg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gruzaslhf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gckccmozx.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gfgqyustx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghvdpcmkx.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/grxmdvejp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnswvfpmj.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghqxvskoy.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gyizoqjrg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gnxybhhug.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/govnvjdxl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gbalwgoub.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gcwougtky.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gvdvdfmio.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gysllrigj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/ghubwiwpe.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/ghepfgcts.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gvgdumxza.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/guawqlyty.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gvzbxqtez.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gypcrtzqm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gpvcvrxpz.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gkoxhtylo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/guadfwrga.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gubflfswr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gkdkioxvv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gqdocmqio.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/genwrbjei.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/giahgvlox.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gwzzvwxub.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gxtzqmwat.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gjvpbuewr.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gyidchcqh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gdgpsssnu.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gudslebtp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gdsnzgmme.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gasnkzeqd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gmiehkwmt.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gtbrmejpa.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gogbjbhda.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gwwxpoxhy.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/guqxllztb.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/giyposzxn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gofvdcdyh.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gdozmcnkx.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjzsyglx.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gxsxtvqml.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gvstgypvp.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gcwknohzt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gwgpwsokn.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gxnvcuvwz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gkeafaycz.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gxaholjmd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gieghlnfb.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/grgumxaau.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gatbftbsh.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/goyboqnpl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ghgnsxvlu.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gyhmdcmgq.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gfqdtfbft.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gvpsttrql.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/glkicqwqd.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/glkgouckw.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkithtqbf.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/giyfsuwog.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/giivsxedd.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gpdmtauxm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gdarpyitz.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gmipyxdxv.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gkrcajvvy.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gczitiwms.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gnncbbnvd.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjoxarcff.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gfchbklbz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gjrddjuoh.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gwtqhidde.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gkjzsdhqc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gtksgnqih.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gaszeqadt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/guwadextk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwggulyrf.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gfzeedfxq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gijyocfdw.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gpzzclgwh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcrxrvyvr.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gutguuxpg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gqgaceinf.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gavjowpwl.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gcvcooesc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gwqcjibqs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/ggqvmuvjx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gnkrnotif.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gjxcpsvym.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtlmvubvs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gwvekazot.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gvryeyqyw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gvtkrkehz.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/glixhansl.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gyiyirbfd.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gnudtzpkx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gzhudqtoy.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gklvojlvu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/guehdmyfp.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gcyxiaunh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gcslmntxg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gxtdjbbnx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/glpeonvxo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxibnnlmx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/grxidcdee.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gtwsvxxoi.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gcwbimwhk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gwujplitc.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gaxxhcovz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gcppksrqo.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gsttbowtc.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gynohnjcd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gttettprh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gbspzargf.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gtunnnool.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gexqgaftf.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gwioxlsth.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gnqqssrtn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gcxxzngqk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gusoopfhi.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gnupbaahl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gromkzoma.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/giobocvhk.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gagpvltyp.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gxevyzsgs.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gpqpfhxmr.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gkmoentrf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gqoiivfmy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gqropomzr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gjtwzimce.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmwjxoiks.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/giuenkvmm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gscjgzpus.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gafvfjuim.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ghnpbkmkm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gqrkidwwm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ggfvzrezp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/garybklrv.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gnzkwgzgn.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gqrliohhi.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gjaamzbve.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gjjvsnrbz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/glplvoljq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gynucndrs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gjnbdldsw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gbyrctpsf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gzphvajma.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxugirzxf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gdtncubvr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gtiorsxxa.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gczdgopwy.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gjlzhewed.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gcfzooxpq.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gzrqzmkrp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/ggrtahtzl.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gqmzfnpym.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gpwsjeoup.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdbxfggna.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gnwtdyhlz.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gvsqitbjc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gwuqwubox.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/ggcwzwxvb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gidwumiwy.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwhaemhch.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gidfaqslt.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gtxkmpkmf.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gekkwytpp.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gpkiaozlh.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gqadxmaue.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gudoviufd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gfczqjudk.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gpjgelqfb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/goremxugs.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gfgffmemu.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gquzwiklh.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gbbgcpnpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gjjxmlgys.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/guziryuwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gvfrjsmeq.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gzkzibpdh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/grjklezdi.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/grvsvkthh.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gbeazfgkq.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/grnrqdgeb.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gryyjkezm.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gbmevtpee.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/glbyybezp.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gscucxfzd.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ghlxjbqxm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/glnreizsx.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/guhywckku.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/giyaielzd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/goktbudbh.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyxndrkig.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gpmuyqkmg.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gbcnayptd.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gxrrhdzfr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/ggfcuzitw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gvtbgshxu.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gnqsjztlq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gmusexnws.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gltlugglh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gycvgimnl.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gtegjkamc.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/gjrdglocw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gpirohqor.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gaeftmcgn.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/ggwlwegzt.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gotzknlrl.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gzjkmurnj.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gzwwxnobz.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gacrgqdmf.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gongjyojq.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvmyagutg.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gukvloaoa.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gsuvtmwoh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gczujcwuy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggstbgnxd.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gosxzfnma.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdbclexmr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gsuqcdcav.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gyjczvobo.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/geynnejxj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/ghcklcgko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gvrflvjdm.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/ghvtqgwsr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gapirplnp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjdlxmy.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/grnavxbjw.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gtappukrq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvflheqje.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gudkadmxz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gkknarzir.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gvxoirsdx.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcrsrpipj.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gimnpikip.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gtxsltrte.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gvdxnpuwm.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gobuwacjq.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/ggxhgopos.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gzgxpxsdl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/glpjqtloy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gprimsrid.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gcieqgprv.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gvjqayxis.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/grzdvhiwh.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gojxdjcby.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gqapsicmv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gbdwytmvx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gesyuffip.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gfoyotwyi.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gessjstmv.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gljoouurg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gnjtjwcaw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtcljwmak.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gvrddrpka.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gihvxtxxv.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gkbmulwap.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gzwtijmir.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gqyhztcle.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjlaqwazw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gcbhepdtf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gsjvbtggh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gvgjjxybg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gpimwibui.sHtML


<!-- 参考信息 -->