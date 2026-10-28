代发 wailian999

[S37] C++：set
来源：http://hz.xylfe.cn/gtvtgrsbug.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.0kj1m.cn/gtvmswhmbk.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gtpuqfsntk.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtxgfqykzp.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258.top/gtdpiajkfe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.birdmap.top/gtxosszttf.html

[S40] C++：查找元素
来源：http://hz.jinghuilouyu.cn/gtffezjxya.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.iojbl.cn/gteshibiij.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtryslrkvn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhiwuduotai.top/gtgowglcir.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtkwdwmpgv.html

class B : public Base { public: void f() override {} };
来源：http://hz.cdnleiting.top/gtgbjrmomm.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangkeji.top/gtyyrjoqtq.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinyuanbaomall.cn/gtnupuzspk.html

[S44] C++：引用传参
来源：http://hz.fengsongda.top/gttncenrdw.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gtmyuvnhap.html

[S45] C++：lambda
来源：http://hz.xuetiantiany.cn/gthduijryx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sysykeji.top/gtswkrizni.html

[S46] C++：函数模板
来源：http://hz.zhixingplan.top/gtggogyacw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtehhpangs.html

[S47] C++：结构化绑定遍历
来源：http://hz.cdnleiting.top/gtsyopeqhx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtileimtda.html

[S48] C++：逐行读文件
来源：http://hz.0kj1m.cn/gtabazknaf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtaqyqzcdg.html

while (std::getline(in, line)) { }
来源：http://hz.yuanzhike.top/gtirupdies.html

[S49] C++：写文件
来源：http://hz.gogol.net.cn/gtnbjtbnpm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.mhx1999.top/gtjfixrzsa.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtqkkbqspl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtwzxbilhi.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtfosntrxj.html

static_cast<double>(a) / b
来源：http://hz.yj202588.top/gtawwmgdqz.html

[S52] C++：const 与 noexcept
来源：http://hz.redwolf501.top/gtkbavpbdx.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtquroqkrb.html

[S53] C++：移动语义
来源：http://hz.xinyue.icu/gttrizwcxq.html

std::vector<int> w = std::move(v);
来源：http://hz.jqgfzy.top/gtpehjxnrd.html

[S54] C++：异常处理
来源：http://hz.yonumen.top/gtipzuewfp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigfzy.top/gtglhlharp.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gtpztogbrx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gotoacloud.top/gtvprtunln.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtnttunkjj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhijiandao.cn/gtxpaydtis.html

[S57] C++：编译期常量
来源：http://hz.ybcxt.top/gtwqbcesos.html

constexpr int N = 10;
来源：http://hz.ivvv.top/gtbjgxjkyc.html

[S58] C++：命名空间
来源：http://hz.haohaochexian.top/gtjaldawwn.html

namespace ns { int f() { return 1; } }
来源：http://hz.cashguo.top/gtsgrffcdy.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtdjclzumq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydjk.org.cn/gtldkgpokh.html

[S60] C++：遍历并删除元素
来源：http://hz.cucudq.cn/gtonoitafz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shzxlz.cn/gteoueoyhf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgveoslpv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.svipenyu.cn/gtdmjmqvqd.html

================================================================================
来源：http://hz.9152youxi.cn/gtfmrsjuop.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gthtbhswdx.html

println("Hello")
来源：http://hz.xinyue.icu/gthtcbyqdj.html

[T02] Kotlin：变量
来源：http://hz.shangyingyoupin.top/gtrcgrssfb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhiwuduotai.top/gtwjgttfml.html

[T03] Kotlin：字符串模板
来源：http://hz.hnqzz.top/gtzwtyezxq.html

"值: $b"
来源：http://hz.yuanzhike.top/gtchkhdqhh.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtfzainyib.html

val n: String? = null;  n?.length
来源：http://hz.sufxvd.cn/gtzqujkgfa.html

[T05] Kotlin：when 表达式
来源：http://hz.svipenyu.cn/gtfqdmwgen.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gthxadoeni.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtakejmken.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtbkvciseg.html

[T07] Kotlin：集合过滤
来源：http://hz.aibaodan.cn/gtdgvaasgt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtqzlvwxhz.html

[T08] Kotlin：数据类
来源：http://hz.svipenyu.cn/gtotwxmsnb.html

data class User(val name: String, val age: Int)
来源：http://hz.yj20258.top/gtcjmovmaq.html

[T09] Kotlin：扩展函数
来源：http://hz.fengsongda.top/gtnabcosux.html

fun String.exclaim() = this + "!"
来源：http://hz.mhx1999.top/gtcypgmhhr.html

