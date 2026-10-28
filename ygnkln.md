代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dashuyun.cn/gtgkzeiskb.html

[R66] 定时任务
来源：http://hz.yueranfly.top/gtkauywgis.html

crontab -e;  crontab -l
来源：http://hz.cashguo.top/gtjovnubaw.html

[R67] 生成随机十六进制串
来源：http://hz.yj202588.top/gtisqzjktg.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtgfbiqdez.html

[R68] 计算文件校验值
来源：http://hz.pycfn.com/gtjvdadebn.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenjidiqi.icu/gtgnbhcwjx.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtxfoncttc.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtmxjkohrs.html

[R70] 时间戳与互转
来源：http://hz.jinqigfzy.top/gtkdchwcwc.html

date +%s;  date -d @1700000000
来源：http://hz.zycfv.cn/gtpkwumqmx.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gttvpldxyr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gzhubu.top/gtzwhpvctv.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangtech.top/gtntzquhgo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gthxcopirx.html

[R73] 分割大日志
来源：http://hz.andypj.xyz/gtscgwvfpo.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtwkorvacj.html

[R74] 批量重命名
来源：http://hz.zycfv.cn/gtcjfcjtbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtqyplrkdk.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtworxgujk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aizwys.cn/gthorsvbvo.html

[R76] 使用临时文件
来源：http://hz.chenlongwang.top/gttydajdui.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtqppiocrv.html

[R77] 读取用户输入
来源：http://hz.yj20258888.top/gtsrmhnrpu.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtnjsgsuob.html

[R78] 交互式菜单
来源：http://hz.quarkkingdee.top/gtpqxdfuhq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gtagnqfmuu.html

[R79] 解析命令行选项
来源：http://hz.cucudq.cn/gtnizcsstc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtkyleqzdf.html

[R80] 查看脚本执行耗时
来源：http://hz.yueranfly.top/gtnolugktv.html

time ./run.sh
来源：http://hz.xylfe.cn/gtnbjsmlxh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnhsbbqhd.html

S. C / C++ 专题
来源：http://hz.52xcode.cn/gttveyvfza.html

================================================================================
来源：http://hz.meibo888.top/gtnnvvwiwc.html

[S01] C：Hello World
来源：http://hz.c1oappe.top/gtlecmmras.html

#include <stdio.h>
来源：http://hz.ydjk.org.cn/gtxzshcycc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtgyjbhrtb.html

[S02] C：变量与格式化输出
来源：http://hz.cashguo.top/gtpsougvoe.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gtmkzikotc.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gthjkwvjxg.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtqdesptry.html

[S04] C：字符串复制
来源：http://hz.fengsongda.top/gtrynuxero.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhiwuduotai.top/gtbkojfowt.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtfniigphq.html

strlen(s)
来源：http://hz.chenjidiqi.icu/gtjdgjtvbp.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gtdgvvmwmt.html

strcmp(a, b) == 0
来源：http://hz.cucudq.cn/gtfxirgtzo.html

[S07] C：数组遍历求和
来源：http://hz.gaohongyu789.top/gttsunrrqv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jianghu66.top/gtoolaposr.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangtech.top/gtewdryuvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.smart0.xyz/gtrqsnquoe.html

[S09] C：结构体定义与初始化
来源：http://hz.jinyuanbaomall.cn/gtlitktpty.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tianlin.xyz/gtfhypdzgk.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtduxeyceb.html

int *p = &a;  *p = 5;
来源：http://hz.zhongyouzk.top/gtovrhnqqu.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtltappeif.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cheryme.top/gtyfjgidou.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtzbqchhcu.html

fclose(f);
来源：http://hz.hnxiangtu.top/gtglwmhzul.html

[S12] C：写文件
来源：http://hz.0kj1m.cn/gtbdsjjqrw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shangyingyoupin.top/gtjuyhvwap.html

[S13] C：宏定义
来源：http://hz.zhoulong.xyz/gtafialewl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shuidangran.top/gttpffiejp.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtbeddgeop.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.kuanghao11.cn/gtyaspizjm.html

