代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ehwqpu.com/gtbbkbmvyv.html

[R72] 等待端口就绪
来源：http://hz.jinqigufen.top/gtiemouujd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtbvtrvmyt.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtmmcgobcv.html

split -l 1000 big.log part_
来源：http://hz.xinyue.icu/gthfsdjotp.html

[R74] 批量重命名
来源：http://hz.ydjk.org.cn/gtrvgzvieg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.redwolf501.top/gtwcxddhzn.html

[R75] 导出环境变量
来源：http://hz.zhoulong.xyz/gtbiwocohd.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.quarkkingdee.top/gtgxxqamvz.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gthuepgbgh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gthqalqmce.html

[R77] 读取用户输入
来源：http://hz.mhx1999.top/gtzejwwynj.html

read -rp "请输入: " ans
来源：http://hz.smart0.xyz/gtaowvvito.html

[R78] 交互式菜单
来源：http://hz.jinqigufen.top/gtmawflwyi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtrxcsrsma.html

[R79] 解析命令行选项
来源：http://hz.haohaochexian.top/gtstjrzuch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yueranfly.top/gtpsimetca.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtbvvhguxp.html

time ./run.sh
来源：http://hz.smart0.xyz/gtermazkzg.html

================================================================================
来源：http://hz.jyoumei.cn/gtuehonxvb.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtpxnrwpov.html

================================================================================
来源：http://hz.daxiang520.top/gtsidmoqxv.html

[S01] C：Hello World
来源：http://hz.daria6918.cn/gttiegbcww.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtmbyyjtug.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtkkujbuwl.html

[S02] C：变量与格式化输出
来源：http://hz.feifeiyinyue.top/gtwsrzzbje.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtpcpnvsrg.html

[S03] C：读入整数
来源：http://hz.xinyue.icu/gtwzmkaqmm.html

int x; scanf("%d", &x);
来源：http://hz.haohaochexian.top/gtsovzgnus.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtkzxahqwp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtfiyinopr.html

[S05] C：字符串长度
来源：http://hz.dianchejie.cn/gtummxwjxs.html

strlen(s)
来源：http://hz.9152youxi.cn/gtktzvnwsr.html

[S06] C：字符串比较
来源：http://hz.tianlin.xyz/gtzqcbdrzu.html

strcmp(a, b) == 0
来源：http://hz.cdnleiting.top/gtkdaxkrtt.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtzyuzhtvt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtrltigdaf.html

[S08] C：动态内存分配与释放
来源：http://hz.jyoumei.cn/gtgwttxeol.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gttjnjfugz.html

[S09] C：结构体定义与初始化
来源：http://hz.dashuyun.cn/gtukyvtozu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgufenzy.top/gtnbakendq.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtrnzscvzb.html

int *p = &a;  *p = 5;
来源：http://hz.aizwys.cn/gtuxhundwb.html

[S11] C：逐行读文件
来源：http://hz.gzhubu.top/gtwcudwwuz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258888.top/gtvddqdkfj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhongyouzk.top/gtsegseyqp.html

fclose(f);
来源：http://hz.xuanzx.com/gtokqmcwvy.html

[S12] C：写文件
来源：http://hz.hnxiangtu.top/gtecswsihf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hnxiangtu.top/gtxqhjfpjc.html

[S13] C：宏定义
来源：http://hz.wangdashe.top/gtelsuhcez.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtafgvjwys.html

[S14] C：枚举
来源：http://hz.hongshengwenyu.top/gthmobdmvg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtjmlwzvqr.html

[S15] C：类型转换
来源：http://hz.andypj.xyz/gtmeaietyl.html

(double) a / b
来源：http://hz.hammf.cn/gtohvhwled.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtzgahtyyq.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtazwgynsv.html

[S17] C：安全拼接字符串
来源：http://hz.jqgfzy.top/gttdsqpdqa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.snrcjt.cn/gthozioapr.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gthedmynbr.html

int main(int argc, char **argv)
来源：http://hz.tanke756.top/gtsotixjgi.html

