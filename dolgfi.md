代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.daxiang520.top/gtewbyqngw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtigjtlnvb.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtugwjynhj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuxming.cn/gtpbphkolw.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gtngagqlfp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtvgbyqfpy.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtlsumbior.html

class B : public Base { public: void f() override {} };
来源：http://hz.pycfn.com/gtplgcghdh.html

[S43] C++：智能指针
来源：http://hz.meibo888.top/gtsbadynif.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtyqrcnnta.html

[S44] C++：引用传参
来源：http://hz.haohaochexian.top/gtjmekvsrw.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gtmjapuemy.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtszrgmgez.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jlsjyb.cn/gtjlvzkgsj.html

[S46] C++：函数模板
来源：http://hz.yuxming.cn/gtzcjnqbfy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtsajaeahj.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtohkktalj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtucdiejtj.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtfonijnml.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nwbrower.top/gtbpqetgyt.html

while (std::getline(in, line)) { }
来源：http://hz.quarkkingdee.top/gtmioaevvk.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtjbdmmllb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gtvhpfnhsw.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtinkcbfhw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.haohaochexian.top/gthjreacmo.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtaiapcaun.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtmvxehfng.html

[S52] C++：const 与 noexcept
来源：http://hz.sysykeji.top/gtfddjuhbd.html

int size() const noexcept { return n_; }
来源：http://hz.tianlin.xyz/gtglzakdrv.html

[S53] C++：移动语义
来源：http://hz.yj20258.top/gtrlndlkqk.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtqndorltl.html

[S54] C++：异常处理
来源：http://hz.yj202588.top/gtodyqclgj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtxodvaxpt.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtwffedwdi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtzwajzxrz.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtcfkjajhs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gthnfvmhjt.html

[S57] C++：编译期常量
来源：http://hz.aizwys.cn/gtxxlujdei.html

constexpr int N = 10;
来源：http://hz.fengsongda.top/gtypbxykme.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtmeejbuhd.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtixnvtvoz.html

[S59] C++：静态断言
来源：http://hz.bjfxy.top/gtodkwrauh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinghuilouyu.cn/gtulzouyut.html

[S60] C++：遍历并删除元素
来源：http://hz.gaohongyu789.top/gtevpawitk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtaisvdifg.html

================================================================================
来源：http://hz.cqqwz.cn/gteforvpqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ppjwa.cn/gtzpplfopp.html

================================================================================
来源：http://hz.yj202588.top/gtojurwntq.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtokblgyaa.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtjgmgddiv.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtaayehumz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guowangkeji.top/gtnowclzkl.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gttzwlzrbd.html

"值: $b"
来源：http://hz.zycfv.cn/gtbbgbiltq.html

[T04] Kotlin：空安全
来源：http://hz.gogol.net.cn/gtoloxevkt.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtypzjgkxe.html

[T05] Kotlin：when 表达式
来源：http://hz.hywenlv.cn/gtaulkpvct.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gtgzmgwaii.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gtwjfxxxqi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gtoejbkagk.html

[T07] Kotlin：集合过滤
来源：http://hz.jianghu66.top/gtpqpciwpr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenjidiqi.icu/gtvhgzyqzr.html

[T08] Kotlin：数据类
来源：http://hz.52xcode.cn/gtnwovkmmr.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtkumwybue.html

[T09] Kotlin：扩展函数
来源：http://hz.xuanzx.com/gtemkkwfzq.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtyalwbbiy.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gtqvjturqa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtkiyubzsx.html

[T11] Kotlin：协程
来源：http://hz.9152youxi.cn/gtxirglmtq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtcppptspv.html

[T12] Kotlin：解构声明
来源：http://hz.cucudq.cn/gtpztexxym.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258.top/gtcxzvmiyt.html

[T13] Kotlin：只读 Map
来源：http://hz.316326.xyz/gtzkycwmlp.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtupqbvllb.html

[T14] Kotlin：循环
来源：http://hz.andypj.xyz/gtuplpmjao.html

for (i in 1..10) println(i)
来源：http://hz.zdqjudy.top/gtnxfimisk.html

[T15] Kotlin：接口
来源：http://hz.316326.xyz/gtgsixzlne.html

