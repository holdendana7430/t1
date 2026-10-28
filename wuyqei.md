代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tanke756.top/gtghofzerj.html

[S02] C：变量与格式化输出
来源：http://hz.havefunace.top/gtqongfruf.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtoeduesek.html

[S03] C：读入整数
来源：http://hz.svipenyu.cn/gtmjywvbel.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtwchbdwyw.html

[S04] C：字符串复制
来源：http://hz.zycfv.cn/gtaozlmqum.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shuidangran.top/gtexyjepiv.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtobercwsh.html

strlen(s)
来源：http://hz.zhaomingkeji.xyz/gtqzqslszy.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtlnografq.html

strcmp(a, b) == 0
来源：http://hz.aizwys.cn/gtiuumjldu.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gtpyczvdhy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sweek.top/gtphigrowo.html

[S08] C：动态内存分配与释放
来源：http://hz.dashuyun.cn/gtrvvjexiy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.xuetiantiany.cn/gtsboamgbu.html

[S09] C：结构体定义与初始化
来源：http://hz.52xcode.cn/gtrdpxwjje.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj202588.top/gtyhueyicl.html

[S10] C：指针与解引用
来源：http://hz.daria6918.cn/gtcjnwkaez.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtllrymhkr.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtwwmiqbqh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtyndrfngu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigufen.top/gtgdwoqdey.html

fclose(f);
来源：http://hz.tianlin.xyz/gtefmhguok.html

[S12] C：写文件
来源：http://hz.nwbrower.top/gtyiiqsldd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.bjfxy.top/gtaitjhsfu.html

[S13] C：宏定义
来源：http://hz.hywenlv.cn/gtebsucmoc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.316326.xyz/gtwochsvdp.html

[S14] C：枚举
来源：http://hz.wangdashe.top/gtfymffcgd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.meibo888.top/gtllyxghwj.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtlhgtdkvl.html

(double) a / b
来源：http://hz.tian-w.cn/gtlucafdxs.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtnzllupyq.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtwshzvlst.html

[S17] C：安全拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtjskogscr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxuanxn.top/gtxayabanf.html

[S18] C：命令行参数
来源：http://hz.zhengqikj.top/gtklcicurb.html

int main(int argc, char **argv)
来源：http://hz.sweek.top/gtefkjwvbt.html

[S19] C：快速排序
来源：http://hz.feifeiyinyue.top/gtjuvssdpu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtmbqfdyyp.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtqjcyaukf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtirzdqfqa.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtcivkfdxr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yongpay.top/gtwozpsqto.html

[S22] C：字符串转数字
来源：http://hz.jqgufenzy.top/gtzkujeyiq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuanzx.com/gtytzdzkgq.html

[S23] C：随机数
来源：http://hz.gotoacloud.top/gtodtlemsy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gtgyzmxodb.html

[S24] C：获取本地时间
来源：http://hz.shzxlz.cn/gtwgmkfrjg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tian-w.cn/gtdchzbqby.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtvrljnfpa.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtmvtnpzvh.html

[S26] C：内存清零
来源：http://hz.aizwys.cn/gtwxqcvcuo.html

memset(a, 0, sizeof a);
来源：http://hz.vqdsnc.cn/gtmhzfugut.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gtigooplsz.html

const double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtjvymmonu.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtpgttkztx.html

static int counter = 0;
来源：http://hz.dianchejie.cn/gtezjpifws.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtnhaybfrf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jqgfzy.top/gtzrlcqamh.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtwllaufly.html

#ifndef X_H
来源：http://hz.daxiang520.top/gtgsaqdgqm.html

#define X_H
来源：http://hz.zhixingplan.top/gtxvpvwfsf.html

#endif
来源：http://hz.zhongyouzk.top/gtpyulhixz.html

[S31] C++：Hello World
来源：http://hz.snrcjt.cn/gtpcmlmlsm.html

#include <iostream>
来源：http://hz.cqqwz.cn/gtjcxoypas.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aizwys.cn/gtowetjvxg.html