[S15] C：类型转换
来源：http://hz.hnqzz.top/gtwpzlqwrk.html

(double) a / b
来源：http://hz.ehwqpu.com/gtrjixctaa.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtwzcvqwqr.html

x |= (1 << 3);
来源：http://hz.jinqigufen.top/gtqklbryzt.html

[S17] C：安全拼接字符串
来源：http://hz.316326.xyz/gtcvhsphpo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ppjwa.cn/gtuxpkymnr.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtthovxjtj.html

int main(int argc, char **argv)
来源：http://hz.cdnleiting.top/gtidawqnmi.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtreswxgso.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gtxcqmuzdp.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gtniwgsvcz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtpstlozav.html

[S21] C：字符类别判断
来源：http://hz.mhx1999.top/gteqvxullb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtbtjbnubf.html

[S22] C：字符串转数字
来源：http://hz.ydjk.org.cn/gthtukjbmo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shuidangran.top/gtcafzqdyg.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtpjqukzbn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxinkj.top/gtacoqnbdx.html

[S24] C：获取本地时间
来源：http://hz.ywan-chungtsiang.top/gtgnbhsyue.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tianlin.xyz/gtyoyjccgq.html

[S25] C：内存拷贝
来源：http://hz.chenzaomai.com/gtsqtidmov.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtsoytgqvh.html

[S26] C：内存清零
来源：http://hz.zhaomingkeji.xyz/gtorpupdug.html

memset(a, 0, sizeof a);
来源：http://hz.wangshuangyany.cn/gtamwycpol.html

[S27] C：定义常量
来源：http://hz.yangfankeji.com/gturxykmdi.html

const double PI = 3.14159;
来源：http://hz.meibo888.top/gtxigjrqrf.html

[S28] C：静态变量
来源：http://hz.nanxinkj.top/gtxnehsfou.html

static int counter = 0;
来源：http://hz.shanyushiyangtech.top/gtnevfzclx.html

[S29] C：变参函数
来源：http://hz.tianlin.xyz/gtacfjtiul.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jiagoushi.top/gtvyeavopg.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtqtfcnqut.html

#ifndef X_H
来源：http://hz.jinqigfzy.top/gtfdvholxa.html

#define X_H
来源：http://hz.yuxming.cn/gttzcxwhsq.html

#endif
来源：http://hz.feifeiyinyue.top/gtpuwbsfes.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtoscyerld.html

#include <iostream>
来源：http://hz.pycfn.com/gttubjltli.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gtnqpjdsrw.html

[S32] C++：字符串
来源：http://hz.jyoumei.cn/gtjyxyzeai.html

std::string s = "hi";  s += "!";
来源：http://hz.sysykeji.top/gtxwzxykdr.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtqtyyzgfy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pengpengdd.cyou/gtakmsiamu.html

[S34] C++：遍历 vector
来源：http://hz.hongshengwenyu.top/gtzwjavxcv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.iojbl.cn/gtolxyfgdi.html

[S35] C++：map
来源：http://hz.ppjwa.cn/gtpsnfbxlp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtekgbabfe.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtcwedudje.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtkuwztcjv.html

[S37] C++：set
来源：http://hz.iojbl.cn/gtytquiiov.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtpfdjnpee.html

[S38] C++：排序
来源：http://hz.316326.xyz/gtlcwkvqac.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtyflkzvgj.html

[S39] C++：自定义比较器排序
来源：http://hz.zdqjudy.top/gtmzityowl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.bjfxy.top/gtfsfkadyd.html

[S40] C++：查找元素
来源：http://hz.zhaomingkeji.xyz/gtjxifpfwh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gtzhnnzmoh.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gtfhjtvtvy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ehwqpu.com/gtabrrbicj.html

[S42] C++：继承与虚函数
来源：http://hz.pengpengdd.cyou/gtxbriedst.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtxghinppd.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gttskfoznl.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnqzz.top/gtawgjfdym.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtkigylfqy.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtrqekakkj.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtlmuvmrbz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gaohongyu789.top/gtsdaezsar.html