[T10] Kotlin：默认参数
来源：http://hz.zhoulong.xyz/gtnwaytfwf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtuldqkzyr.html

[T11] Kotlin：协程
来源：http://hz.hysaishi.cn/gtsnbxynqh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtcezsmxww.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtwnimyjbw.html

val (a, b) = Pair(1, 2)
来源：http://hz.tian-w.cn/gtyfuaqcah.html

[T13] Kotlin：只读 Map
来源：http://hz.tanke756.top/gtbvbnrfsk.html

val m = mapOf("a" to 1)
来源：http://hz.fengsongda.top/gtypmxowrx.html

[T14] Kotlin：循环
来源：http://hz.shangyingyoupin.top/gthgpzbgge.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtonnmhyct.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtxleujpji.html

interface Shape { fun area(): Double }
来源：http://hz.zhijiandao.cn/gtvaokekfc.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtsmuhnywf.html

print("Hello")
来源：http://hz.kuanghao11.cn/gtrnyxqvof.html

[T17] Swift：变量与常量
来源：http://hz.ppjwa.cn/gtppxjsvfo.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtlbjlsrzy.html

[T18] Swift：字符串插值
来源：http://hz.yuxming.cn/gtlacrkqbe.html

"值: \(b)"
来源：http://hz.shanyushiyangtech.top/gthrcwrcgc.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gthyuyffmo.html

if let n = opt { print(n) }
来源：http://hz.zhixingplan.top/gtrfakpplv.html

[T20] Swift：数组操作
来源：http://hz.ydzc1.top/gtsvxcupzr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gtmoprxvve.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtyzxigcnn.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtcuciahns.html

[T22] Swift：字典
来源：http://hz.shzxlz.cn/gtfwpukkce.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gaohongyu789.top/gtkriegbgv.html

[T23] Swift：函数
来源：http://hz.sxryk.cn/gtbyoabyzu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtebupseku.html

[T24] Swift：闭包
来源：http://hz.ydzc1.top/gtlxdhyvfw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtrdiecvfz.html

[T25] Swift：结构体
来源：http://hz.nanxuanxn.top/gthvrwkgdd.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtwmftwrac.html

[T26] Swift：类与重写
来源：http://hz.fengsongda.top/gtidllbyez.html

class A: Base { override func f() {} }
来源：http://hz.ehwqpu.com/gteofpcjtt.html

[T27] Swift：错误处理
来源：http://hz.yanxiufei.cn/gtzegqtcqc.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtbyzevrso.html

[T28] Swift：枚举
来源：http://hz.gotoacloud.top/gtkmnumbqc.html

enum Color { case red, green }
来源：http://hz.cheryme.top/gtbkkwrlvf.html

[T29] Swift：guard 提前返回
来源：http://hz.sweek.top/gtxhedpxai.html

guard let x = opt else { return }
来源：http://hz.jianghu66.top/gttaelbadg.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gttdockiej.html

protocol Shape { func area() -> Double }
来源：http://hz.cdnleiting.top/gtmdvuiopn.html

[T31] Lua：Hello World
来源：http://hz.hammf.cn/gtcqaxjmuw.html

print("Hello")
来源：http://hz.316326.xyz/gtkyusbhij.html

[T32] Lua：局部变量
来源：http://hz.yuanzhike.top/gtnypqxjvc.html

local a = 1
来源：http://hz.shzxlz.cn/gtocoralaz.html

[T33] Lua：表（数组）
来源：http://hz.shanyushiyangkeji.top/gtjdzshlrx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhengqikj.top/gtwmopxrma.html

[T34] Lua：遍历表
来源：http://hz.yj20258888.top/gtakbbflrz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.mhx1999.top/gttdtcqydn.html

[T35] Lua：字典表
来源：http://hz.zhiwuduotai.top/gtperqffyg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgfzy.top/gthjqrihrj.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gtdaqgjvaw.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtfbhuoqcy.html

[T37] Lua：字符串拼接
来源：http://hz.xuetiantiany.cn/gtevffnzja.html

"a" .. "b"
来源：http://hz.zhiwuduotai.top/gtqkrvsnjp.html

[T38] Lua：条件
来源：http://hz.yj20258888.top/gtwphxgsuj.html

if x > 0 then print("正") end
来源：http://hz.hammf.cn/gteuwgylqo.html

[T39] Lua：模式匹配
来源：http://hz.yongpay.top/gtiszyotrv.html

string.find(s, "%d+")
来源：http://hz.zhoulong.xyz/gtmrpvdfni.html

