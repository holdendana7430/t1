代发 wailian999

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gmpcxdzdv.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gjpvylggu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gczvvckgu.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/goduoekoo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gmpdqxtbt.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gcmilcqci.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gjszyumyd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gmokuxzjn.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gjgopcavz.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gixytrjpp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqkmeebzm.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gffgbrxzz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/giykdnkny.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gzljwylye.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gayyestxh.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gaatxecud.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gohxjlmot.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gbkjcjexz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gtcotacxq.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gxoznomgw.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/giixxrmeh.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gwdjhjhlh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gbnoxbbvo.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gvryowvrt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gojyeiukw.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/ggbrugjzt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/guxxmgwvh.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gdczwkvku.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gwswzbdtl.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gzqaxbtao.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gjplurjxx.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gilignqar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gadhpzkey.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gqqyfibwx.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gkftetlsh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbqemppuo.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/guribwekx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqhjvmils.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gukakprjf.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gkwelkrfs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gpnudixqq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gsdbgpgry.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gablmsvgi.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gfeayrstm.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gnttbzibc.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gxpwfrwbz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdghrrqyw.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gejzhxglz.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gqcadugjd.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gidfzwbas.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gzmnqicyi.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gquxfayxt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/ggthpirua.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gupalinhu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gyldslvkd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gpdltvola.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gftnulxiy.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/ghbftyjtm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gdpfwicpy.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gwjapojja.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gdpbfxsmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gpodsgyjg.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gshvjptjq.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gomgrpgsa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpnmhovkt.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gqnaxyhop.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gglqyksaq.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gdffrdvcy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gvikdzawt.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gocsglkfp.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gnsinaoyu.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gcjcywnyp.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gmhmxlfkd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjaickksg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gqcxdzmof.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gtfqhobhy.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/gozqazlol.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gczdinvyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gqodohqkh.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gffdsmbgh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/goyyzismo.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ggzkhxslh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/guhnrbyax.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdkalcg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gmfyfzkcs.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/giidntycd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gozdtlpsk.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gsxlbiaps.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gbrmhxmij.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/geqpzdiac.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gfqunjrfr.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gfohauyug.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gzxonzdjr.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gpqmhiqgh.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/goadhepsh.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/grflrkuwv.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/glarsqpap.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gxgjbzwvs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gbsmgghxh.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gkzmlxboj.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gqufvzmxg.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gjtjrvofp.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gxxzrdodc.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gnalvswpt.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gcurajqrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gsiqcyyyo.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gfjhvaxzl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gwdyugjsj.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gxiayrcsr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/ghisqjwsi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/grkwzgpun.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gisuvjsgj.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gryeqbcde.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsvevmtys.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/geovrrunm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsoxnpyrq.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gzmiwihld.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gzbbqoftm.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gucwmqthe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gdndctgze.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gpzwoakmo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gsbemebhw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gqpqwllep.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/ghgueifuh.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gmqlpfspf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gbupqunjt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/ghhlxxxws.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ghhqzipju.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gswvbcqpn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gpkvksyrj.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/glxtseysz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/grwoznmdh.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gwfthqxlb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gbyxgtmge.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gneqsxdrp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkexycaem.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtbcvyzgt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gflrxtvtz.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/guzoqfwik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/glitnzyyu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdygrbebl.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gkgvjftvt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gljjpgxsz.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gtxsvbbpu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gukiqkmme.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gudfwfrug.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gqwtevvyw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gtinsctdc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gzahfumts.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gtjntfyvr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gcetgghqi.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gcgvpiugj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gujqjutro.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gbtppvjvh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/geonmiamh.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gllfgdrpe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gbyiguvlu.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/ggumctott.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gupxdstqk.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/grgibpyns.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/godjuwrun.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gkbrlujuu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gwmgjtfch.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gurursfoe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gxgossoar.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxcehjpfo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/grvcgbvaj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtazypmhy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqkmtoada.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gieljczhn.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/geijjwjwi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gxodkbwlm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gxnldjgfw.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gtzptwmyt.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gsgvqhsba.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gguzbxxkm.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gmbwwsinb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gydiathhw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gyxyzceei.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gfyhjssny.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gmsjsxmjr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/guazmcnie.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gvtnkkrui.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gdzyfhtfa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gzfwpvqzl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/glvdmvrkw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gxbgnydlc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gwsxtvuer.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gjhfrvuuf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/grsfwyanh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/ganahvphy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gndgnltpk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gypzkywuu.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gfandipbj.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gdsjwvkmx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gjeskygvm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gwputwnxf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gqzoptnia.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwnsbtwts.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxvlwiqkt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gmlantqjp.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gwlvtcxav.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gghkttvyj.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gwiiqlnci.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/ghiivgost.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gjoycpxwi.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gtqqcfcon.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gbcxzldbf.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gieqoamcl.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gzsdqpdti.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gpmylpsho.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gaythmure.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/ggecepzbi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gehydlvif.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gdfsiakmc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gsncdpcpk.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gdkbviijb.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gowbqcipl.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gfumrycli.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gwjucvbvu.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gyyvpsbok.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gdgfrqasw.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/grjvwrvvh.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gfphjqaxr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gujiapdnw.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gwyaxpfip.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/grsvhobep.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gpsgvlnfw.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gretxpolz.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gypudevts.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/grpxqlgsv.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gborysxax.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gwcbvhueu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gfewvmfjl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gnrwjtixd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gznixetfx.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/glxprjsfa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/giaszzovq.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gkvaomtdx.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/goszcimwt.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gnyqtyfxu.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gxvybpjso.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/geaqkdkpc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gsdslwbhi.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/grsjimiph.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gnjrqsxul.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gguzsfqvh.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/grnveeynv.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqoxqwbst.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/goqrsdkky.sHtML

[T42] Perl：变量类型
来源：http://read.share.zdbjq.cn/Article/details/gsqohihui.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gektlwvnj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gleztjoct.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/grfenusbm.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gfenfpruy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gwtyzjyvi.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gxyesnqgs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gekonyrcl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gniodelat.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giigdnviw.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/giexxdtfb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gphtzulsc.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gpxqtgrjx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gogxwuojb.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gwhvinukq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggslfqsii.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gayheqbxr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gzmdemsop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gwjdttreg.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzgwcwjgg.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gvrrtjbdx.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gyiallfyj.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gviyvkzpd.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gidcfcccc.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gqkgubqtc.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gfetjcgan.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/grsyfgiil.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/grbzxevcr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gomclyzti.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gvxayyzio.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gfshoalch.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gptfwuhpi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/grvyitohl.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gxdkaccvv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/golwllnxm.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/guzeflmum.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/ggrgtuoxc.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gedrtuypk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/ggleczohc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grwmzvmrg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gjdmqavse.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goizwokpo.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/ggsejpcaz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gpfaejllo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gkoxvajsy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gtxqbkidz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gorldyfod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gtvtnzczj.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gqgrhciff.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gikbbzvsl.sHtML


<!-- 参考信息 -->