[S46] C++：函数模板
来源：http://hz.daria6918.cn/gtvjozfcak.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtkzwbyuqr.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtedhkpuuo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hammf.cn/gtgrncovqk.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gttpnqsjgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtqjdbmgpm.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtgepytzvn.html

[S49] C++：写文件
来源：http://hz.gotoacloud.top/gtsjabeemk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtvxpwottw.html

[S50] C++：格式化数字
来源：http://hz.bjfxy.top/gtydsjmetv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.9152youxi.cn/gtsgullcni.html

[S51] C++：显式类型转换
来源：http://hz.snrcjt.cn/gtgzhwciyq.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtfgdxsnax.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gthdbydcjq.html

int size() const noexcept { return n_; }
来源：http://hz.zhengqikj.top/gtcsgbicep.html

[S53] C++：移动语义
来源：http://hz.zycfv.cn/gtzacxemdf.html

std::vector<int> w = std::move(v);
来源：http://hz.yvedp.cn/gtwqjlgjzr.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gteylsyobs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gtxklzbtal.html

[S55] C++：结构化绑定
来源：http://hz.svipenyu.cn/gtdsuzovuq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtkyhqsbet.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtamcdstxh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtltaqmbsq.html

[S57] C++：编译期常量
来源：http://hz.cucudq.cn/gtfnabqvyv.html

constexpr int N = 10;
来源：http://hz.shanyushiyangtech.top/gtrbwffvxz.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtqgtsycjm.html

namespace ns { int f() { return 1; } }
来源：http://hz.c1oappe.top/gtgbsryqim.html

[S59] C++：静态断言
来源：http://hz.sxryk.cn/gtvapqioto.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtdafoslra.html

[S60] C++：遍历并删除元素
来源：http://hz.tanke756.top/gtuqhrazir.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtjezdzegz.html

================================================================================
来源：http://hz.ehwqpu.com/gtkgooubyb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtktlzednl.html

================================================================================
来源：http://hz.0kj1m.cn/gtzmsemvgl.html

[T01] Kotlin：Hello World
来源：http://hz.zhijiandao.cn/gtbbhngzxb.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtzaocxtkr.html

[T02] Kotlin：变量
来源：http://hz.xingfuxueyuan.xyz/gtahbavpoh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.daria6918.cn/gtpkerpdyc.html

[T03] Kotlin：字符串模板
来源：http://hz.tanke756.top/gtemugjcgu.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtuzgxsbad.html

[T04] Kotlin：空安全
来源：http://hz.316326.xyz/gtkfzeyvip.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtotfmblxp.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gtbysmfsvl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtaqcpdbuy.html

[T06] Kotlin：集合映射
来源：http://hz.c1oappe.top/gtguydtovb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.andypj.xyz/gtddbmuwwu.html

[T07] Kotlin：集合过滤
来源：http://hz.wangdashe.top/gtxlwiulae.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinyuanbaomall.cn/gtkasvsukj.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gtftcxwxkp.html

data class User(val name: String, val age: Int)
来源：http://hz.hysaishi.cn/gtnkoclmdd.html

[T09] Kotlin：扩展函数
来源：http://hz.yuxming.cn/gthofrgrdr.html

fun String.exclaim() = this + "!"
来源：http://hz.sweek.top/gtjbzluauf.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtyutqjfqu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj202588.top/gtychibmpn.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtvaoncyhv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hongshengwenyu.top/gtptjvbltd.html

[T12] Kotlin：解构声明
来源：http://hz.cdnleiting.top/gtbkdkpcbr.html

val (a, b) = Pair(1, 2)
来源：http://hz.hongshengwenyu.top/gtzmefwqgz.html

[T13] Kotlin：只读 Map
来源：http://hz.yj20258.top/gtvdzhznoq.html

val m = mapOf("a" to 1)
来源：http://hz.iojbl.cn/gtmmpcexej.html

