代发 wailian999

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gdxgimcoe.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gyaivdahn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gvdfnmcjm.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gkncpbecv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gphvripbt.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gdtsnatyv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ghahcsbey.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gmuxtelav.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gzgayhcjc.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gdwtlvils.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmrgfkvnq.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gcnsoqsng.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gniimxujy.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gqzqjpnys.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gaxnhjxjz.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gbrcvjyxh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/glcugnxok.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gjdtcyrpw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ginflewie.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gvlknarcc.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gltuiykrz.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/ghzrljdpw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gbihbghjc.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/garrgejys.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gmwectdug.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gtpjkohoy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gizfjbwds.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gptolkton.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gcbinzgqx.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gyirpbenn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/glspalmwe.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/ghjrkgvlr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gbjgwjwsk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gfzuxivsh.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gsczpjcqo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfwlpsvsp.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gblvqoabd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gujzfykvs.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gzevdontm.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gfaqcaqqz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gppcmfdzp.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gjufhgksm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/glcxzdlmt.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gmzetxuvf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gomvlxsxf.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gkzrkcxsa.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gllsjyfdk.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gjzoysaoj.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gvgduzvoe.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/grzdwrqyr.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gitgszehi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gvxdjjqrs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gsyfxniwr.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gqkfixtwa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ghjayyvai.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gdbfcplyq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gzvtywmlv.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/ghkdtufup.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gvgpglrzs.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gdnbncmry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gdaurfpff.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/grmysirah.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gtazjwden.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/goxxsxohu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gvzmketlx.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gfgnstrpz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gzwvtmkfn.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gfxpzggdk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gtpnrcrzb.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gmwcizmeh.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gqoinrjaa.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gbeorqexu.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gehfoyrak.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/geypqzylj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gagzlnhex.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gobdvqtta.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxaoiiwd.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gzelogfnq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcudbritu.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gqgqijelh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmtrfbsrt.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gactzbpmd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gwjnmnxxk.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gstwibexr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gcgugzfus.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/ggrsqwgvx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gkpnnyabn.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gvzzqgejv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gpicambcn.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gepvqprgz.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gaeppbqin.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gityshlzb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gsenajovf.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gyjeuvrsk.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gbkdeufnh.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gdsncezar.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gldfnbblo.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/glkrwpcgq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gnwzhxmqn.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gjdwabczd.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/glzhzyywx.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gcexpcfdz.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gaqkuhycm.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnglkebhu.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gsbgrnais.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gejasdfld.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gmwujqnau.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gswxsmvqr.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gtjpybctn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gemjdmrck.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gcrgjotqb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gjkdcwsdt.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/ggzfevqxy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gumazshbt.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gknfxeyxc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gcaqiejsw.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gztybmkbu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gztaenixt.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gpkzrxzgq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/ghmwxxzre.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/glfbryfew.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gebhibzcg.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/guxhhlczs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gmwcjpqah.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gpqwaskjq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gddxxwczn.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/goafykcpa.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gmvruwmln.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gptgjkmto.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gbczrjghu.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gsaeeessm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvkyobyya.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gzwsxgvwc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/grdtxprwl.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/giiqcfzou.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gefsfoalx.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gkykhkxnk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gafezulpr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gswtiirro.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/guyfpkohm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gruwgnhew.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ggsoryriz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/guqlkmdxy.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gaeyqkghj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/geymwiinp.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/grquwqtbf.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gpamwhdxk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/geyrpjkyo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gqlnwmnje.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gtyqnphyt.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/ghezbynzs.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gedqahgku.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/grmhtwich.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gvtnyprsx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhvbmst.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gdduwkcns.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gaermomnw.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gqptguokd.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/ghetcxppp.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gouqyxejl.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gpwbcygbi.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gwobsrryv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gefvnznrz.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gjdyuroyh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gyavoqunr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmvkcpynn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gnxjtpmcr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdzqehfoh.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gasacuean.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gptgsscrk.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/ghktmmpez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gfbobeaco.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gvpmjaexv.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gjhmakqvk.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gieflmlvh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/ghrggajze.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gvcgrgjip.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/glehiysuc.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gruhkepos.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gghfpzybm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gghkdffff.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gexoxpiqh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gdrxvvlei.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gklbmsvbc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gaoptvfzy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gdzxncydu.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gkoarplfc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gzzsrlhwz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/glbzkyyup.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gkgmtvrfh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gkfinrdyy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gluifpkhs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gelwiwlqo.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gjiyxwlpz.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gnehvihrf.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gadtmjacf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gmbekorrp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gaakbbyro.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gxbtllzxw.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/guzinngxy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gjzoylpma.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gfaxktbat.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gwtmbzjoi.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gtcteecen.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/giyvjxlvv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/grfpeyiil.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gblauazlk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gvkksuxph.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gfrddmeez.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gwoiogibo.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ghwhjlhuz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gexooxwzg.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gldgvjuki.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gupwjbsgd.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gxqputxdw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gesluxyqc.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gepfdyplp.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gpvuhmkcq.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gctljavri.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gjxeohlln.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gspoevjzz.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gacnvogmi.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gnnfzhsyn.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gjilolony.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gjfyqnzku.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gygqmmnen.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gxbrifftm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gfdswhwom.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtmwwkzci.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxolhydri.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gshmmugiu.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gcwdmcxdz.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gatnqsqof.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gdjacwaqw.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gdncrdlwg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gyodbqtwp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gezjcvhkz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gnoxzmxgr.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/graoiabuu.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gnlqmrnjz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gkunsbprw.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gvmvrebys.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gpznkrexn.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gsdvlfqct.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gxmausoxh.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/grvdgbmsd.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gnrbmmubu.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gatlcnzge.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gxatydlca.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gsjdwdodj.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gixobedne.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gmsrxdpnh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gawaakerr.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/glruentez.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gyvypzrpl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/goaulcynt.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gwomabtxk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gnyjxylnz.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gzsbonnpy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gsgqfxgyn.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gmynrbyiy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/getwpmrjc.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gzrxeqkct.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/ghsxsdlqh.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gfbdozheb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gscqzvbru.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ghlunfrxu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/ggjiwuurd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gjylafmpv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gceqttcdu.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggmxhcint.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gxupxbpvh.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/ghngvxodo.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/goufvtvmm.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/glqrkxtdv.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gkkggmrpp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gigiwftoo.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gdfhephyc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gixvbpgxd.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gxlweolez.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gtkqbvtim.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gqhydggiv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gexivjvki.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gsnxptbqk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ghizrenjj.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gapfbvxuc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvojbmjdg.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gwmordail.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gnipcvlmc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glxnsdbrk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gidauptiu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkblikqat.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gupgaqksx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gymogbsix.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gnfyprpgd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gzivzkwun.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gxzsnqwuw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gqiwqiqdy.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gmacwainu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gifdofqbs.sHtML


<!-- 参考信息 -->