[S19] C：快速排序
来源：http://hz.shanyushiyangkeji.top/gtdwwplneq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gthldxbmqj.html

[S20] C：二分查找
来源：http://hz.chenjidiqi.icu/gtkitpypou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtesjdrtoa.html

[S21] C：字符类别判断
来源：http://hz.hfpthk.cn/gtnwqsxutg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yvedp.cn/gtkhagofdf.html

[S22] C：字符串转数字
来源：http://hz.cashguo.top/gtznyxjtig.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtzuhxvheq.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtdcnubqlg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhijiandao.cn/gtxyludhuz.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtiubgzuvp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenzaomai.com/gtnycvamue.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtmjsqppwz.html

memcpy(dst, src, n);
来源：http://hz.cucudq.cn/gtfhloxiuh.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtzldhnrcf.html

memset(a, 0, sizeof a);
来源：http://hz.ppjwa.cn/gtgfleblkq.html

[S27] C：定义常量
来源：http://hz.cqqwz.cn/gtiaqjbfwq.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtxpulwxwr.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtixvvahec.html

static int counter = 0;
来源：http://hz.jinqigfzy.top/gtlyymhxkx.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtbdmgjkar.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtpkrvvkcj.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtzybqqhcd.html

#ifndef X_H
来源：http://hz.zhongyouzk.top/gttdprrmay.html

#define X_H
来源：http://hz.shangyingyoupin.top/gthfmsmhej.html

#endif
来源：http://hz.jyoumei.cn/gtspqympsw.html

[S31] C++：Hello World
来源：http://hz.yonumen.top/gtbqilfldy.html

#include <iostream>
来源：http://hz.xylfe.cn/gtvgtieqqe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtmdudqrei.html

[S32] C++：字符串
来源：http://hz.kuanghao11.cn/gtzzdakwmt.html

std::string s = "hi";  s += "!";
来源：http://hz.ydjk.org.cn/gtnfknyidw.html

[S33] C++：vector 增删
来源：http://hz.sweek.top/gtawrcwjms.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jinghuilouyu.cn/gtadazztrl.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtdwthtbhp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtmwtnpkcw.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtzutyeufv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtnhlaglnb.html

[S36] C++：unordered_map
来源：http://hz.jiagoushi.top/gtgkjxeosw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtpvmkruge.html

[S37] C++：set
来源：http://hz.pycfn.com/gtbhwwyruf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sufxvd.cn/gtgqgqpcxe.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gtydvezzge.html

std::sort(v.begin(), v.end());
来源：http://hz.xinyue.icu/gtqmgmfebj.html

[S39] C++：自定义比较器排序
来源：http://hz.hfpthk.cn/gtomecijrl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenzaomai.com/gtkndzkbju.html

[S40] C++：查找元素
来源：http://hz.zhengqikj.top/gtyazjbmxz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ywan-chungtsiang.top/gtsvhiubkk.html

[S41] C++：类与构造函数
来源：http://hz.yangfankeji.com/gtxjfwrjzg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigfzy.top/gtsietwsrl.html

[S42] C++：继承与虚函数
来源：http://hz.pengpengdd.cyou/gtttuxvhdh.html

class B : public Base { public: void f() override {} };
来源：http://hz.tian-w.cn/gtzlmsvxzy.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtlytyorhn.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinyuanbaomall.cn/gtmtngpfgs.html

[S44] C++：引用传参
来源：http://hz.meibo888.top/gtxixmrjzn.html

void inc(int &x) { ++x; }
来源：http://hz.jyoumei.cn/gtmdvfrznd.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gttgpwbfow.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.mhx1999.top/gtnzjlpzpf.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtwmrwskra.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gticldvejb.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtaclqiumg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gteicimfzi.html

[S48] C++：逐行读文件
来源：http://hz.ivvv.top/gtiaclqlla.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hammf.cn/gtlowklunk.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gtagmfzuxj.html

[S49] C++：写文件
来源：http://hz.9152youxi.cn/gtdeowfcmw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gtwgvfvcah.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtdbbywtva.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtymwqbear.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtkrdiemfz.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtvoiotzia.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gtssucthue.html