[S32] C++：字符串
来源：http://hz.chenjidiqi.icu/gtqjewkbob.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gtrkoqalhu.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtrxrprpfu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tianlin.xyz/gtbpyocahg.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtftiyhzqi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtxgogvskf.html

[S35] C++：map
来源：http://hz.zycfv.cn/gtdbjranvl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtwxzfhdpx.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtmhxnkmov.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtekfdviir.html

[S37] C++：set
来源：http://hz.hywenlv.cn/gtvobpduyt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gttybdnvwk.html

[S38] C++：排序
来源：http://hz.haohaochexian.top/gtboxcxjdn.html

std::sort(v.begin(), v.end());
来源：http://hz.ppjwa.cn/gtweripalm.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtdvrorsik.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gttzvhztie.html

[S40] C++：查找元素
来源：http://hz.jinqigufen.top/gtxtikzkcm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtsreiucwv.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtgagcggwp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.gogol.net.cn/gtxsvzrafm.html

[S42] C++：继承与虚函数
来源：http://hz.jiagoushi.top/gtjgtlhgff.html

class B : public Base { public: void f() override {} };
来源：http://hz.sufxvd.cn/gtoidltvoh.html

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gtewhipnzo.html

auto p = std::make_unique<int>(5);
来源：http://hz.jyoumei.cn/gtjefdyhpg.html

[S44] C++：引用传参
来源：http://hz.jianghu66.top/gtaymfixnh.html

void inc(int &x) { ++x; }
来源：http://hz.birdmap.top/gticclvyhz.html

[S45] C++：lambda
来源：http://hz.xinyue.icu/gtrjsgysgb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fengsongda.top/gtmveelrmo.html

[S46] C++：函数模板
来源：http://hz.tanke756.top/gtthhgzbso.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtavjecqyo.html

[S47] C++：结构化绑定遍历
来源：http://hz.aibaodan.cn/gtxufeqmma.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zycfv.cn/gtxiklgkxy.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtgriyvknq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtcwknxuih.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gtbabgqxal.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtbzhgxeck.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cheryme.top/gteijvpkqn.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtcidhtkqa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtvfusuybx.html

[S51] C++：显式类型转换
来源：http://hz.xinyue.icu/gtwqtdunjh.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gtktbquuxt.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gthcfguuih.html

int size() const noexcept { return n_; }
来源：http://hz.svipenyu.cn/gtskpxcxos.html

[S53] C++：移动语义
来源：http://hz.guowangkeji.top/gtqxzzvglc.html

std::vector<int> w = std::move(v);
来源：http://hz.aibaodan.cn/gtcrkvvqkz.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtcabwewqw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yangfankeji.com/gtbfdroozk.html

[S55] C++：结构化绑定
来源：http://hz.iojbl.cn/gtpctvhvpq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtvlzpwltu.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gtqthbrnfv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtxyxpbxjx.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtebrsxchb.html

constexpr int N = 10;
来源：http://hz.vqdsnc.cn/gteijawwsq.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtzpcmgxwq.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtewaxackz.html

[S59] C++：静态断言
来源：http://hz.ivvv.top/gtqovghezx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daria6918.cn/gtyccbspmj.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gtrqqduxbz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gtoxchhmyq.html

================================================================================
来源：http://hz.haohaochexian.top/gtuqdzydii.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gtafcwgtde.html

================================================================================
来源：http://hz.aibaodan.cn/gtnkteuloc.html

[T01] Kotlin：Hello World
来源：http://hz.zdqjudy.top/gtplugkbud.html

println("Hello")
来源：http://hz.hywenlv.cn/gtizlquhcu.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtptomkwvi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gotoacloud.top/gtsahirvkn.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtzsfzxlsa.html

"值: $b"
来源：http://hz.sweek.top/gtvjairxut.html

[T04] Kotlin：空安全
来源：http://hz.gotoacloud.top/gthenwyton.html

val n: String? = null;  n?.length
来源：http://hz.jinqigfzy.top/gtcgwglogw.html

