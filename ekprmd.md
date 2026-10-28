代发 wailian999

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gtdwkkvecv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.bjfxy.top/gtvipxtzfj.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gtdfzsouhe.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgfzy.top/gtftkjmxub.html

[S35] C++：map
来源：http://hz.nanxuanxn.top/gtuycsqeoz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtuycsdfmz.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gticfhkhnr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtdqoopatn.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtxrnhencv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cheryme.top/gtbjsxrzuu.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtzafjrkcr.html

std::sort(v.begin(), v.end());
来源：http://hz.daxiang520.top/gtlybhcjyh.html

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gtkjgduncu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sxryk.cn/gtncmezrho.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtzljcadts.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.wangdashe.top/gtvyrcwabr.html

[S41] C++：类与构造函数
来源：http://hz.smart0.xyz/gtchhlfvdz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daxiang520.top/gtotbfhiih.html

[S42] C++：继承与虚函数
来源：http://hz.sxryk.cn/gtneswjkht.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtnpsizvvn.html

[S43] C++：智能指针
来源：http://hz.daxiang520.top/gtgasdmvce.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gtoamrhiib.html

[S44] C++：引用传参
来源：http://hz.svipenyu.cn/gtjvjjhint.html

void inc(int &x) { ++x; }
来源：http://hz.shuidangran.top/gtzotmqrri.html

[S45] C++：lambda
来源：http://hz.nanxuanxn.top/gtgldcvdjo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yongpay.top/gtdhmltsev.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtyiblyfjn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtrjyaiaje.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigfzy.top/gtcqyybxsr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgfzy.top/gtjnylcmfj.html

[S48] C++：逐行读文件
来源：http://hz.yj202588.top/gtqvsfajyy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.redwolf501.top/gtqbgnnqcf.html

while (std::getline(in, line)) { }
来源：http://hz.ydjk.org.cn/gtvvhlufnm.html

[S49] C++：写文件
来源：http://hz.cqqwz.cn/gtouekegho.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinyuanbaomall.cn/gtqwnnbidg.html

[S50] C++：格式化数字
来源：http://hz.hammf.cn/gtjspovzmr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtbjiyitwx.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gttvltdtyz.html

static_cast<double>(a) / b
来源：http://hz.yuanzhike.top/gtefdezyqg.html

[S52] C++：const 与 noexcept
来源：http://hz.dashuyun.cn/gtfuwszfvm.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtdmmshreo.html

[S53] C++：移动语义
来源：http://hz.yvedp.cn/gtwlfssskr.html

std::vector<int> w = std::move(v);
来源：http://hz.sysykeji.top/gtyvpnpxam.html

[S54] C++：异常处理
来源：http://hz.kuanghao11.cn/gtjpksvlmv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtqqvwxxhj.html

[S55] C++：结构化绑定
来源：http://hz.cucudq.cn/gtaxljvyrz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuanzhike.top/gtrrttvlcp.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtqgvyycuk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gtelbtzzyg.html

[S57] C++：编译期常量
来源：http://hz.gotoacloud.top/gtzmgqazse.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtavegxlrw.html

[S58] C++：命名空间
来源：http://hz.wangshuangyany.cn/gtszzwrwiy.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtlhojnokx.html

[S59] C++：静态断言
来源：http://hz.9152youxi.cn/gtqgzzlbuz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gtxselqwik.html

[S60] C++：遍历并删除元素
来源：http://hz.iojbl.cn/gtvzrfrnkj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guowangkeji.top/gtndmfzwoe.html

================================================================================
来源：http://hz.ehwqpu.com/gtthwxmauq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.mhx1999.top/gtulzugrck.html

================================================================================
来源：http://hz.jianghu66.top/gtowkdeybj.html

[T01] Kotlin：Hello World
来源：http://hz.wangshuangyany.cn/gtqkjumcoe.html

println("Hello")
来源：http://hz.dashuyun.cn/gtjwqfkfgo.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gttlyyfwle.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhengqikj.top/gtacxfypml.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gtqggbcbzq.html

"值: $b"
来源：http://hz.jqgfzy.top/gtshznynbk.html

[T04] Kotlin：空安全
来源：http://hz.yuxming.cn/gtxgoshfzh.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gthpcoqoyt.html

