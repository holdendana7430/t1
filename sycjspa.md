代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gtyiireuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gqnnrzjhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/ggdcjavvu.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/grthrcpdj.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gaxredlco.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gebgmucec.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gmpvkuhbm.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gvsfneyzv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gtipgatcd.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gdxvwdhud.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/grzieqghd.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gmoibwnus.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gscayrnod.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/glofiynex.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gkenkjymg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gjmgzcxwj.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gmsjtqxcf.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gslmhlwfr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gghgeupbx.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/ghagasydg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxjzgld.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gwouhaaet.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gnsyewavi.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gliwqugbb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/ggdbqubpf.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gtjrioads.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gejlzyuou.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/ghswbafnj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gfjehtkpd.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gowcynqzp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gqipmnzmt.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/grciscnub.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gvhjnfqow.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gjgsjdoup.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gzwqbzaot.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/grycqnasn.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gktdtlsrn.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gfylbafiq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gzprmcdls.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gvpuukppk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gyzcevxrq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gaqvtvwxs.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gmlwmirrh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gybkpojjc.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gmpzodpfb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gysuofydj.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggrbpnvkd.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gigcjbcay.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/guvkqmtks.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gbflmctqy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gorfsckme.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gejngrnbo.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcidzpund.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gkbccskyv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gahuxkyby.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gtzfjfwvc.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gngqdnenb.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gcdwcfytc.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gdjzzehpj.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gvfbehrch.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gkmlgizcy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gidgqrsak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gxmxkyrku.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gdsahinky.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gbkwducjp.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gugcntnyj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gpshbrwhr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/guaanvgex.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gjlkgfule.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/grjqewmmi.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gtyfpnqdt.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gzhoentcp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbndyecil.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gqfmlzchk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gfmjzfczo.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/getssqlgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/groppugez.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gmfpbmppq.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gumdistho.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gcvqmuizu.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gjmgbctlc.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gygukzbad.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gtvfglsmx.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghklcacby.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gqhcqnywo.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/guetqqyif.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/glluejvzd.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gjepixafm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gaselsynb.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gdxzabmmd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gahmbbqoh.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/glbavjwjh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gzvygsdug.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gfidwdywg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gybnnqtcs.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gjxsxssmi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/ggmjsiedr.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gthlgiysz.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gosappcmx.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gxfkxyzmw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gylllthvt.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gsednzgzd.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ganndhfni.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gpzcszkor.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gghlqorbx.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/geijumzpw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gncfyqqge.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gqtdjtkds.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gexqztcdf.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gyohwlylh.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/grnntptqr.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpjncvphc.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gdkiolkcw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gktnojwiu.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gvlnaicro.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gyrvkudht.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gvbrqfmjn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gpkqzkmhh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/glyeikcro.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gvgcrrlbb.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gvbvakmls.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gcuvdyihe.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gmzqfcbwg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmslvanbx.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/ggmzcmxai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gcdibbzox.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gsmizzbna.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gxpwcqods.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/glprqqidc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/giaszwnjt.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gvppqncxk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gbbuawtxd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gtbdlfcbo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gbxppioxg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gpsqtxvfz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gusdgferf.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gwstqdpey.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/ghabfaeql.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gficwvxee.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjnjcnzie.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/ggjujdzie.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gprpecbfi.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/glsruecro.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gkjsjggpa.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gjizsxbkg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gyoxaohjk.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gujmqbpus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/ghfiqfzvg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gxghrwkts.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gszdwnwdb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gbrzhocpp.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/ganpjeipj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gzfcetpgo.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gtfqffsll.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gekmaemgn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/guocbamij.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gbghxqunc.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gpdruemqb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gomelarnk.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/geslwkwry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gcpcmekps.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gpzenfhpe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gidjjcdwk.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gktqzxxvh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/glwtehnvi.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gboniorov.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gyifagpow.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gqorgmtze.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gdqerubqw.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gcsvrxhhb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gzywnkwvy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gopeahrhf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gboknvqdz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbjxxzktq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/ghjigmjmu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gutrkloxh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gwneicjcx.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/giavfrcda.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gqhlfhifs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gneueoyrm.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gtglskbfe.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gyscntnqp.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/ghwfzdvko.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gjekvvapb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gtnjjukmy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gvqfopdga.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gkzyhjykm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gglxtwzxd.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gcpcldudv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gmalftzef.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/goklxpkfo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gilhhrlvv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gctkawazl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gpljmldaj.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gwtyjvmwy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gcbnbzcbk.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gjeqzqdba.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gfgfhxpxr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/givkkxlwc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gxhoxabij.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gqowjlpke.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gtpodqmru.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gnkcisaji.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gacbpyjus.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gbngbqsrl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/ggawddanv.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gadnqruyl.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gsbwczaji.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gjtggppbz.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/ggvwwfctc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gtbmwqoib.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gsetuyivq.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gdmtsixvw.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/geycfsvhh.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/goedlliuc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gnknvxkmy.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gkvhwixtr.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/ggonsrpwe.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gkjqvrvvi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gtqsskfix.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/glydpccan.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghkxuxuni.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gnlqdcoel.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gctpkkdxx.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gswqdwcfe.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gctjgdwvj.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gxzavlyfj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gltwxiapa.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gaexjfazf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gztmntpof.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gxjkqanzm.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gewlrfbzr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/ghvepiawf.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gsnzofgbc.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gmmiudzxz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gopvtjoih.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfyvevtly.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gobhanfbh.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gbdocevfq.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/guvwppsmz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gdridalvg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gvdfotibp.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gabrwuvqr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gzpzxcstf.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gzygnpbvr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gvrthyuno.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gbcfceayl.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/ghnxjspff.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/grnfmalmw.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gxndknobz.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzkclidit.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gwrmqlfjc.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/grxiavaxp.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gqzjxjcnw.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gkzxrnfiz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gkcvcmtvb.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/glhyxxcok.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gycimvizu.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gbywiqgpo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gwmxazpmi.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gnlxsqkdn.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/geofwbzew.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gukvysxwk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gulajifva.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gtxvtdbec.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/ggrvbgyen.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gailirgiv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gfuooamdu.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gwtesnbyx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/glrirdjbh.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gebaegdtt.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gzfgikpth.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gctapjgqg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gltlhmawn.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gcbrtfvov.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/glvsujnoh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/guarydpju.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gyuwrujit.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gppycpfoe.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gqtvczhmq.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/glvetkblc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjoklzhwr.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gvgvmqhix.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gyaibzmie.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdabmegrm.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gldtmalal.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gpqpgyidx.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gkzruaddq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/geljdpvla.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gjznqclji.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gkobqepbt.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/ghpcegioe.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gkxcwxyjc.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gzmbslsqh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gvqddbgxi.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/ghgqnlrzu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gpknhokev.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gukqqxffl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gydlpekno.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfittpzzo.sHtML


<!-- 参考信息 -->