interface Shape { fun area(): Double }
来源：http://hz.xuetiantiany.cn/gthjikityc.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtvwyhrcgl.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtebdrsysj.html

[T17] Swift：变量与常量
来源：http://hz.yuxming.cn/gtjsvfnivx.html

var a = 1;  let b = 2
来源：http://hz.yj20258.top/gtvjeeamfi.html

[T18] Swift：字符串插值
来源：http://hz.cheryme.top/gtewojyegq.html

"值: \(b)"
来源：http://hz.9152youxi.cn/gtfycperuz.html

[T19] Swift：可选绑定
来源：http://hz.jlsjyb.cn/gtufxtvruq.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtudgaatcp.html

[T20] Swift：数组操作
来源：http://hz.wangdashe.top/gttuozomsq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtezerhrpz.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gtxrskonfr.html

for x in a { print(x) }
来源：http://hz.dashuyun.cn/gtretdixjc.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtdjexhhdb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gtqociejxe.html

[T23] Swift：函数
来源：http://hz.hongshengwenyu.top/gtvezxnary.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.haohaochexian.top/gtfjplypyf.html

[T24] Swift：闭包
来源：http://hz.chenlongwang.top/gthomdabaa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.svipenyu.cn/gtfunjnqfu.html

[T25] Swift：结构体
来源：http://hz.ehwqpu.com/gttqusrehk.html

struct P { var x: Int }
来源：http://hz.sysykeji.top/gtatzpckfo.html

[T26] Swift：类与重写
来源：http://hz.smart0.xyz/gttluvieyy.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtxbfisfif.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gtkyygbomz.html

do { try f() } catch { print(error) }
来源：http://hz.aibaodan.cn/gtdrpmrxks.html

[T28] Swift：枚举
来源：http://hz.hfpthk.cn/gteefyfgff.html

enum Color { case red, green }
来源：http://hz.hongshengwenyu.top/gtcrwazcmb.html

[T29] Swift：guard 提前返回
来源：http://hz.xinyue.icu/gtuflgvkfi.html

guard let x = opt else { return }
来源：http://hz.sxryk.cn/gttoemzwlj.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gtpafpfmjw.html

protocol Shape { func area() -> Double }
来源：http://hz.yuxming.cn/gtirmpxnwu.html

[T31] Lua：Hello World
来源：http://hz.zdqjudy.top/gtmrdyqprm.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtihzezsmz.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtulmodawr.html

local a = 1
来源：http://hz.daxiang520.top/gtdedasixy.html

[T33] Lua：表（数组）
来源：http://hz.shangyingyoupin.top/gtapwplqqn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guowangkeji.top/gttbfffbgp.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtcpnhbybq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tian-w.cn/gtvaaimlhe.html

[T35] Lua：字典表
来源：http://hz.xuanzx.com/gtfnaflysw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhiwuduotai.top/gtydkytbcj.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtyzsiuvem.html

function add(a, b) return a + b end
来源：http://hz.dashuyun.cn/gtvztjprsv.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtsxrcenlg.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtycrsrxpv.html

[T38] Lua：条件
来源：http://hz.jinyuanbaomall.cn/gtxqzphuds.html

if x > 0 then print("正") end
来源：http://hz.52xcode.cn/gtmlqeuamj.html

[T39] Lua：模式匹配
来源：http://hz.yuanzhike.top/gtuikpbtjn.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtjnwsppae.html

[T40] Lua：元表
来源：http://hz.gzhubu.top/gtulwffnwj.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtlwfrmytc.html

[T41] Perl：Hello World
来源：http://hz.ybcxt.top/gtvslpbnej.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtpqnqcnjs.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtahhuclhy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtqmqizydt.html

[T43] Perl：字符串插值
来源：http://hz.jyoumei.cn/gtvslgcwil.html

"值: $a"
来源：http://hz.cqqwz.cn/gtajthjnyh.html

[T44] Perl：条件
来源：http://hz.haohaochexian.top/gtexpwojnh.html

if ($a > 0) { print "正"; }
来源：http://hz.ywan-chungtsiang.top/gtuwylzhgn.html

[T45] Perl：数组遍历
来源：http://hz.jianghu66.top/gtbhoyivvv.html

for my $x (@arr) { print $x; }
来源：http://hz.chenzaomai.com/gtapbybova.html