[T05] Kotlin：when 表达式
来源：http://hz.hywenlv.cn/gtbwjlqpzc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtybeccpbj.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtbyqavoxq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.iojbl.cn/gtaqzlvksq.html

[T07] Kotlin：集合过滤
来源：http://hz.tianlin.xyz/gtcftgunou.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtmohglppl.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gthsevudhz.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangkeji.top/gtfesnuukn.html

[T09] Kotlin：扩展函数
来源：http://hz.aizwys.cn/gtsryoxmdb.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtpsflolkp.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigfzy.top/gthgykbfbc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhiwuduotai.top/gtsspdbfru.html

[T11] Kotlin：协程
来源：http://hz.fzhhl.top/gturtsbepy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.havefunace.top/gtnpqqxogc.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangkeji.top/gtdqkwvvlw.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtlmhlaybm.html

[T13] Kotlin：只读 Map
来源：http://hz.hammf.cn/gtmkmfrhqy.html

val m = mapOf("a" to 1)
来源：http://hz.jinyuanbaomall.cn/gtlhrmkjzl.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtpkpswofi.html

for (i in 1..10) println(i)
来源：http://hz.wangdashe.top/gttcwxwhbr.html

[T15] Kotlin：接口
来源：http://hz.tian-w.cn/gtrrugcwhg.html

interface Shape { fun area(): Double }
来源：http://hz.xuetiantiany.cn/gtemekusyd.html

[T16] Swift：Hello World
来源：http://hz.tianlin.xyz/gtyzqrnuil.html

print("Hello")
来源：http://hz.smart0.xyz/gtvsvpohhf.html

[T17] Swift：变量与常量
来源：http://hz.mhx1999.top/gtelwxxxtt.html

var a = 1;  let b = 2
来源：http://hz.bjfxy.top/gtoxqddedd.html

[T18] Swift：字符串插值
来源：http://hz.gotoacloud.top/gtwupjqyry.html

"值: \(b)"
来源：http://hz.sxryk.cn/gtyxnofeeg.html

[T19] Swift：可选绑定
来源：http://hz.quarkkingdee.top/gtxsiivkqu.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gtqjwsvlfm.html

[T20] Swift：数组操作
来源：http://hz.yj20258.top/gtdwjcwcjs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtbjmcumfc.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtfrktcvwo.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtqzawbtgu.html

[T22] Swift：字典
来源：http://hz.jinqigfzy.top/gtkapnfvvz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinghuilouyu.cn/gttqajrcjn.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gtovjmoyom.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yuxming.cn/gtijtbcuyc.html

[T24] Swift：闭包
来源：http://hz.guannengcc.top/gthtdpzlgp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtwijchhxn.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gteeirrdtf.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gttbeosyyb.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtbykqjuxt.html

class A: Base { override func f() {} }
来源：http://hz.gogol.net.cn/gtdbcxfedu.html

[T27] Swift：错误处理
来源：http://hz.chenlongwang.top/gtekozdbvq.html

do { try f() } catch { print(error) }
来源：http://hz.andypj.xyz/gtjkhmunax.html

[T28] Swift：枚举
来源：http://hz.shuidangran.top/gtlnyvleqb.html

enum Color { case red, green }
来源：http://hz.yongpay.top/gtdjiisgae.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtluflctoo.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gtixogicio.html

[T30] Swift：协议
来源：http://hz.birdmap.top/gtrrzywwuy.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxuanxn.top/gtzlatvbcm.html

[T31] Lua：Hello World
来源：http://hz.zhengqikj.top/gtdtffjrxx.html

print("Hello")
来源：http://hz.hammf.cn/gtfhyrtmgg.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtoypxpthu.html

local a = 1
来源：http://hz.chenlongwang.top/gtnkbxibcr.html

[T33] Lua：表（数组）
来源：http://hz.svipenyu.cn/gtezqwfluz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.pengpengdd.cyou/gtsymdgllj.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtplnquhvs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shuidangran.top/gtpmvgcpbs.html

[T35] Lua：字典表
来源：http://hz.hysaishi.cn/gtwengrpjg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtxswflgjq.html

[T36] Lua：函数
来源：http://hz.yanxiufei.cn/gtlhryjddi.html

function add(a, b) return a + b end
来源：http://hz.yanxiufei.cn/gtdexmcjkb.html

[T37] Lua：字符串拼接
来源：http://hz.jianghu66.top/gtpzqpklsh.html