[T14] Kotlin：循环
来源：http://hz.zhengqikj.top/gtooekbjpc.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtvfsyniyc.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gtyyuammmh.html

interface Shape { fun area(): Double }
来源：http://hz.shzxlz.cn/gtsygrgmkt.html

[T16] Swift：Hello World
来源：http://hz.daria6918.cn/gtilyroinc.html

print("Hello")
来源：http://hz.guannengcc.top/gtzohxlsdu.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtmnoxdhtt.html

var a = 1;  let b = 2
来源：http://hz.tanke756.top/gtjjiemqbt.html

[T18] Swift：字符串插值
来源：http://hz.sxryk.cn/gtjiozarvh.html

"值: \(b)"
来源：http://hz.jiagoushi.top/gtoljxzafr.html

[T19] Swift：可选绑定
来源：http://hz.jlsjyb.cn/gtdfcrflwa.html

if let n = opt { print(n) }
来源：http://hz.chenjidiqi.icu/gtqkiclqlo.html

[T20] Swift：数组操作
来源：http://hz.zdqjudy.top/gtdrvjrunk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daxiang520.top/gtxfsdaxut.html

[T21] Swift：遍历
来源：http://hz.xuanzx.com/gtkdfjsbar.html

for x in a { print(x) }
来源：http://hz.quarkkingdee.top/gtlqmtigrz.html

[T22] Swift：字典
来源：http://hz.jlsjyb.cn/gtbbzwdcgs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gtcuqyracc.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtlomnjiaz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenzaomai.com/gtnjzpchfa.html

[T24] Swift：闭包
来源：http://hz.nanxinkj.top/gtablmxnsi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tian-w.cn/gthxycclzb.html

[T25] Swift：结构体
来源：http://hz.zhijiandao.cn/gtschinclb.html

struct P { var x: Int }
来源：http://hz.yj202588.top/gtzhvnfuds.html

[T26] Swift：类与重写
来源：http://hz.ybcxt.top/gtavvvlxik.html

class A: Base { override func f() {} }
来源：http://hz.yj20258888.top/gtxarhmquf.html

[T27] Swift：错误处理
来源：http://hz.pycfn.com/gterziqzzx.html

do { try f() } catch { print(error) }
来源：http://hz.0kj1m.cn/gtnpjetsia.html

[T28] Swift：枚举
来源：http://hz.tian-w.cn/gtfmfdoibk.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gtfikhncrv.html

[T29] Swift：guard 提前返回
来源：http://hz.hammf.cn/gtywxswkqi.html

guard let x = opt else { return }
来源：http://hz.kuanghao11.cn/gtgepfvith.html

[T30] Swift：协议
来源：http://hz.0kj1m.cn/gtgxdaotyw.html

protocol Shape { func area() -> Double }
来源：http://hz.dashuyun.cn/gturornjlc.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangtech.top/gtwmxljfyv.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtvpuilcow.html

[T32] Lua：局部变量
来源：http://hz.ehwqpu.com/gtktaqqllf.html

local a = 1
来源：http://hz.yj20258.top/gtsxsswyyc.html

[T33] Lua：表（数组）
来源：http://hz.mhx1999.top/gtxqrevndg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.havefunace.top/gtzluqdbxi.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtwyrlxrog.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.daxiang520.top/gtzgnaokyd.html

[T35] Lua：字典表
来源：http://hz.snrcjt.cn/gtayabmyzy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtbewwujwy.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtruxslava.html

function add(a, b) return a + b end
来源：http://hz.zhiwuduotai.top/gthvmxmbds.html

[T37] Lua：字符串拼接
来源：http://hz.guannengcc.top/gtxfvrkrkk.html

"a" .. "b"
来源：http://hz.ydzc1.top/gtcpihsazv.html

[T38] Lua：条件
来源：http://hz.sxryk.cn/gtiojlaypf.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtpvfljsza.html

