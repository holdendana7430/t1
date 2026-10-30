代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gkjhvktox.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/glwnpqbba.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtqxelem.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gesrzlmwt.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gylixfeup.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gvoqjjakt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggpjiybrt.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbtgzjzj.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqvwundo.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfsvcbmk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjwekrbi.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqozmfyn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdeamnxv.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gfmqtalhj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpasrmdmp.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhjwqxk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gjalfzrox.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/golnhknii.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyghzpdy.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gumabnbci.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gksqgwyfp.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsazhecz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnllizivo.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gqdzkibuo.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gndcxkjlv.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gachdjzbh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/givgapluo.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/glyzupnwc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnkrztuv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjryprkj.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gvxlcgzdg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggajlffgr.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgqifjie.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaevkjqvy.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtunarcpg.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkzuahlg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsoojqla.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gnvcxqedu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrehoibx.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gexuhemvl.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpnmxxbd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gtbdqxqsl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gwklxkbfn.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkhhtdawb.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gxfgvgyev.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkviqptrj.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gjipnzdvd.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gakgvacqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gclgfxnkv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoovwrqp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/grnyuiwaq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmzbyyve.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzztservn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwuunqik.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/grslkzrnh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goakkscho.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gfayolysh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmngtderd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gafxoauwz.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeunvfxb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkypsobge.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbctpnqkp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkhzdxfp.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxmpfzwy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gmlzldomm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylziqwml.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqlnbjjou.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxytqocfy.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gbkcmbjvx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuizvtve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gzhpcpjqw.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzaysiiwz.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxnjnjqm.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gcccmvqvy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gymqwbpmg.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grsjpvxzh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gigluuhbl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtmdetsw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/guvltctto.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ghozwwhxs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyhjvbni.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyjmdrdm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbiqvcvz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gedxsxcnx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymquklvq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gzttuvpgs.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxrtdqub.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gpjofovjv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gddxykyfl.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/guqrfqdds.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grsuaobyy.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaksqofie.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gfosgzuva.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gboiuhzck.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/geoijftgi.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gjsrqwrmt.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdiroezh.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gmksiwxxp.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gmqfomlzg.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjnsfovbh.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gcesfcsmh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gewacdfhd.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/ghugulpan.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geahobjnx.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gwggzqhpd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/galfexamw.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gdwgbvaex.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzpxgslt.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhszgrd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcllysam.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjothoko.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsivycm.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmmolxyb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnadkgrgh.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxoexrzu.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gntpkmeoa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxhsrzci.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gecliwrno.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaezjbud.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxekeggvk.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmliksfgg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcnxcczx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzmgecteq.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxskjmrea.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gibsvdrfd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmpdvpvc.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gaghswvxv.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzugdagpl.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/geojgvdlw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/girmgrnfy.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gocpcjdzk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmfselan.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gajgofksx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurpagxos.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdxarimp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gfdttvwwq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/ggdobcsij.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfvwshtq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqdxznxx.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyqycoij.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/golktasck.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnrzgemtq.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/guaqfxsuf.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/grsflgszu.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyudqzlre.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqtxhjr.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gmabplrut.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gfppqmthg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrqcqjpp.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gxrooxmgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdturlmy.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/ghlpecaro.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghljpkoms.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnajaszg.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbtfaocq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjggptjml.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gfjzfvugu.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gpblvgnwb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzszidhla.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gipwpvatp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwexppcll.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrnkbetr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gnnnegrxe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggsuzbgis.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnzjlbhju.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblwaowhp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvrgxdvr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/giugdmrbd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqngifxdx.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galfiboez.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gwlwlgbce.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzlsymuk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyzsfixi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/goywfqlod.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gymdjaydg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjcoredlg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehpfntm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpzukrq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojfacqz.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrohwvzw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gckbncwgy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqqqnxi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceesutaj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gucjlokhi.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtrymwtw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gkgymlxpm.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdeuvdu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjgbfyrw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxpaviha.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbckvcvzm.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfvdoxeh.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcldsura.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdkafxff.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgrlmhyx.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gugfkzojv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmtglgmes.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqlegdjs.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuxhxbgg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzudwjxs.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghulzdnii.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzynzyhd.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grqbvhybv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygibjqwa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhqhczld.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmibrtvsk.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpatjwwda.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grducuclk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/glmfcrrqh.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjhhggnkb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwfdzhdu.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gexavnnts.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gpekvkuyn.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuwrenmi.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeeaiyxo.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gntzngqtw.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnhewjrr.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzbvywww.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcidgqxi.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlfikhml.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gbixfruwi.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmovpjg.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gtksoursy.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gurpaougd.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gkbyguexv.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjenabvy.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkjacrpd.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtvytnoai.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjnfrxun.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvslfvtz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkxkjwre.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlozdqsb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gniimpcqo.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gqgxjtwtw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcpxzhjo.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvdvkmqbd.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaxqmuns.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gylhmxtcj.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxozsgwy.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagtcotge.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/grvpkyxrh.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geomsynnl.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gknatnfdp.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbwfnbbu.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizvhegsh.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpvpxhtyx.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpwhovmt.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gsaanfzak.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkiuevjv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/guhxubxso.sHtML

"值: $a"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwessmkkm.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbtmtgufs.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvqyceeqx.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfalozxzz.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcytgclys.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgmoflhj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhsodxla.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/gvhvgxvax.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctyamwij.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkpqhhch.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/goyqdgbmz.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gfqoztdyc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsplfetjx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnnzfhfzq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gngjqxtut.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozqzeaqi.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkkgrdgra.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmeocray.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdnxgzfox.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbptsrvhi.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/giibrqvoj.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjigvomg.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gmtjlrmxl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmzfdzcj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gghtypymk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gaylpnzbz.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gzveojuzb.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/glnbvnexi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/goabdgwsi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhbfnyds.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghzuxznpt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnrnggph.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gyoayjqlc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgyjledu.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gslbywqqb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/ggcojsqup.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzcguuhe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/guzjcxlwd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqmmimjgr.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbufjjeg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gjapvugxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvflyohq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gonvqktos.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/grxljljae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpavoixe.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glktxgcal.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfjrrksc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozgibshz.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gftaaixlf.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gppusoqaz.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gpwfpxdkb.sHtML


<!-- 参考信息 -->