"a" .. "b"
来源：http://hz.cdnleiting.top/gtgzsssbll.html

[T38] Lua：条件
来源：http://hz.tanke756.top/gtccmdeknf.html

if x > 0 then print("正") end
来源：http://hz.yj202588.top/gttwrnqkuf.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtjleudldb.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtpdgfjgqs.html

[T40] Lua：元表
来源：http://hz.bjfxy.top/gtrpcwrpix.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258888.top/gtwbptnpjb.html

[T41] Perl：Hello World
来源：http://hz.xinyue.icu/gtfualkikq.html

print "Hello\n";
来源：http://hz.andypj.xyz/gtqnbtmjwz.html

[T42] Perl：变量类型
来源：http://hz.ywan-chungtsiang.top/gthauiqyve.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.mhx1999.top/gtfbabpxwv.html

[T43] Perl：字符串插值
来源：http://hz.smart0.xyz/gtmfnmkytt.html

"值: $a"
来源：http://hz.zhiwuduotai.top/gtlchxdlgu.html

[T44] Perl：条件
来源：http://hz.tanke756.top/gtxqfkxiba.html

if ($a > 0) { print "正"; }
来源：http://hz.c1oappe.top/gtyascqane.html

[T45] Perl：数组遍历
来源：http://hz.zhixingplan.top/gtxeizgxat.html

for my $x (@arr) { print $x; }
来源：http://hz.shangyingyoupin.top/gtrqbanccs.html

[T46] Perl：哈希操作
来源：http://hz.xingfuxueyuan.xyz/gthzmotsql.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gzhubu.top/gtpymlpczx.html

[T47] Perl：正则捕获
来源：http://hz.ivvv.top/gtpwlhoxpy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.haohaochexian.top/gtkeldvypj.html

[T48] Perl：正则替换
来源：http://hz.sweek.top/gtakiiibpg.html

$s =~ s/old/new/g;
来源：http://hz.yonumen.top/gtyvjsypra.html

[T49] Perl：函数
来源：http://hz.vqdsnc.cn/gtkoxrotmd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtvslicyoc.html

[T50] Perl：逐行读文件
来源：http://hz.yuanzhike.top/gtmojeivhh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.kuanghao11.cn/gtqjsvmgih.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinyuanbaomall.cn/gtjierxyei.html

[T51] Scala：Hello World
来源：http://hz.ybcxt.top/gtgwkzfbbd.html

println("Hello")
来源：http://hz.shuidangran.top/gtucelvxkf.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtodlfcjyq.html

val a = 1;  var b = 2
来源：http://hz.cheryme.top/gtjbxhvyxl.html

[T53] Scala：字符串插值
来源：http://hz.sweek.top/gtwcuguvvo.html

s"值: $b"
来源：http://hz.yuanzhike.top/gtotetcaek.html

[T54] Scala：集合映射
来源：http://hz.sweek.top/gtpacjhrls.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenlongwang.top/gtklygbrwv.html

[T55] Scala：集合过滤
来源：http://hz.havefunace.top/gtzmblamtg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj202588.top/gtkeziunhr.html

[T56] Scala：样例类
来源：http://hz.yangfankeji.com/gtmokmccny.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gthnppfhnk.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtwbijndbk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gttnariokl.html

[T58] Scala：函数定义
来源：http://hz.sufxvd.cn/gtavmjwugk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtxcqgswof.html

[T59] Scala：循环
来源：http://hz.shanyushiyangtech.top/gtlpklwarg.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtqczexxyn.html

[T60] Scala：折叠
来源：http://hz.ybcxt.top/gtaylpmlzw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.pengpengdd.cyou/gtltiltidl.html

================================================================================
来源：http://hz.yongpay.top/gtyidelpjr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtylfquyfi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtafuyjrrf.html

[U01] Py：创建虚拟环境
来源：http://hz.tanke756.top/gtwkgmrezf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sweek.top/gtfwlqoywt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yonumen.top/gtaeevqzlf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtsmxdmzje.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtlvtjsvwa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tianlin.xyz/gtmtvjqxsz.html

[U04] Py：变量调试打印
来源：http://hz.52xcode.cn/gtlyzjryzb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.kuanghao11.cn/gtmosunluk.html

[U05] Py：列表去重且保序
来源：http://hz.havefunace.top/gtgrgzibox.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gthenwxsto.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gtfjpcxqab.html

