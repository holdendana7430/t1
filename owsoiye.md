代发 wailian999

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gjziqcsii.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/goblekdrv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gbncziisb.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/grajnwvro.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gqkffqmwr.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbpabpqzk.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gnxaydefw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gwrmsbqya.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/grnzwejqs.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/guoszjtoe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gmhgunqhp.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/ggqfgqlkp.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gmfxhsctl.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gitmmuxui.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gmqohtgfp.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ggajdhckm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gmfuvmysv.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gveyagfry.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghtvxbsmw.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gvfvxyyzr.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gtrxgdcbm.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gowgpldmt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gbjbbvhpw.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gxttjnaxp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gshtokgps.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gdvtehynq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gtvxofffh.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gjifokazz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/ghaxpkdug.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/grnzcodqr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gzyxvgklo.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/grtjqhnid.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gwidctcud.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gexhbsxhl.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gccgcmkcl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guqycvgyu.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gdvureofc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geoxewrhk.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gooeigsam.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/ganldyret.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gpgahmjtn.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/glogbpykv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gyuvvvomr.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gewgusytd.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gulkqitdn.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/glnjabbvs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/glwbcckto.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gvbnkqktc.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gffumixhn.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gziwrpjxd.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gzztvhchj.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gjotdcruo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gyuwdureq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gwdmcbdfm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gpqrxszrn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gzszrulrn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gphvpneff.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gwcyamubf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gfbdqztlh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gyjurhvkq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gcmuhtjpb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gjdysrhfk.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gkdpknezs.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gdlanbymy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdmurvxs.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/ggjhniboy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gdcdutmbt.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gryewixfq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gjmcvehtj.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gmzxzulpi.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/ghewkfmhx.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gccyguwgz.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/geknfetpc.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gghnymkwb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gyslqvpzq.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gzxhrxwol.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/ggabhvxyf.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/glqxccjup.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/govzaiekt.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gjmawgjsv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gvpifuhwd.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gkdrhbgfs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gebnznfvo.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gyggcgxue.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gjdclpckk.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gutjsebob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/glcohinpa.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gmaovxbeg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/grrihqamt.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gwcyigqlw.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gyaqmsfis.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gkvtzzaoo.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gjadulric.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gvicdjtgs.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gnovfvqdy.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gjcfitmbw.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gaogwcjkz.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gyhiclcsu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gfawwwfpl.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ghznqcjkr.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gkdzkuykw.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gforvzmjv.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gcxfrbahr.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glawrobbp.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gpmkevzrf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gcarmpeae.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/ghbyypkjx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gvuoxbhwm.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gvucenaql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gemfibebm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gxmerexjd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gwcryvrod.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gkzconwux.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggtjcttyv.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gauzzgiqd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gvjfrjaxo.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gmhsnmlxp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gtmfhlxwz.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gfjszxmtm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gndukxckp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gqvpauzvj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gkymwjrwa.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/ggwxbqjcq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gtppwpaej.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gughbqrhp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gnaegkmfn.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gauvcxvtw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gzvrywenr.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gsooehfqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gbhykjgbe.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gzdaomjdt.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gqubyylzz.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gcdrglwlo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjaztzpme.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gpvjklaxi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/guqhwiade.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxccapgfq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gdqvbemap.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmvhidgcc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gqsejhonm.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/ggafodwwr.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gjwaiflao.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gbfcogrpv.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/goanloctl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjeiflgqw.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gdslohvzg.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gkzkrhdvu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/glqixmjhw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/glryfesvj.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gdvtwnmlq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gddudiftg.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gwudsnfha.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gheirfvnr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gbnyaobbl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/giwtwacgi.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gpsulyszl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtuucen.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gxjbxmbsr.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/gbxltylkk.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gxrpdaqqg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gqytsjnpa.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gxoruscvz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/ggyrfjzzw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gzkvwnvof.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gwhhpeetz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqtulkugv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gzyibauwk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghawrkghe.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsykdppgl.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyaadjbvd.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gzpvhoabj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gslwbrnyc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/geyclvagw.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gekpfjjhv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gblrbudpa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gcncilqmb.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/grhmqiktn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gmusdwutr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gxdycerkw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbtbqpmyi.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gawzdjxqo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ggjggnojf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gostkaulh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gijmtxred.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gjdxggqrw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gfpdqyeuy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/guqgmqtxr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gqbxtnbji.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gekzaixex.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gigixqmgc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gqgglshyn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gnqqgmbqx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/giwnmofqz.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwiwztqmk.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gvmsqceea.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gnqdhdazp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gdcjfagml.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gsexptysj.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gdazsxong.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/guyfioonk.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gqckfuxep.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvkyfzieg.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gmprdpijq.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gdwepvgbf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gvjmnacej.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gexwdqssp.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gbczgnxfj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gjyuohquv.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gkicjtics.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gjvcaaftl.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gtgwndszp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gccanmsaq.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gzuieedyk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gsveoycop.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gtwikclyn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/getxiqpcg.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gmhfofqqb.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/grpelwkya.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/ggiotdibj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gdduihmhg.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gcrijmtxa.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gcyjhkgqj.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/grwsdepkz.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gbburclvb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gbnkgnqmf.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gzlrmdokc.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gqrmeecvk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gufzzekzm.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxsblhlql.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gdedpvkey.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gqpnbualg.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gmtqnbntk.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gkdhwgonc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gjiejcoty.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gbbnxxweq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gkkcpunwl.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gsgcxpkio.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gvaehlfyv.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gagynbojw.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gsbvivpon.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjrbhkl.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gluqmoeyt.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gpgjlbcnt.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/geawbjpod.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gwbeoxznq.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gckppdriu.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gfbxiikkd.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gvswwzqca.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gakloisuf.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gsgbsemer.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdchauwqv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/genxnihic.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gpfdhobsc.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gdouojvdh.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gggfjcdgt.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gztjnzsgo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxyssbnqf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtwypceq.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gqsdratil.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gmmqnqrrl.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/girhslros.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gyanjevkh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gfynawnkl.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gggtfifuw.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gexzxhdyn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gkospkrtx.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gbfppdhws.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gafizffnj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gdgefjoco.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/grxqvoboo.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gdkufmtxw.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gjorfdaqw.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/geqcghabl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ggtresehf.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/glwbletht.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/giyftszcb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/grbeyydup.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gsoktaffk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfabwskkk.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gpukpiqnj.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gofcxoeip.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gstsprdjk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gawcrfywa.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gmatjippt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gxmxobshx.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gaslhavdg.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gchrjszoh.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gatiejbxr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gjkottdjo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkzrrkruv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gklmefprq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grtcdlyou.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/glnmfogwz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gqxyixrhz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gletzepxh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/goudqprnn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gtgydvmny.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gvxxwbiat.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gofwgczsb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gqwlggueu.sHtML


<!-- 参考信息 -->