int size() const noexcept { return n_; }
来源：http://hz.kuanghao11.cn/gtwbgempux.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtvcjfnapo.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtseitmkeo.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtsvijymdn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ivvv.top/gtvtxtqtrd.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtjjzshgwv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shzxlz.cn/gtlefyrxrk.html

[S56] C++：optional
来源：http://hz.cheryme.top/gtuigsvhsw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtzpbgvctv.html

[S57] C++：编译期常量
来源：http://hz.vqdsnc.cn/gtmfatqxpl.html

constexpr int N = 10;
来源：http://hz.cdnleiting.top/gtylgbbopg.html

[S58] C++：命名空间
来源：http://hz.yj202588.top/gtqrmmdomb.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtokfhmaem.html

[S59] C++：静态断言
来源：http://hz.shuidangran.top/gtbitxofki.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtpjzwndqf.html

[S60] C++：遍历并删除元素
来源：http://hz.birdmap.top/gtsdxxzrhy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.9152youxi.cn/gtpvofuoby.html

================================================================================
来源：http://hz.vqdsnc.cn/gtovkzoqco.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.birdmap.top/gtudzwilko.html

================================================================================
来源：http://hz.jinqigufen.top/gtujyfecyz.html

[T01] Kotlin：Hello World
来源：http://hz.ydjk.org.cn/gtrjyqqcie.html

println("Hello")
来源：http://hz.shzxlz.cn/gtnrhixkgy.html

[T02] Kotlin：变量
来源：http://hz.jinghuilouyu.cn/gtlsnxhkbs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtllhgfqxj.html

[T03] Kotlin：字符串模板
来源：http://hz.jinghuilouyu.cn/gtwdolbtip.html

"值: $b"
来源：http://hz.bjfxy.top/gtoaecxqak.html

[T04] Kotlin：空安全
来源：http://hz.jiagoushi.top/gtjlsicctc.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtdvvaudse.html

[T05] Kotlin：when 表达式
来源：http://hz.sufxvd.cn/gtdkfwvzlr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.meibo888.top/gtqhtahtmo.html

[T06] Kotlin：集合映射
来源：http://hz.zhiwuduotai.top/gtzxfkchnr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hongshengwenyu.top/gtnkbqpigi.html

[T07] Kotlin：集合过滤
来源：http://hz.sweek.top/gtwgvepyfx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pycfn.com/gtezoyjjjb.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gtegmuioef.html

data class User(val name: String, val age: Int)
来源：http://hz.tian-w.cn/gtnafnuwpe.html

[T09] Kotlin：扩展函数
来源：http://hz.aibaodan.cn/gtgpgbojya.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtuzyzoxum.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtxwagjmpw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtdoobeyzl.html

[T11] Kotlin：协程
来源：http://hz.c1oappe.top/gtabgvjnsu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtdambafza.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtinxjucib.html

val (a, b) = Pair(1, 2)
来源：http://hz.9152youxi.cn/gtejrzzveb.html

[T13] Kotlin：只读 Map
来源：http://hz.hnqzz.top/gtxeiqbeia.html

val m = mapOf("a" to 1)
来源：http://hz.aibaodan.cn/gtiqmgnwpw.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gturgploni.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtixlzleun.html

[T15] Kotlin：接口
来源：http://hz.yj202588.top/gtglnjqkut.html

interface Shape { fun area(): Double }
来源：http://hz.hammf.cn/gtluhaiuov.html

[T16] Swift：Hello World
来源：http://hz.ivvv.top/gtzswkrzlm.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtpaewgcey.html

[T17] Swift：变量与常量
来源：http://hz.meibo888.top/gtmecvpfpb.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtthgkhxea.html

[T18] Swift：字符串插值
来源：http://hz.tian-w.cn/gtkzcfsxju.html

"值: \(b)"
来源：http://hz.c1oappe.top/gtayodhukf.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtjhbbwyyn.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtvxdvhboj.html