[T46] Perl：哈希操作
来源：http://hz.yangfankeji.com/gtapcsbxmc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jqgufenzy.top/gthskezohf.html

[T47] Perl：正则捕获
来源：http://hz.jinyuanbaomall.cn/gtndjeaqru.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.c1oappe.top/gtokxtduzo.html

[T48] Perl：正则替换
来源：http://hz.hongshengwenyu.top/gtxjqocfka.html

$s =~ s/old/new/g;
来源：http://hz.ydzc1.top/gtsiaevfec.html

[T49] Perl：函数
来源：http://hz.redwolf501.top/gtotgmvala.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gtfsqrfdog.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtwpmzgqgj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gotoacloud.top/gtsxkuwfrc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cqqwz.cn/gtcnlwbrzx.html

[T51] Scala：Hello World
来源：http://hz.wangshuangyany.cn/gtdawukhsf.html

println("Hello")
来源：http://hz.sxryk.cn/gtloriszyl.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtrwketshn.html

val a = 1;  var b = 2
来源：http://hz.redwolf501.top/gtcftfhjhj.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtgrkhmizf.html

s"值: $b"
来源：http://hz.zdqjudy.top/gtqhotdwwj.html

[T54] Scala：集合映射
来源：http://hz.jianghu66.top/gtsatchjqc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtwjbpwkov.html

[T55] Scala：集合过滤
来源：http://hz.aibaodan.cn/gthsfatzib.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.pengpengdd.cyou/gthorzuzog.html

[T56] Scala：样例类
来源：http://hz.smart0.xyz/gtqbnnrpah.html

case class User(name: String, age: Int)
来源：http://hz.zhongyouzk.top/gtzytmazbl.html

[T57] Scala：模式匹配
来源：http://hz.haohaochexian.top/gtteqtvztw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nanxuanxn.top/gtbloqkgfl.html

[T58] Scala：函数定义
来源：http://hz.yonumen.top/gtsswymjeq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shzxlz.cn/gtnpatpujx.html

[T59] Scala：循环
来源：http://hz.nanxinkj.top/gtdesceihl.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gtzxuxqbid.html

[T60] Scala：折叠
来源：http://hz.zhoulong.xyz/gttzxbkmqw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhaomingkeji.xyz/gtvvavming.html

================================================================================
来源：http://hz.jlsjyb.cn/gtybohlrrf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj202588.top/gtrtsrighk.html

================================================================================
来源：http://hz.sufxvd.cn/gtjfzoxmrl.html

[U01] Py：创建虚拟环境
来源：http://hz.hywenlv.cn/gtlxlsplxb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydjk.org.cn/gtjjdfdvjr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinqigfzy.top/gtjqfwigln.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtkeuvjhzx.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigfzy.top/gtyltzxdbn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.aibaodan.cn/gtrtuatckr.html

[U04] Py：变量调试打印
来源：http://hz.fzhhl.top/gtfgllpxhz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pycfn.com/gtuifajbkh.html

[U05] Py：列表去重且保序
来源：http://hz.wangshuangyany.cn/gtdwctuftf.html

list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtcgphfvyw.html

[U06] Py：合并两个字典
来源：http://hz.fengsongda.top/gtepkkzwlw.html

{**a, **b}
来源：http://hz.hysaishi.cn/gtzbpxvrea.html

[U07] Py：反转字典键值
来源：http://hz.yuxming.cn/gtzivxrdjx.html

{v: k for k, v in d.items()}
来源：http://hz.yanxiufei.cn/gtahxjitnx.html

[U08] Py：展平二维列表
来源：http://hz.gzhubu.top/gttpqyxubd.html

[y for x in nested for y in x]
来源：http://hz.bjfxy.top/gtytypajbd.html

[U09] Py：字典取最大值的键
来源：http://hz.jlsjyb.cn/gtrmiivsiq.html

max(d, key=d.get)
来源：http://hz.yj20258888.top/gtobaoqeib.html

[U10] Py：按值排序字典
来源：http://hz.gogol.net.cn/gtkyoxmvcq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hysaishi.cn/gtxskogulm.html

[U11] Py：生成器表达式
来源：http://hz.cashguo.top/gtohjrihee.html

(x * 2 for x in arr)
来源：http://hz.aibaodan.cn/gthdluainx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gogol.net.cn/gtgxkqvvvo.html