[T39] Lua：模式匹配
来源：http://hz.zycfv.cn/gtjgoclyji.html

string.find(s, "%d+")
来源：http://hz.hysaishi.cn/gtjfmsiutb.html

[T40] Lua：元表
来源：http://hz.redwolf501.top/gtejfwkpsb.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtjqecedzr.html

[T41] Perl：Hello World
来源：http://hz.zdqjudy.top/gtfppufqhf.html

print "Hello\n";
来源：http://hz.zhijiandao.cn/gtuxvrybbh.html

[T42] Perl：变量类型
来源：http://hz.iojbl.cn/gtbvrfhjjv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.quarkkingdee.top/gtzjzzltam.html

[T43] Perl：字符串插值
来源：http://hz.jiagoushi.top/gtdilqvdqm.html

"值: $a"
来源：http://hz.haohaochexian.top/gtfajmlnzq.html

[T44] Perl：条件
来源：http://hz.jyoumei.cn/gtaolirmdb.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtvulxqrkp.html

[T45] Perl：数组遍历
来源：http://hz.tanke756.top/gteocpnapg.html

for my $x (@arr) { print $x; }
来源：http://hz.hongshengwenyu.top/gthyuhjbgt.html

[T46] Perl：哈希操作
来源：http://hz.zycfv.cn/gtknoisepv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.svipenyu.cn/gtsefliswr.html

[T47] Perl：正则捕获
来源：http://hz.fengsongda.top/gtibkcefyf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dianchejie.cn/gtxbawdobt.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtbhioqavh.html

$s =~ s/old/new/g;
来源：http://hz.nwbrower.top/gtagzyxtmk.html

[T49] Perl：函数
来源：http://hz.gogol.net.cn/gtbdslkaai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.snrcjt.cn/gtahfnlnpq.html

[T50] Perl：逐行读文件
来源：http://hz.svipenyu.cn/gtksplwlvr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.9152youxi.cn/gtztkrhtzq.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.dashuyun.cn/gtecaoabvm.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gtgzzutvmc.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtilyhkhiu.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtlunqzlst.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtfypfakux.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtosarjzxo.html

s"值: $b"
来源：http://hz.yvedp.cn/gtsjqpbixy.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtetqemser.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cdnleiting.top/gtzmeieeva.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gtxiwnsglc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nwbrower.top/gtaiwioydu.html

[T56] Scala：样例类
来源：http://hz.cheryme.top/gtwzaaxpxi.html

case class User(name: String, age: Int)
来源：http://hz.xinyue.icu/gtvrpzcpob.html

[T57] Scala：模式匹配
来源：http://hz.zhoulong.xyz/gtqyomzocg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ywan-chungtsiang.top/gtkfxwycev.html

[T58] Scala：函数定义
来源：http://hz.zhengqikj.top/gtglqujfut.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cdnleiting.top/gtiswjzzhx.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtjkvkuchx.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gtrmrorkaf.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangkeji.top/gtjvrlbhuw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hywenlv.cn/gtingxiwom.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzprfxttd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtxselxncp.html

================================================================================
来源：http://hz.sufxvd.cn/gtmjoawhzt.html

[U01] Py：创建虚拟环境
来源：http://hz.xinyue.icu/gtmyzuxgle.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuanzx.com/gtzmowhqvg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cqqwz.cn/gtkktffhib.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zdqjudy.top/gtvmbcnqkh.html

[U03] Py：加载 .env 配置
来源：http://hz.hnxiangtu.top/gtvxcymqwd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhengqikj.top/gtxzzfdkkk.html

[U04] Py：变量调试打印
来源：http://hz.cqqwz.cn/gtfoitzctv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhaomingkeji.xyz/gtnffiteia.html

[U05] Py：列表去重且保序
来源：http://hz.cashguo.top/gtbsxiypxu.html

list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gthgrtymlv.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangtech.top/gtggfigxzj.html

{**a, **b}
来源：http://hz.kuanghao11.cn/gtsxmqsfwr.html


<!-- 参考信息 -->