[T20] Swift：数组操作
来源：http://hz.pycfn.com/gttxruqbrl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtvmvzkkks.html

[T21] Swift：遍历
来源：http://hz.jinqigufen.top/gtgzrmupnb.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtlywdvpku.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtkayolsbs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.tanke756.top/gtykxparhg.html

[T23] Swift：函数
来源：http://hz.0kj1m.cn/gtiunwytos.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yonumen.top/gtjitwnjfp.html

[T24] Swift：闭包
来源：http://hz.9152youxi.cn/gtwowxebrm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.andypj.xyz/gtkvrjinmj.html

[T25] Swift：结构体
来源：http://hz.sweek.top/gtimlkyuus.html

struct P { var x: Int }
来源：http://hz.gotoacloud.top/gtrancziuu.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtywxusgmt.html

class A: Base { override func f() {} }
来源：http://hz.cqqwz.cn/gthzqusdxn.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gtsjpqcysx.html

do { try f() } catch { print(error) }
来源：http://hz.quarkkingdee.top/gttzpyzwff.html

[T28] Swift：枚举
来源：http://hz.shanyushiyangtech.top/gtqbjsusbj.html

enum Color { case red, green }
来源：http://hz.gzhubu.top/gtntzoxcjv.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gtmiawxszg.html

guard let x = opt else { return }
来源：http://hz.gaohongyu789.top/gtxaomupmq.html

[T30] Swift：协议
来源：http://hz.pycfn.com/gtdcefjdle.html

protocol Shape { func area() -> Double }
来源：http://hz.vqdsnc.cn/gtoxyynfjr.html

[T31] Lua：Hello World
来源：http://hz.ydzc1.top/gtzfzxsonn.html

print("Hello")
来源：http://hz.yangfankeji.com/gtlqdysvxi.html

[T32] Lua：局部变量
来源：http://hz.meibo888.top/gtfkrgmwzw.html

local a = 1
来源：http://hz.mhx1999.top/gtzcyclqql.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtlqaazbss.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnxiangtu.top/gtrjykxang.html

[T34] Lua：遍历表
来源：http://hz.zhiwuduotai.top/gtgibyqxqx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sweek.top/gtufbgyqny.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtimccumcr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hysaishi.cn/gtirccljfd.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtidjantlf.html

function add(a, b) return a + b end
来源：http://hz.shuidangran.top/gtfdfwtqjv.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtltiwewwl.html

"a" .. "b"
来源：http://hz.jlsjyb.cn/gtheylbhti.html

[T38] Lua：条件
来源：http://hz.birdmap.top/gtnhknsdol.html

if x > 0 then print("正") end
来源：http://hz.hongshengwenyu.top/gtmwizznje.html

[T39] Lua：模式匹配
来源：http://hz.yongpay.top/gtjlpmtwne.html

string.find(s, "%d+")
来源：http://hz.jqgufenzy.top/gtxbjvzjpz.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtrbhfzira.html

setmetatable({}, { __index = base })
来源：http://hz.ybcxt.top/gtyamzhzjm.html

[T41] Perl：Hello World
来源：http://hz.jinghuilouyu.cn/gtvtxxynxr.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtbuwkjutt.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gtfuetloqw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ybcxt.top/gtleevuwvo.html

[T43] Perl：字符串插值
来源：http://hz.cdnleiting.top/gtdlnbunpg.html

"值: $a"
来源：http://hz.chenzaomai.com/gtjumsceor.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtsaohjjin.html

if ($a > 0) { print "正"; }
来源：http://hz.shzxlz.cn/gtedtsdjpm.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtwttgrbsv.html

for my $x (@arr) { print $x; }
来源：http://hz.gogol.net.cn/gtgkqswzop.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gtfzuaasgg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shuidangran.top/gtnwykvgpd.html

[T47] Perl：正则捕获
来源：http://hz.sweek.top/gtmztvwpin.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gtuymuqazv.html

[T48] Perl：正则替换
来源：http://hz.nanxuanxn.top/gtnkaouebz.html