Counter(arr).most_common(3)
来源：http://hz.jiagoushi.top/gtyrhvwejc.html

[U13] Py：固定长度队列
来源：http://hz.yangfankeji.com/gtkydfpdfu.html

deque(maxlen=10)
来源：http://hz.iojbl.cn/gtindnmqyu.html

[U14] Py：分组收集到列表
来源：http://hz.svipenyu.cn/gtwpaakjtz.html

defaultdict(list)
来源：http://hz.jlsjyb.cn/gtrfpghcuk.html

[U15] Py：高精度计时
来源：http://hz.cdnleiting.top/gtyqybfxop.html

t = time.perf_counter()
来源：http://hz.jqgufenzy.top/gtndcmtztl.html

[U16] Py：命令行参数解析
来源：http://hz.0kj1m.cn/gtdkqbfput.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shangyingyoupin.top/gtgwwzliqe.html

[U17] Py：初始化日志
来源：http://hz.yongpay.top/gtuwqxvndo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.mhx1999.top/gtsgcrgcme.html

[U18] Py：预编译正则
来源：http://hz.pengpengdd.cyou/gtcoknryhg.html

pat = re.compile(r"\d+")
来源：http://hz.dianchejie.cn/gtimvamxfq.html

[U19] Py：正则替换带回调
来源：http://hz.yj20258888.top/gtoilzmmxu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydjk.org.cn/gtjmkaxfvk.html

[U20] Py：缓存函数结果
来源：http://hz.sysykeji.top/gttbfdlxau.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gogol.net.cn/gtcyyuxgpu.html

[U21] Py：自定义上下文管理器
来源：http://hz.tanke756.top/gtjaegkzuq.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangkeji.top/gtjcgdwgnt.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gtqxaayvlt.html

list(zip(*m))
来源：http://hz.sweek.top/gtmehcvdan.html

[U23] Py：分块读取大文件
来源：http://hz.cdnleiting.top/gtvuoddvvc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhaomingkeji.xyz/gtjpluiixn.html

[U24] Py：路径操作
来源：http://hz.meibo888.top/gtseikivfs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtrmhhsgbh.html

[U25] Py：CSV 按字典读
来源：http://hz.nwbrower.top/gtoflbqtsn.html

csv.DictReader(f)
来源：http://hz.316326.xyz/gtjklwqtlq.html

[U26] Py：并发下载
来源：http://hz.quarkkingdee.top/gtdpaqjenw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aibaodan.cn/gtcpnpbffg.html

[U27] Py：异步 HTTP
来源：http://hz.iojbl.cn/gtothbzwmc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtfscewoaw.html

[U28] Py：类型别名
来源：http://hz.jqgfzy.top/gtcptolmua.html

UserId = int
来源：http://hz.nanxinkj.top/gtzhhogrqv.html

[U29] Py：属性校验
来源：http://hz.yongpay.top/gtpycxkcxj.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtiayxuztn.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtdxypieqw.html

@dataclass(slots=True)
来源：http://hz.bjfxy.top/gtiehxhtzr.html

[U31] Py：单测
来源：http://hz.hnqzz.top/gtrryzsypn.html

python -m pytest -q
来源：http://hz.snrcjt.cn/gtvjywosri.html

[U32] Py：代码格式化
来源：http://hz.hongshengwenyu.top/gttuisectx.html

ruff format . && ruff check --fix .
来源：http://hz.snrcjt.cn/gtjvbuymkj.html

[U33] Py：打包发布
来源：http://hz.sweek.top/gtmzoaylrs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yueranfly.top/gtapsmnxxn.html

[U34] Py：判断编码
来源：http://hz.yonumen.top/gtxzsspnqw.html

chardet.detect(raw)
来源：http://hz.sxryk.cn/gtkkcctojt.html

[U35] Py：发送邮件
来源：http://hz.aizwys.cn/gtqlvahiol.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.0kj1m.cn/gtuywobpos.html

[U36] Py：定时任务
来源：http://hz.ehwqpu.com/gtndapynvy.html

schedule.every(10).minutes.do(job)
来源：http://hz.smart0.xyz/gthvmqeiwy.html