{**a, **b}
来源：http://hz.cdnleiting.top/gticxyjphr.html

[U07] Py：反转字典键值
来源：http://hz.yongpay.top/gthbflvyiw.html

{v: k for k, v in d.items()}
来源：http://hz.jyoumei.cn/gtdeujibfq.html

[U08] Py：展平二维列表
来源：http://hz.xziqi.cn/gtprdfyswe.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gtasiqvnfz.html

[U09] Py：字典取最大值的键
来源：http://hz.hongshengwenyu.top/gtqqueyufd.html

max(d, key=d.get)
来源：http://hz.dashuyun.cn/gtrougtyvu.html

[U10] Py：按值排序字典
来源：http://hz.jinqigufen.top/gtfxcsugaq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tian-w.cn/gtrqdrfkns.html

[U11] Py：生成器表达式
来源：http://hz.vqdsnc.cn/gtayfvwjdk.html

(x * 2 for x in arr)
来源：http://hz.jinghuilouyu.cn/gttubpmgpa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daria6918.cn/gtuenjodfz.html

Counter(arr).most_common(3)
来源：http://hz.jqgufenzy.top/gtpnecemhk.html

[U13] Py：固定长度队列
来源：http://hz.quarkkingdee.top/gtanrwibmd.html

deque(maxlen=10)
来源：http://hz.haohaochexian.top/gtiahuwdqv.html

[U14] Py：分组收集到列表
来源：http://hz.haohaochexian.top/gtmgumyqhj.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtlcigcipa.html

[U15] Py：高精度计时
来源：http://hz.guowangkeji.top/gtylpxilwh.html

t = time.perf_counter()
来源：http://hz.cucudq.cn/gtadhxwupu.html

[U16] Py：命令行参数解析
来源：http://hz.quarkkingdee.top/gttlywutfv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aibaodan.cn/gtxyatszvo.html

[U17] Py：初始化日志
来源：http://hz.xuetiantiany.cn/gtyzfybcqz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ppjwa.cn/gthhgpugfw.html

[U18] Py：预编译正则
来源：http://hz.nwbrower.top/gtnozplcxu.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gttctqzcgo.html

[U19] Py：正则替换带回调
来源：http://hz.shanyushiyangtech.top/gtdxxssyca.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.haohaochexian.top/gtjzpvxxxz.html

[U20] Py：缓存函数结果
来源：http://hz.ppjwa.cn/gtuolorgma.html

@functools.lru_cache(maxsize=None)
来源：http://hz.andypj.xyz/gtmzrkrayc.html

[U21] Py：自定义上下文管理器
来源：http://hz.xylfe.cn/gtvgdjsfgn.html

@contextlib.contextmanager
来源：http://hz.zhijiandao.cn/gtecayurue.html

[U22] Py：矩阵转置
来源：http://hz.52xcode.cn/gtzlpaydyz.html

list(zip(*m))
来源：http://hz.vqdsnc.cn/gttqcnadfh.html

[U23] Py：分块读取大文件
来源：http://hz.ivvv.top/gtyxxathbe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yvedp.cn/gtqunoqmit.html

[U24] Py：路径操作
来源：http://hz.dashuyun.cn/gtsvlljexl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtkpssjfpr.html

[U25] Py：CSV 按字典读
来源：http://hz.yueranfly.top/gtdlzjhjql.html

csv.DictReader(f)
来源：http://hz.cqqwz.cn/gtatlmsqqh.html

[U26] Py：并发下载
来源：http://hz.jinyuanbaomall.cn/gttungcbsg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sxryk.cn/gtzbysvvcs.html

[U27] Py：异步 HTTP
来源：http://hz.jyoumei.cn/gtgdtfyppx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinghuilouyu.cn/gtnbmarlbv.html

[U28] Py：类型别名
来源：http://hz.pycfn.com/gteznbztsx.html

UserId = int
来源：http://hz.dianchejie.cn/gtytixtwck.html

[U29] Py：属性校验
来源：http://hz.smart0.xyz/gtijivefwc.html

@property 与 @x.setter 配合
来源：http://hz.wangshuangyany.cn/gtlicmodtv.html

[U30] Py：数据类
来源：http://hz.chenjidiqi.icu/gtxwuldepz.html

