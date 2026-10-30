代发 wailian999

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrgvifun.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbuiuczn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgevorif.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gwthwwxzt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gyugfgakw.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gasbcbrar.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfthliael.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaylugduw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gwatisavn.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtrbwufa.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtudziavy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gsclxlwaq.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/giarhyxvq.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/grsoucusp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnahdmqln.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gspppkpbm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbcnwipy.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggrlsgbpv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gxssvdrpn.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/guveduqpe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhtpuriw.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gpmghzoxp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/glpqwwbay.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gsziiosmb.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnwvjjjg.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvpmigix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqevevnud.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glwvljofl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gzizenxps.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsbtcyel.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gtvrntzin.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjrttkws.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gypnbxnqv.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfsoblub.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzjooivz.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gzicyyjdh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/goxnenxzc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gylbqjmhi.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/guktwwvmn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdtjvclz.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gveaemqkc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gujjpafxw.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhzplbnt.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gyvqxmnfn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoaseyuv.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gsulgmdxg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/glamehwoc.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/glqkbqkje.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/grdqnpnlw.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkxjubkx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gamhsouol.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnktmamez.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkggxmazc.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/glaqkrbxt.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwvfknqkg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqtaqtkh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gqokzpzbi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gjcaapsui.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjftulxh.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gkjieybvk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gqateudbw.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqhplemk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxedpxcf.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdaewjaqr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaercbwxk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/guwtrodoj.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdwhzbndg.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gevtnnksd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlmpkyiy.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjnufraz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjfeyrgk.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gthwiprro.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcnijajg.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwwohcbqq.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqsvxuh.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gznshwyos.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjmclhuq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksptbifs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcxldaur.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gseemewsw.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgsdgkv.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gprulncyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzqtrdmwp.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwwvmwjfg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbumyrqeq.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gpdjnedmc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gkluboggf.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gaewtmmls.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmupptmyf.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/ghjyjecna.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrveavly.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvlydny.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gchxkjonb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykdtqrvh.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gfduibfjr.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnrdertn.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gmurxvcyj.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gemnflhug.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtqptnwo.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjlnehsu.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gxsgjaluj.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtjglelu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlhtzggv.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/glntsbbzz.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnccqbxjj.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gboeuhhcg.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gmimiceta.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gytklyqxt.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxikgzhg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gorpjjhcg.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gpkhvxcvf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizjlhhcj.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gqqqixtvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwmzfcip.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/ghexwahsk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmufnhky.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofltctzq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwuyaffru.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdgzqro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexcvnzoy.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpnyzqqs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqttjiwzo.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggedwodql.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/grwmumsgx.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdmbpbkg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gidzlejjl.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwnkepnb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gusuoolnu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzzmrfpl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiqacgky.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkfpkyrk.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gfpvpewmd.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gveykfwau.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gkpfhxjtx.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gdfvimupx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gywgspomu.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwjwzbev.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsgljfmu.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gqpxezyob.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giahflvli.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvbrayvj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxgmgzwo.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gogykspyq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gzwayyquy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gklyivwum.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlirkqcr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/ghwjcpgtz.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gfjsjfdjw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gfwtafrjz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzpjnovq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnvcpllp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpqsogue.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjizhzwes.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgwkejdl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaxvhvsn.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gbmsjgkoy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gjbhsuxop.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpdsrgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbrilwlf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gbszqkjdg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvieqpsyp.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpevfvzug.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczvrvbnz.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/glnuyelgy.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/ghjwelutp.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/goonfrqkw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gelojzriv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmblptsnn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grwlpdrri.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuhotgjp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/glvcxahtz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghgheqpdr.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqgcbqfo.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/geqwnbfoi.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxvwcxmlk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbohyavp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gwvkmmhaz.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaikftzgh.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/genvhlyqx.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gplcphzfb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxujyleuh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyzeihjj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbytvqgx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gejozugmx.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gtcrybbes.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/guenxlofm.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gyjzmdjds.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glrlnxzjx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqrkywlg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gkejgxxnq.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqkjhgy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gaouxlxhq.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gteozkxjd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gumnmnxhb.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbayzkgoj.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdmmxllfg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gtxioqmjn.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gdgmoqfyx.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtvnwxnun.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwqzquqs.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjkeposh.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmyagwomg.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvtlkeoc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdhraahk.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gdfncqrjp.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggpledeft.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkbmbirrb.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsradqfl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gbalvavqm.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmebtlvsk.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gewnuciyh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giozvzapr.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksnevrdm.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbmacwuch.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/geunmdcvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmfyyppeo.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grllsbnre.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogiffhsb.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghggfmhdq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsnaejgq.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkmaupuy.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbklwcpyr.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/garmievqd.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbgymzmw.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjawpumgp.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gvqnwlscx.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gousgqowb.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnoeshpg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gqwlrfwxl.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gzhpylvne.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/glhrzjggs.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gdlddagtn.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpmxwvzqr.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gylsdbowt.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpusoxzsi.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gcxohfack.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/ghymkjobb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvfnusqw.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvfyzryd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlpkslnv.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmljqhux.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqisspbij.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyqepczi.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpioeglb.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gansrczkr.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdzgyuith.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbtdwtgr.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjfycodt.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqbxtvwd.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gfmtmvhlf.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gnedneqwb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gbnzfmlom.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfrjreyg.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmzyclfz.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbxsxdqqo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgiyvhnp.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/glppnzahb.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gcjgvzswn.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gwrxjzfbm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gklbylwvc.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfwonilwd.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnjmgnp.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gctiglfsx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gilhhabkt.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzojbees.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvrtfxjm.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfvtdljk.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/goffhayew.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmspppibi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtrpgwrj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxurhzoa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gcgoboeye.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfjqhgiln.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwzfisjfd.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcrhdfal.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gwzogmkbp.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcfbhurk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjbqxlkx.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghadccmmt.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkgiobvq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgzpbbmh.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/grpqdmhtt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjazdbnve.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwxojhpv.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gckzlfwsl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gtluzbsvm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/goqruiqiy.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gffckruwu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmpdrfrl.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/goxfonthg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/glqrbzqrz.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/grqqrwcby.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gvdppibnm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjsnowiq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gvhlujxgi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnfjqquc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/guguotzbd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gungyznex.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gazptggwa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuzsaxyp.sHtML


<!-- 参考信息 -->