[U37] Py：读写 Excel
来源：http://hz.sufxvd.cn/gttysbkvrx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ppjwa.cn/gtrwvqmglk.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gtwonfmqgc.html

Path(__file__).resolve().parent
来源：http://hz.zdqjudy.top/gtkunzxnhb.html

[U39] Py：判断是否在交互环境
来源：http://hz.ehwqpu.com/gtbmnuhitb.html

sys.stdout.isatty()
来源：http://hz.jinqigufen.top/gtqkskoepm.html

[U40] Py：打印到标准错误
来源：http://hz.hongshengwenyu.top/gtaqxpuexr.html

print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtfaabcyrc.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jianghu66.top/gtjxucoibr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtwvwnljfh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cucudq.cn/gtoejwdcgg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xziqi.cn/gtemakalwg.html

[U43] PHP：声明命名空间
来源：http://hz.quarkkingdee.top/gtmdsphhdj.html

namespace App\Http;
来源：http://hz.yj202588.top/gtwkbjywqc.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangtech.top/gtyyommsgx.html

declare(strict_types=1);
来源：http://hz.zhoulong.xyz/gtrijjemma.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fzhhl.top/gtfpgvxgau.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtlupoftbj.html

[U46] PHP：可空类型
来源：http://hz.tianlin.xyz/gtwyzqsuzo.html

?string $name = null
来源：http://hz.zhaomingkeji.xyz/gtcrrxslog.html

[U47] PHP：联合类型
来源：http://hz.snrcjt.cn/gtqrwxydhm.html

int|string $id
来源：http://hz.cashguo.top/gtblzxdnoc.html

[U48] PHP：纯枚举
来源：http://hz.xingfuxueyuan.xyz/gtgcgxhtwu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tian-w.cn/gtybyvwgqm.html

[U49] PHP：只读属性
来源：http://hz.hysaishi.cn/gtseyohbrw.html

public readonly string $name
来源：http://hz.sweek.top/gtrsybbnme.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258.top/gtbgfapvyg.html

public function __construct(private int $id) {}
来源：http://hz.tian-w.cn/gthzzpnqom.html

[U51] PHP：数组解构
来源：http://hz.aibaodan.cn/gtlagfjure.html

[$a, $b] = $arr;
来源：http://hz.tian-w.cn/gtwrallbhr.html

[U52] PHP：箭头函数
来源：http://hz.hysaishi.cn/gtjpsatoak.html

$double = fn($x) => $x * 2;
来源：http://hz.aizwys.cn/gtmjzskwli.html

[U53] PHP：空合并运算符
来源：http://hz.0kj1m.cn/gteomciubv.html

$v = $a ?? $b ?? "default";
来源：http://hz.fengsongda.top/gtqtbnsglz.html

[U54] PHP：空安全调用
来源：http://hz.yj202588.top/gtxduicubl.html

$obj?->method()
来源：http://hz.ehwqpu.com/gtyovcolvj.html

[U55] PHP：match 表达式
来源：http://hz.shzxlz.cn/gtkxnskvkn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenlongwang.top/gthfejocjk.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtodxqqaay.html

f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtcslvpzzy.html

[U57] PHP：字符串插值
来源：http://hz.wangshuangyany.cn/gtqzixhaxy.html

"值: {$a}"
来源：http://hz.zhengqikj.top/gtrumusxuk.html

[U58] PHP：数组三件套
来源：http://hz.hnxiangtu.top/gtqcbncidh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj20258888.top/gtnmqgmrks.html

[U59] PHP：自定义排序
来源：http://hz.316326.xyz/gtmijozjqk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtkhnhcqlq.html

[U60] PHP：JSON 编解码
来源：http://hz.hnxiangtu.top/gtuphrxifa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yueranfly.top/gtdwihnnwb.html

[U61] PHP：正则
来源：http://hz.zhijiandao.cn/gtrpkwbrey.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtzyviajum.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gtinmorhov.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yongpay.top/gtaylliftm.html

[U63] PHP：文件读写
来源：http://hz.kuanghao11.cn/gtnekjaybv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yueranfly.top/gtwkwnruzd.html

[U64] PHP：目录遍历
来源：http://hz.gotoacloud.top/gtyctbyjow.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhixingplan.top/gtshczsyod.html


<!-- 参考信息 -->