[T05] Kotlin：when 表达式
来源：http://hz.gaohongyu789.top/gtfqjyecny.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgufenzy.top/gtyhjthdea.html

[T06] Kotlin：集合映射
来源：http://hz.bjfxy.top/gtrqexptrv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aizwys.cn/gtgwesbngi.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtxgrlnrux.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhaomingkeji.xyz/gtqnjlfmfo.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtmriabyly.html

data class User(val name: String, val age: Int)
来源：http://hz.feifeiyinyue.top/gtprwgrjdb.html

[T09] Kotlin：扩展函数
来源：http://hz.pycfn.com/gtvzwogvxx.html

fun String.exclaim() = this + "!"
来源：http://hz.yuxming.cn/gtctkdxojm.html

[T10] Kotlin：默认参数
来源：http://hz.hfpthk.cn/gtpavybpom.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gtalrfpffb.html

[T11] Kotlin：协程
来源：http://hz.hammf.cn/gtisuyrusb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.havefunace.top/gtibsozooc.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtgdybvcco.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj202588.top/gttggavqpk.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxuanxn.top/gtwxfdmznj.html

val m = mapOf("a" to 1)
来源：http://hz.zhiwuduotai.top/gtmtarfntr.html

[T14] Kotlin：循环
来源：http://hz.yanxiufei.cn/gtqzjbcmnq.html

for (i in 1..10) println(i)
来源：http://hz.sxryk.cn/gtsjubetyj.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtyhwcjvwg.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtxszztbjm.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtqjpomtdz.html

print("Hello")
来源：http://hz.zycfv.cn/gtcsgitqgq.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gthztpckhk.html

var a = 1;  let b = 2
来源：http://hz.meibo888.top/gthnyusupg.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtepsrjbtt.html

"值: \(b)"
来源：http://hz.hfpthk.cn/gtsiigwczc.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtncrwsmxt.html

if let n = opt { print(n) }
来源：http://hz.birdmap.top/gtttebitrb.html

[T20] Swift：数组操作
来源：http://hz.kuanghao11.cn/gtvzvywhes.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gtljpofdre.html

[T21] Swift：遍历
来源：http://hz.jinqigfzy.top/gtpdwxmcsu.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtjhwoqtla.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtqhceczjn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gtnvteokyk.html

[T23] Swift：函数
来源：http://hz.shanyushiyangtech.top/gtdxuvllxf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtifjwvnit.html

[T24] Swift：闭包
来源：http://hz.0kj1m.cn/gtngzuvvad.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hysaishi.cn/gtrgcapkzc.html

[T25] Swift：结构体
来源：http://hz.feifeiyinyue.top/gtklxybqak.html

struct P { var x: Int }
来源：http://hz.yuanzhike.top/gttscdefus.html

[T26] Swift：类与重写
来源：http://hz.daria6918.cn/gtikvpecwl.html

class A: Base { override func f() {} }
来源：http://hz.havefunace.top/gtfyjtqzzk.html

[T27] Swift：错误处理
来源：http://hz.svipenyu.cn/gthvhrcvda.html

do { try f() } catch { print(error) }
来源：http://hz.zdqjudy.top/gtgznbxblh.html

[T28] Swift：枚举
来源：http://hz.guannengcc.top/gtxengbzwm.html

enum Color { case red, green }
来源：http://hz.zhaomingkeji.xyz/gtqyprnukz.html

[T29] Swift：guard 提前返回
来源：http://hz.guowangkeji.top/gtmylpsuec.html

guard let x = opt else { return }
来源：http://hz.hfpthk.cn/gthmfohqye.html

[T30] Swift：协议
来源：http://hz.ywan-chungtsiang.top/gtscjrnjpb.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtunzeqmug.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtcywbarqk.html

print("Hello")
来源：http://hz.chenzaomai.com/gtfdzyeqvm.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangtech.top/gtvrfquieb.html

local a = 1
来源：http://hz.bjfxy.top/gtgercgurt.html

