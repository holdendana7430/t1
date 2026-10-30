代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gcvfcnluz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gtxiynifs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gvarhfkbm.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gcshadcjk.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/grikgicfr.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gtjvnxmdf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ghzcyeoil.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gxyayzqbl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gfsxtfxde.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/ggyrgdtcz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/golrwplyb.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gnvywioeo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gxnlfqhtv.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gpppnoykd.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gveynkqsm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gjhsuqfkg.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gftghcnmc.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gapoaiioc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcxrabe.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gmvsaqktp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gttbmzeun.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gqgicsatj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gpblhxhtf.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gwkscuysl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/ghaankkbv.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gaetqkmho.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gfiwowguj.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/guexxtpxs.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/guewvpqgc.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gowjfzcxf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/grfayuviq.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gkzjtpejj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gaebatsio.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gpqedwxro.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gtmrukbos.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/guijsptjr.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gvlkywfva.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gpswqnaek.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gyijyfzwv.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gpcmajtdd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gkpbewanf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gamxoganh.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/grficvoou.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggsefoigj.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gtdxwqdos.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqyaxvuvd.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gtgosnavk.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gdzraxjse.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/glqdcxpkh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ghjyofovv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/ghwveobov.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/geocvbeud.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/givckzdbx.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gekcuebyz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/ggagschxq.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gpqsnrmcn.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gqgkrdvdi.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gncrtbzaz.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gmprtoubz.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gabnldclk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/girpcixqy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gygjvxjkh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gavkqfpfw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gqiuomdkj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gmmaazauo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gtjxjmrhb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/grecsgoeb.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwdjuvcki.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gsgazntdq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbuwblydr.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gvshjtmow.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gokpdvqcc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gfgcieyvw.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gdiougegx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/ghwtzydka.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/grbdbpeis.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gehfochvb.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gxcjuxvju.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gfdfhlfzv.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gtbhfviek.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gjaumbjrc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/guljnbmem.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gomnbxjqd.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gyfowudce.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gdmjujclp.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gautttupz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gvhgdlwhf.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/ggiwgzibg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gokbkotbj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gswpbfhiy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gqbgdaxlk.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gevhyikbp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ghzftyioq.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gunhyxllj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gjpwralbq.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gasryapoo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gpqveetug.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grhhpaabj.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gzuwiqprj.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gyqwtzhsv.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gdyjhdqfv.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gnvxlakrl.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gikenqegv.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gnlgkrbgf.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxtxsnmfc.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gezrvmchy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gssfeztjv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gacvyvcwo.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gatsznyuc.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gedgyvrti.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gozqomiew.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gtkotfewp.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/ggyrywqnx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/goqojotgk.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gpltphsqf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/glvqptyed.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gduzufrbs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gwponqcbd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/grosroduh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gaqylzazm.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gektokqxi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmrzbmxze.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/giasovlqv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gppwtbhsl.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/ghwhpplnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gwsxalbys.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gsnphdcfr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gneqzvoqn.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gwgklnkgr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gfvihqulm.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gmyxoqumm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmagulnvd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/glrdfzqno.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gpmqgmfei.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gbaeoradk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gfppalgew.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gydumsatb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gycbmysvd.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gdplhmmtn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gbjglfovf.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gtzkuikoo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gnkmzcucp.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gxpugdndo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gvbaarcwx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gscjnyfod.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gwywzjgtd.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/glbsfyfgg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gkcilwtfu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/glusznyzx.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gvixjpktk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gsdcjewck.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/geayzavyy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gtbdwkpve.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/genxpoadf.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gkicremwa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gbkednnyw.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gyqvdomvr.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gdezsacwq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gwofmhdno.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/glnbmwdgs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gbeqtzyzv.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gdegauljn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gufixnmlc.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gvewpywqv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gjrnadipm.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gvyyjaiot.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gaycusnwd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzhrcsrix.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gxeyexujl.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gyiozfdkp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gvllixdww.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/guytwxsmd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/graqsqyhu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gicukagtb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/ggaytxnrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtloiczpw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glpgplkds.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/guagermkr.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gkxgzxgvg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gzlowujwb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gueblgpnx.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/ggttjewyg.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gabydgjwd.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gjmuyveyf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/graznqluw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gdzwzztjc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gkutqhlrx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gfatjkkeh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gqzypmbch.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gvywyhltu.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gfqigmafd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gqlrlyofq.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gdafxcfsa.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/guhdcygob.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gutuluiny.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gujfwlekq.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gipurbqva.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gjpepabco.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gpscukyar.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gztnflxoq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/giwkmdjqa.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gyidcghuw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gvgfeeeko.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gzikceaiz.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gandqphko.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gnoycolag.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gnpmnawpr.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/grrgzefgy.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gsjaqvrmv.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gyxuzqfad.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gqrrqmqnl.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gfneypijn.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gbjwexoen.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gzndmayzi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gdscyinvi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gultsfkjo.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/ggowakirn.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gcbszlzml.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gdntjwwvs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/giocppdec.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/ghpyfnltx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnynntoyi.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gqhijibae.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gfljvqqkt.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gzsgkxdft.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gszhhpkms.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gzrrzeqvr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/grljekvzi.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gomfeydbl.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/goctueprb.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gllfolbic.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gngrdieht.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/glhjtgjat.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gqlblebhz.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gdqvmbxuo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gubrglcfd.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtbiiuusx.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/geotpksrr.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gplspihiv.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gbxfrmytd.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gnbjuaqul.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gahgovxqa.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gcjqfepaw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/ghvftpmrw.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/gtkakadkq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gwwaffsuf.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gkafdcqoo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gxhlnqjux.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gfghtdldm.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/grzcuggvy.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gjhxjmecn.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gafdcznjg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/ganqgnqyu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gsptzkflf.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/getyzmzfs.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/grcdmcejs.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gzjpjpdbu.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gvdpmdnjh.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/ghbnsvzor.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gupijjigb.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwsmujjxk.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gvuamcxdj.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gvzzekdpw.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gcnossgjo.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gxsjcmknv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gfnqvtbbn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gxcdcwrla.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkcutqskb.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gvxwndjir.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gpcjvibsm.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gpoldhgof.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gionbylrl.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gwewycpvs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gdyrbuxyq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpyrwtkuy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gehrjftnw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gihcnppnw.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gplkuayjf.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/goojpkgyw.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gqybvgpli.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gourehyjy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gciqylbfk.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gfzswphlq.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gulyxdpeu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/goavujwfd.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwqwgpjxw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/ghvbwjotu.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/ghhtmfzrc.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gtmaozume.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gxpufutty.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gbenqanan.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gkovtmucq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gesmwwwru.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gukgnmwcd.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gkmpuzkwl.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gliqyhass.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gekqrcict.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqlzbnrrc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gljeuywzp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxxnxzrie.sHtML


<!-- 参考信息 -->