@dataclass(slots=True)
来源：http://hz.ybcxt.top/gtmrjpvnpr.html

[U31] Py：单测
来源：http://hz.0kj1m.cn/gtvrvbjdxm.html

python -m pytest -q
来源：http://hz.xziqi.cn/gtkkjcoxbg.html

[U32] Py：代码格式化
来源：http://hz.jinghuilouyu.cn/gtwjbbnlqf.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtwvdlsvku.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtivhrypgn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gogol.net.cn/gtnhfuhjra.html

[U34] Py：判断编码
来源：http://hz.sufxvd.cn/gtgpdbcaim.html

chardet.detect(raw)
来源：http://hz.jqgfzy.top/gtraidsank.html

[U35] Py：发送邮件
来源：http://hz.snrcjt.cn/gtboslccrn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yueranfly.top/gtamcqfayv.html

[U36] Py：定时任务
来源：http://hz.gaohongyu789.top/gtibxpzgbs.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtfbcdthzp.html

[U37] Py：读写 Excel
来源：http://hz.xziqi.cn/gtxulstoiy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.9152youxi.cn/gtuewnhhmk.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhoulong.xyz/gtilkugfgn.html

Path(__file__).resolve().parent
来源：http://hz.yj20258888.top/gtesirzabq.html

[U39] Py：判断是否在交互环境
来源：http://hz.wangshuangyany.cn/gthmukxnwl.html

sys.stdout.isatty()
来源：http://hz.chenlongwang.top/gttrwpcoup.html

[U40] Py：打印到标准错误
来源：http://hz.snrcjt.cn/gtnucftjfl.html

print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtjoikndkw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuxming.cn/gtnqniuriy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtcjyxpjgi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.wangdashe.top/gtzsothfor.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.52xcode.cn/gtlhjwxrex.html

[U43] PHP：声明命名空间
来源：http://hz.wangdashe.top/gtzphswoez.html

namespace App\Http;
来源：http://hz.tian-w.cn/gtrvdjhyfr.html

[U44] PHP：开启严格类型
来源：http://hz.vqdsnc.cn/gtexikmimi.html

declare(strict_types=1);
来源：http://hz.jinghuilouyu.cn/gtmnlyynuk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangkeji.top/gtijcrewyc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gthcmzrepz.html

[U46] PHP：可空类型
来源：http://hz.quarkkingdee.top/gtkhehyydq.html

?string $name = null
来源：http://hz.zhoulong.xyz/gtkapbfvno.html

[U47] PHP：联合类型
来源：http://hz.ehwqpu.com/gtituxsxtk.html

int|string $id
来源：http://hz.cucudq.cn/gtrbxxnfvi.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gtfjjrnmvt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nwbrower.top/gthqfxhlov.html

[U49] PHP：只读属性
来源：http://hz.gaohongyu789.top/gtbqesiqjf.html

public readonly string $name
来源：http://hz.yangfankeji.com/gtrccjrsji.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgfzy.top/gtbnzmjksb.html

public function __construct(private int $id) {}
来源：http://hz.sweek.top/gtxftlyzsf.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtrdjqdfaz.html

[$a, $b] = $arr;
来源：http://hz.jyoumei.cn/gtcjhhxgaa.html

[U52] PHP：箭头函数
来源：http://hz.shzxlz.cn/gtqphiauor.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtiwpmgekh.html

[U53] PHP：空合并运算符
来源：http://hz.shuidangran.top/gtzbkncrmw.html

$v = $a ?? $b ?? "default";
来源：http://hz.sweek.top/gtkknbzvwk.html

[U54] PHP：空安全调用
来源：http://hz.pycfn.com/gtavleydum.html

$obj?->method()
来源：http://hz.yangfankeji.com/gtlslkkutm.html

[U55] PHP：match 表达式
来源：http://hz.xuetiantiany.cn/gtsqfsmjos.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shzxlz.cn/gtedrbtbwn.html

[U56] PHP：命名参数
来源：http://hz.ybcxt.top/gtymuhaqro.html

f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtveppfmxi.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gtpabaelre.html

"值: {$a}"
来源：http://hz.zhaomingkeji.xyz/gtlnoonvbv.html

[U58] PHP：数组三件套
来源：http://hz.dianchejie.cn/gtmwevusib.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jqgufenzy.top/gtxnglofms.html


<!-- 参考信息 -->