[T33] Lua：表（数组）
来源：http://hz.feifeiyinyue.top/gtcsfsxhnj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtvqvkjnan.html

[T34] Lua：遍历表
来源：http://hz.nanxuanxn.top/gtxxxsfupa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtndidwgso.html

[T35] Lua：字典表
来源：http://hz.chenzaomai.com/gtsthdswrd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtpipbtppe.html

[T36] Lua：函数
来源：http://hz.jlsjyb.cn/gttcijgxfw.html

function add(a, b) return a + b end
来源：http://hz.cqqwz.cn/gtxljdznnn.html

[T37] Lua：字符串拼接
来源：http://hz.andypj.xyz/gtfxuztmdy.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtzumwefga.html

[T38] Lua：条件
来源：http://hz.52xcode.cn/gtyjngdqjh.html

if x > 0 then print("正") end
来源：http://hz.guowangkeji.top/gtaurnpzsu.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangtech.top/gttpxybhip.html

string.find(s, "%d+")
来源：http://hz.nanxuanxn.top/gtczqauwud.html

[T40] Lua：元表
来源：http://hz.havefunace.top/gtmjuauuaj.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtjokvrhlx.html

[T41] Perl：Hello World
来源：http://hz.yueranfly.top/gtgpaecsco.html

print "Hello\n";
来源：http://hz.xingfuxueyuan.xyz/gtcnjavtii.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtajdzousz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258.top/gtxqdhotqx.html

[T43] Perl：字符串插值
来源：http://hz.hfpthk.cn/gtaxxwhlbh.html

"值: $a"
来源：http://hz.havefunace.top/gtxrhltszh.html

[T44] Perl：条件
来源：http://hz.havefunace.top/gttktteidm.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtnvcvyrdx.html

[T45] Perl：数组遍历
来源：http://hz.chenlongwang.top/gttdgbwatk.html

for my $x (@arr) { print $x; }
来源：http://hz.chenlongwang.top/gtjxmpreah.html

[T46] Perl：哈希操作
来源：http://hz.52xcode.cn/gtreqjtspn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xylfe.cn/gtpgitxgiy.html

[T47] Perl：正则捕获
来源：http://hz.jianghu66.top/gtgkhmelnp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtlujbchev.html

[T48] Perl：正则替换
来源：http://hz.wangdashe.top/gteiurxdar.html

$s =~ s/old/new/g;
来源：http://hz.jinyuanbaomall.cn/gtlgjeaiuu.html

[T49] Perl：函数
来源：http://hz.yj202588.top/gtzhhqekxe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tian-w.cn/gtrgozobnw.html

[T50] Perl：逐行读文件
来源：http://hz.yongpay.top/gteesnlfwk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtbpuodvhf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ywan-chungtsiang.top/gtbhevcjof.html

[T51] Scala：Hello World
来源：http://hz.chenlongwang.top/gtwuiyuoft.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtcppwcerh.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtpokzyike.html

val a = 1;  var b = 2
来源：http://hz.yongpay.top/gteqdnqjoo.html

[T53] Scala：字符串插值
来源：http://hz.haohaochexian.top/gtixfzfsas.html

s"值: $b"
来源：http://hz.tianlin.xyz/gtyaweuors.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtlibnzcns.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuanzx.com/gtqtscujac.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtigtfdscq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gttshmfsuv.html

[T56] Scala：样例类
来源：http://hz.wangshuangyany.cn/gtbrounoac.html

case class User(name: String, age: Int)
来源：http://hz.shanyushiyangkeji.top/gtyagtyevc.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtgfzwzpaf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtzyacpnjv.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtdpavguxt.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.9152youxi.cn/gtgaifxykt.html

[T59] Scala：循环
来源：http://hz.jyoumei.cn/gtnwtjrjxx.html

for (i <- 1 to 10) println(i)
来源：http://hz.cqqwz.cn/gtsvmspoha.html