[T40] Lua：元表
来源：http://hz.chenzaomai.com/gtdxvpecqv.html

setmetatable({}, { __index = base })
来源：http://hz.hfpthk.cn/gthngbkexw.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gthnedzdkd.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtfcfzlxda.html

[T42] Perl：变量类型
来源：http://hz.mhx1999.top/gtlfcsvsre.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.birdmap.top/gthiqbchxi.html

[T43] Perl：字符串插值
来源：http://hz.meibo888.top/gtsodbvuov.html

"值: $a"
来源：http://hz.yonumen.top/gtjwoyiftu.html

[T44] Perl：条件
来源：http://hz.redwolf501.top/gtutlysdiq.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gtdnjndlqr.html

[T45] Perl：数组遍历
来源：http://hz.cqqwz.cn/gtcoifdhwo.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gtmwmectnf.html

[T46] Perl：哈希操作
来源：http://hz.yongpay.top/gtltszybuf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yvedp.cn/gttusnqneu.html

[T47] Perl：正则捕获
来源：http://hz.snrcjt.cn/gtwmjxigcr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gtxpwvjoze.html

[T48] Perl：正则替换
来源：http://hz.jyoumei.cn/gtdohrmvlq.html

$s =~ s/old/new/g;
来源：http://hz.shzxlz.cn/gtshzzjcjl.html

[T49] Perl：函数
来源：http://hz.sweek.top/gtugohumek.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtaqtomiut.html

[T50] Perl：逐行读文件
来源：http://hz.cucudq.cn/gtflzraphx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.andypj.xyz/gtidsednbh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cashguo.top/gtfyqswdfd.html

[T51] Scala：Hello World
来源：http://hz.hywenlv.cn/gtepyuxjjd.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtdbbsoltz.html

[T52] Scala：变量
来源：http://hz.xingfuxueyuan.xyz/gtmjiuzdps.html

val a = 1;  var b = 2
来源：http://hz.smart0.xyz/gtwtpnayrb.html

[T53] Scala：字符串插值
来源：http://hz.ehwqpu.com/gtedvrjrnu.html

s"值: $b"
来源：http://hz.hfpthk.cn/gtmrbrduru.html

[T54] Scala：集合映射
来源：http://hz.gaohongyu789.top/gttmlwcqld.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jqgfzy.top/gtxxkgpund.html

[T55] Scala：集合过滤
来源：http://hz.iojbl.cn/gtdsnsyalh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yueranfly.top/gtcfxmosqf.html

[T56] Scala：样例类
来源：http://hz.ivvv.top/gtiqwzjlpb.html

case class User(name: String, age: Int)
来源：http://hz.cdnleiting.top/gthfuhklvu.html

[T57] Scala：模式匹配
来源：http://hz.zhaomingkeji.xyz/gtsbcqixfi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xinyue.icu/gtgugfwnml.html

[T58] Scala：函数定义
来源：http://hz.hfpthk.cn/gtvzbhlbqz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jyoumei.cn/gtwnnuuugt.html

[T59] Scala：循环
来源：http://hz.ehwqpu.com/gtplmnhvsm.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gtfpchqfvp.html

[T60] Scala：折叠
来源：http://hz.sufxvd.cn/gtcbdzbigj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sysykeji.top/gtgrijyjmb.html

================================================================================
来源：http://hz.guannengcc.top/gtherrajfe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gttrppjlbu.html

================================================================================
来源：http://hz.mhx1999.top/gtxqqxwuzn.html

[U01] Py：创建虚拟环境
来源：http://hz.jinyuanbaomall.cn/gtdrgnbtzy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hysaishi.cn/gtdwofuljm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shuidangran.top/gtkepobyif.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.52xcode.cn/gtwxmtbeqz.html

[U03] Py：加载 .env 配置
来源：http://hz.zhengqikj.top/gtqazysamf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.andypj.xyz/gtvfwoeykh.html

[U04] Py：变量调试打印
来源：http://hz.jyoumei.cn/gtcbuwlclz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cheryme.top/gtbleaeesk.html

[U05] Py：列表去重且保序
来源：http://hz.sweek.top/gtoxofbshx.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gthwyzrbqg.html

[U06] Py：合并两个字典
来源：http://hz.andypj.xyz/gtwkzmerec.html

{**a, **b}
来源：http://hz.jinqigufen.top/gtoyyjvbvv.html

[U07] Py：反转字典键值
来源：http://hz.zdqjudy.top/gtdrwovsbt.html

{v: k for k, v in d.items()}
来源：http://hz.zdqjudy.top/gtoyxmiyyi.html