$s =~ s/old/new/g;
来源：http://hz.yuanzhike.top/gtjkulfuqb.html

[T49] Perl：函数
来源：http://hz.jinghuilouyu.cn/gtsjehqmlc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cdnleiting.top/gtickjvblh.html

[T50] Perl：逐行读文件
来源：http://hz.0kj1m.cn/gtvflpdtny.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtpfwidvnm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinqigfzy.top/gtxbicbzqp.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gtqauagezq.html

println("Hello")
来源：http://hz.daria6918.cn/gtmfasohpk.html

[T52] Scala：变量
来源：http://hz.xziqi.cn/gtnxmiiewq.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gtawiwddro.html

[T53] Scala：字符串插值
来源：http://hz.zhoulong.xyz/gtyjdamuos.html

s"值: $b"
来源：http://hz.wangdashe.top/gtequewihs.html

[T54] Scala：集合映射
来源：http://hz.guowangkeji.top/gtcetpchcp.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhoulong.xyz/gtecxjivcf.html

[T55] Scala：集合过滤
来源：http://hz.ppjwa.cn/gtewatmjcw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ppjwa.cn/gtijxveynl.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtzczzjaxn.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtpidpadqj.html

[T57] Scala：模式匹配
来源：http://hz.ehwqpu.com/gtjjinusaa.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xylfe.cn/gttcwypqqk.html

[T58] Scala：函数定义
来源：http://hz.zhijiandao.cn/gtsuarjuxg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cheryme.top/gthcfkcufu.html

[T59] Scala：循环
来源：http://hz.wangshuangyany.cn/gteytjncwo.html

for (i <- 1 to 10) println(i)
来源：http://hz.ydzc1.top/gtmumsfejo.html

[T60] Scala：折叠
来源：http://hz.fengsongda.top/gtnulygjmq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hammf.cn/gtcfqbcrgd.html

================================================================================
来源：http://hz.sufxvd.cn/gtvedozjjc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ydjk.org.cn/gtkjvddwad.html

================================================================================
来源：http://hz.zhongyouzk.top/gtsirsawkg.html

[U01] Py：创建虚拟环境
来源：http://hz.dashuyun.cn/gtvballdzi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangkeji.top/gtiusfswgc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtstmlsfil.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtjzffxqhl.html

[U03] Py：加载 .env 配置
来源：http://hz.0kj1m.cn/gtjgtstnuh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.chenlongwang.top/gtejrwjuec.html

[U04] Py：变量调试打印
来源：http://hz.xuanzx.com/gtnxubixvr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yanxiufei.cn/gtldrqeowa.html

[U05] Py：列表去重且保序
来源：http://hz.gotoacloud.top/gthnxibegi.html

list(dict.fromkeys(arr))
来源：http://hz.zhengqikj.top/gtutggifuk.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtkjrebnjc.html

{**a, **b}
来源：http://hz.zhiwuduotai.top/gtnidlsosm.html

[U07] Py：反转字典键值
来源：http://hz.xylfe.cn/gteavdlwzj.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtiscwmeya.html

[U08] Py：展平二维列表
来源：http://hz.chenlongwang.top/gtrdqokeae.html

[y for x in nested for y in x]
来源：http://hz.meibo888.top/gtftcdlfoi.html

[U09] Py：字典取最大值的键
来源：http://hz.aibaodan.cn/gtvpwmyocf.html

max(d, key=d.get)
来源：http://hz.jqgfzy.top/gtcdielrxj.html

[U10] Py：按值排序字典
来源：http://hz.kuanghao11.cn/gtwuwaomwl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sufxvd.cn/gtcurksibi.html

[U11] Py：生成器表达式
来源：http://hz.fzhhl.top/gtqpzgkyjr.html

(x * 2 for x in arr)
来源：http://hz.chenjidiqi.icu/gtouotkvin.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.fzhhl.top/gthquxdcxg.html

Counter(arr).most_common(3)
来源：http://hz.sufxvd.cn/gttqvvypoh.html


<!-- 参考信息 -->