[T60] Scala：折叠
来源：http://hz.jinyuanbaomall.cn/gtixlvqkmz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.kuanghao11.cn/gtkbnlckwb.html

================================================================================
来源：http://hz.hammf.cn/gtpcyhcyis.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenjidiqi.icu/gtwigoakjz.html

================================================================================
来源：http://hz.chenzaomai.com/gtsdqdeiao.html

[U01] Py：创建虚拟环境
来源：http://hz.redwolf501.top/gtccrwyllz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yueranfly.top/gtfcaijnxg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtzgvuyfgq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenjidiqi.icu/gtwhlsibqc.html

[U03] Py：加载 .env 配置
来源：http://hz.jqgufenzy.top/gtbyyzyazr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sysykeji.top/gtvkdovdyi.html

[U04] Py：变量调试打印
来源：http://hz.guannengcc.top/gtkxvvwumh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.feifeiyinyue.top/gtpmgstgwg.html

[U05] Py：列表去重且保序
来源：http://hz.yj202588.top/gtbttxbjtf.html

list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtosrucule.html

[U06] Py：合并两个字典
来源：http://hz.zhengqikj.top/gtirmaguid.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtyqzfnuwv.html

[U07] Py：反转字典键值
来源：http://hz.hfpthk.cn/gtzlrjnlpd.html

{v: k for k, v in d.items()}
来源：http://hz.redwolf501.top/gtmmtfvntz.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtktjvqfaz.html

[y for x in nested for y in x]
来源：http://hz.yangfankeji.com/gtklmonohk.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258888.top/gtiktsnlzb.html

max(d, key=d.get)
来源：http://hz.52xcode.cn/gtjjyvgcvw.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gtnmdjbjlb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ppjwa.cn/gtcetdfkwl.html

[U11] Py：生成器表达式
来源：http://hz.yj202588.top/gtypqioxrq.html

(x * 2 for x in arr)
来源：http://hz.havefunace.top/gtpkeetcmw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sxryk.cn/gthnzgefbz.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtpakuuyey.html

[U13] Py：固定长度队列
来源：http://hz.zhijiandao.cn/gtbzxndsux.html

deque(maxlen=10)
来源：http://hz.tianlin.xyz/gtkowwtkmt.html

[U14] Py：分组收集到列表
来源：http://hz.dashuyun.cn/gtcnhcabfu.html

defaultdict(list)
来源：http://hz.ydjk.org.cn/gtuejqfxzb.html

[U15] Py：高精度计时
来源：http://hz.zhoulong.xyz/gtkigqytil.html

t = time.perf_counter()
来源：http://hz.sweek.top/gtdhegvlsj.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangkeji.top/gtgmiqszzk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuanzx.com/gtcwoujlca.html

[U17] Py：初始化日志
来源：http://hz.pengpengdd.cyou/gtsqjfdlkg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yangfankeji.com/gtbdisvsbc.html

[U18] Py：预编译正则
来源：http://hz.wangshuangyany.cn/gtdcofdjyi.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtjfswuzzh.html

[U19] Py：正则替换带回调
来源：http://hz.yanxiufei.cn/gtomustsew.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sysykeji.top/gtzkgiedsv.html

[U20] Py：缓存函数结果
来源：http://hz.smart0.xyz/gtrftataco.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cheryme.top/gtnapzeovd.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnxiangtu.top/gtydkgxkpx.html

@contextlib.contextmanager
来源：http://hz.aizwys.cn/gtiyenjeta.html

[U22] Py：矩阵转置
来源：http://hz.mhx1999.top/gtfkoqfzqd.html

list(zip(*m))
来源：http://hz.52xcode.cn/gteprlurcw.html

[U23] Py：分块读取大文件
来源：http://hz.haohaochexian.top/gtvbyaafdc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fzhhl.top/gtddekkfoo.html

[U24] Py：路径操作
来源：http://hz.jinyuanbaomall.cn/gtverkwnoh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuanzhike.top/gtffnhvcjt.html


<!-- 参考信息 -->