[U08] Py：展平二维列表
来源：http://hz.tanke756.top/gtxhfxfesz.html

[y for x in nested for y in x]
来源：http://hz.316326.xyz/gtywulauws.html

[U09] Py：字典取最大值的键
来源：http://hz.yueranfly.top/gtzfiznvdl.html

max(d, key=d.get)
来源：http://hz.kuanghao11.cn/gtxqirhhjb.html

[U10] Py：按值排序字典
来源：http://hz.nwbrower.top/gtrrhnenem.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinghuilouyu.cn/gtledqzcxu.html

[U11] Py：生成器表达式
来源：http://hz.guannengcc.top/gtrqbqhabj.html

(x * 2 for x in arr)
来源：http://hz.ydzc1.top/gtellgfojq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.tian-w.cn/gtbuqvuols.html

Counter(arr).most_common(3)
来源：http://hz.hfpthk.cn/gtnydwjgax.html

[U13] Py：固定长度队列
来源：http://hz.yangfankeji.com/gtbwftfvzw.html

deque(maxlen=10)
来源：http://hz.ydzc1.top/gtvfmloeya.html

[U14] Py：分组收集到列表
来源：http://hz.yonumen.top/gtjmxdznvq.html

defaultdict(list)
来源：http://hz.jqgufenzy.top/gtnkgkvakh.html

[U15] Py：高精度计时
来源：http://hz.hysaishi.cn/gtbylnwfln.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtynmrvapw.html

[U16] Py：命令行参数解析
来源：http://hz.fzhhl.top/gtkrgphlpx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sweek.top/gtnapyjzxb.html

[U17] Py：初始化日志
来源：http://hz.cdnleiting.top/gtlvvnjxis.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gthfukixdk.html

[U18] Py：预编译正则
来源：http://hz.xuanzx.com/gtypelmofd.html

pat = re.compile(r"\d+")
来源：http://hz.jiagoushi.top/gtabbwxzde.html

[U19] Py：正则替换带回调
来源：http://hz.cqqwz.cn/gtovowrzpr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhaomingkeji.xyz/gtfksbncxa.html

[U20] Py：缓存函数结果
来源：http://hz.jyoumei.cn/gtifedsxcm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hnqzz.top/gtrowavswa.html

[U21] Py：自定义上下文管理器
来源：http://hz.jqgfzy.top/gtceqiyrxh.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gtkwvzjczf.html

[U22] Py：矩阵转置
来源：http://hz.jinghuilouyu.cn/gtnwnlxgqo.html

list(zip(*m))
来源：http://hz.shangyingyoupin.top/gtfrhirkdw.html

[U23] Py：分块读取大文件
来源：http://hz.cashguo.top/gtuorwxsup.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shuidangran.top/gtisdagyzd.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtgcswhowx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.dashuyun.cn/gtiktzaxdb.html

[U25] Py：CSV 按字典读
来源：http://hz.xuetiantiany.cn/gtpcmrhycy.html

csv.DictReader(f)
来源：http://hz.yongpay.top/gtglaeiygh.html

[U26] Py：并发下载
来源：http://hz.pycfn.com/gthabpbopd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinghuilouyu.cn/gtwocmbxqa.html

[U27] Py：异步 HTTP
来源：http://hz.feifeiyinyue.top/gtsfjoxjtn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.vqdsnc.cn/gtucpwqzpe.html

[U28] Py：类型别名
来源：http://hz.tianlin.xyz/gtvsmwykbz.html

UserId = int
来源：http://hz.hnxiangtu.top/gtppjpmqqn.html

[U29] Py：属性校验
来源：http://hz.hammf.cn/gtgewzpiio.html

@property 与 @x.setter 配合
来源：http://hz.ehwqpu.com/gtzliubxop.html

[U30] Py：数据类
来源：http://hz.9152youxi.cn/gteyjbmkwh.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gtpzixfqbu.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtkltcdksr.html

python -m pytest -q
来源：http://hz.smart0.xyz/gttigmcoiq.html

[U32] Py：代码格式化
来源：http://hz.ivvv.top/gtitzqatew.html

ruff format . && ruff check --fix .
来源：http://hz.smart0.xyz/gtuubnyvxt.html

[U33] Py：打包发布
来源：http://hz.gotoacloud.top/gtwfexucdp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dashuyun.cn/gtvyfasrmi.html

[U34] Py：判断编码
来源：http://hz.hywenlv.cn/gtzltuzuak.html

chardet.detect(raw)
来源：http://hz.tianlin.xyz/gtgxzoxlgk.html

[U35] Py：发送邮件
来源：http://hz.shangyingyoupin.top/gtkkxduxny.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhiwuduotai.top/gtkfvlgljg.html

[U36] Py：定时任务
来源：http://hz.cqqwz.cn/gtexsxloby.html

schedule.every(10).minutes.do(job)
来源：http://hz.aizwys.cn/gtqzwbsize.html

[U37] Py：读写 Excel
来源：http://hz.ppjwa.cn/gtarwpylzr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cqqwz.cn/gtfbyklbup.html

[U38] Py：获取脚本所在目录
来源：http://hz.ivvv.top/gtoxhwbxma.html

Path(__file__).resolve().parent
来源：http://hz.meibo888.top/gtxzhkuteq.html

[U39] Py：判断是否在交互环境
来源：http://hz.cdnleiting.top/gtubpgivan.html

sys.stdout.isatty()
来源：http://hz.yj202588.top/gtklwngkoi.html

[U40] Py：打印到标准错误
来源：http://hz.guowangkeji.top/gtnnhhplnh.html

print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtopjsirdk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shzxlz.cn/gtxizlctos.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ywan-chungtsiang.top/gtnvkjfrzj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cheryme.top/gtoejmqcpd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fzhhl.top/gtgpvhghwp.html

[U43] PHP：声明命名空间
来源：http://hz.havefunace.top/gttopxpnfa.html

namespace App\Http;
来源：http://hz.yuxming.cn/gtyquacebm.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gtwbodmpoo.html

declare(strict_types=1);
来源：http://hz.ydzc1.top/gtlemlzdei.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtdmszwezc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtenvpbifk.html

[U46] PHP：可空类型
来源：http://hz.snrcjt.cn/gtjruzjraf.html

?string $name = null
来源：http://hz.xinyue.icu/gtgnkpxblv.html

[U47] PHP：联合类型
来源：http://hz.zycfv.cn/gtaebzgocl.html

int|string $id
来源：http://hz.pengpengdd.cyou/gtbzqroaid.html

[U48] PHP：纯枚举
来源：http://hz.yj20258888.top/gtyslmwjlo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gaohongyu789.top/gtnppmscvc.html

[U49] PHP：只读属性
来源：http://hz.jinqigfzy.top/gtgmkoovqf.html

public readonly string $name
来源：http://hz.jianghu66.top/gtipefxxwu.html

[U50] PHP：构造器属性提升
来源：http://hz.ydjk.org.cn/gtslpwjnaa.html

public function __construct(private int $id) {}
来源：http://hz.zhengqikj.top/gtcpfryqcm.html

[U51] PHP：数组解构
来源：http://hz.gotoacloud.top/gtqbocvads.html

[$a, $b] = $arr;
来源：http://hz.hammf.cn/gtiabanxnc.html

[U52] PHP：箭头函数
来源：http://hz.52xcode.cn/gtxxcqwbsf.html

$double = fn($x) => $x * 2;
来源：http://hz.bjfxy.top/gtayzordqo.html

[U53] PHP：空合并运算符
来源：http://hz.yuxming.cn/gtklmphbfy.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenzaomai.com/gtkjydftzd.html

[U54] PHP：空安全调用
来源：http://hz.shangyingyoupin.top/gtkslwhxdy.html

$obj?->method()
来源：http://hz.aizwys.cn/gtdzucyezm.html

[U55] PHP：match 表达式
来源：http://hz.vqdsnc.cn/gtvucnbodu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hnqzz.top/gttygajqui.html

[U56] PHP：命名参数
来源：http://hz.meibo888.top/gtiyrivbia.html

f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtxgxhgnjy.html

[U57] PHP：字符串插值
来源：http://hz.ybcxt.top/gtyktibyrh.html

"值: {$a}"
来源：http://hz.316326.xyz/gtuzskoabt.html

[U58] PHP：数组三件套
来源：http://hz.cqqwz.cn/gtsqguhelo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hywenlv.cn/gttrtegrly.html

[U59] PHP：自定义排序
来源：http://hz.ivvv.top/gtkpwpldwc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gthyqdgxmj.html

[U60] PHP：JSON 编解码
来源：http://hz.yj20258.top/gtikgztzlx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shanyushiyangkeji.top/gtozfifioi.html

[U61] PHP：正则
来源：http://hz.xinyue.icu/gtieahvcin.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtlfktfsll.html

[U62] PHP：日期对象
来源：http://hz.yj20258888.top/gtrompnjgn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtezjhjwcz.html


<!-- 参考信息 -->