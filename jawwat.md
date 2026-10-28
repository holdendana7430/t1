代发 wailian999

[S37] C++：set
来源：http://hz.bjfxy.top/gtywzadbgl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigufen.top/gtddjhnobl.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtictgokce.html

std::sort(v.begin(), v.end());
来源：http://hz.yvedp.cn/gthprlzlfo.html

[S39] C++：自定义比较器排序
来源：http://hz.guowangkeji.top/gtkfjycnfb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtfduqoqaf.html

[S40] C++：查找元素
来源：http://hz.yj20258.top/gtjklfjcpf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhixingplan.top/gtkkqueisw.html

[S41] C++：类与构造函数
来源：http://hz.c1oappe.top/gtiekkcogp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pycfn.com/gtlwzcsfxn.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtzlesxtpe.html

class B : public Base { public: void f() override {} };
来源：http://hz.hysaishi.cn/gttepogzns.html

[S43] C++：智能指针
来源：http://hz.zhiwuduotai.top/gtrricnbkv.html

auto p = std::make_unique<int>(5);
来源：http://hz.wangshuangyany.cn/gteyhpybxj.html

[S44] C++：引用传参
来源：http://hz.chenzaomai.com/gtgygwokgv.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gtryhataff.html

[S45] C++：lambda
来源：http://hz.vqdsnc.cn/gtcnvmuost.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtolldykrb.html

[S46] C++：函数模板
来源：http://hz.zhijiandao.cn/gtrfyuzjkh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtryhskuie.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtmittvghl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhoulong.xyz/gtsdoqqmfo.html

[S48] C++：逐行读文件
来源：http://hz.316326.xyz/gtsgdjvrba.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtfylhaujq.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtutmvzkog.html

[S49] C++：写文件
来源：http://hz.birdmap.top/gtgvtzsfhe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ivvv.top/gtrxqpdadw.html

[S50] C++：格式化数字
来源：http://hz.birdmap.top/gtobulwyyx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xingfuxueyuan.xyz/gtwufdhcpu.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gtbkbpolgz.html

static_cast<double>(a) / b
来源：http://hz.daria6918.cn/gtkhgeajxg.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gthgbtqbfr.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtzubxchuv.html

[S53] C++：移动语义
来源：http://hz.wangdashe.top/gtvfteczdx.html

std::vector<int> w = std::move(v);
来源：http://hz.haohaochexian.top/gtnlccpxwi.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtiuegooof.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guowangkeji.top/gtemhrymbj.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtummdekqt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtbrmfoxtf.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gtibgclayu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhengqikj.top/gtboetsmsk.html

[S57] C++：编译期常量
来源：http://hz.redwolf501.top/gtxessuhhc.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtmgzocqtn.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtngigtums.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258888.top/gtyvuilqoc.html

[S59] C++：静态断言
来源：http://hz.yanxiufei.cn/gtorgvyrgm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtkyfhnxrb.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtgzassiuj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nanxinkj.top/gtfqznwnvr.html

================================================================================
来源：http://hz.sxryk.cn/gtriqckeho.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtxcfynwoe.html

================================================================================
来源：http://hz.svipenyu.cn/gtcgvlfpld.html

[T01] Kotlin：Hello World
来源：http://hz.yongpay.top/gtkddhfeca.html

println("Hello")
来源：http://hz.shuidangran.top/gtqzrxrfdt.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtikwergab.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cashguo.top/gtaugyexzf.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtvxzcpunt.html

"值: $b"
来源：http://hz.yonumen.top/gttuaxzwej.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtgzojuyrw.html

val n: String? = null;  n?.length
来源：http://hz.zhongyouzk.top/gtqmwztcyo.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtcmjigpfm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gotoacloud.top/gtoaxemdcu.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtbyhmcfjt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.daria6918.cn/gttdawgpgn.html

[T07] Kotlin：集合过滤
来源：http://hz.dianchejie.cn/gtnewxpoqr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.mhx1999.top/gtrswjxcsq.html

[T08] Kotlin：数据类
来源：http://hz.aibaodan.cn/gtryelxmpm.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtfmkvdfou.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gtxrwocddm.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gtuwjerjhy.html

[T10] Kotlin：默认参数
来源：http://hz.zhixingplan.top/gtjivzdlba.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtqthirgrw.html

[T11] Kotlin：协程
来源：http://hz.feifeiyinyue.top/gtzjpnblvn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zdqjudy.top/gtvheoukat.html

[T12] Kotlin：解构声明
来源：http://hz.cdnleiting.top/gtusqsjfpu.html

val (a, b) = Pair(1, 2)
来源：http://hz.zdqjudy.top/gtulozdtup.html

[T13] Kotlin：只读 Map
来源：http://hz.dianchejie.cn/gtttfwxqii.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtbvbqvyvb.html

[T14] Kotlin：循环
来源：http://hz.bjfxy.top/gtpoxoncyl.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtkaslcrbh.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtzdzjarjq.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtubdwldyg.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtchdwckho.html

print("Hello")
来源：http://hz.guannengcc.top/gtxvivwmxg.html

[T17] Swift：变量与常量
来源：http://hz.yanxiufei.cn/gtwtgsqene.html

var a = 1;  let b = 2
来源：http://hz.jinghuilouyu.cn/gtfgkwwfcx.html

[T18] Swift：字符串插值
来源：http://hz.ivvv.top/gttjtrenip.html

"值: \(b)"
来源：http://hz.316326.xyz/gtlubuscqe.html

[T19] Swift：可选绑定
来源：http://hz.yueranfly.top/gtgllfksnp.html

if let n = opt { print(n) }
来源：http://hz.c1oappe.top/gthxweqzor.html

[T20] Swift：数组操作
来源：http://hz.gaohongyu789.top/gttgzdpnii.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtewxblwpr.html

[T21] Swift：遍历
来源：http://hz.hywenlv.cn/gtiiykabao.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtonvwlgcd.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtnfsydyem.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuanzx.com/gtgblkgcha.html

[T23] Swift：函数
来源：http://hz.wangshuangyany.cn/gtbqwlookf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgufenzy.top/gtjmbtcqus.html

[T24] Swift：闭包
来源：http://hz.vqdsnc.cn/gtqjsxylpl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtkezuiorz.html

[T25] Swift：结构体
来源：http://hz.quarkkingdee.top/gtfhkepdbn.html

struct P { var x: Int }
来源：http://hz.gogol.net.cn/gtaqomuaou.html

[T26] Swift：类与重写
来源：http://hz.hywenlv.cn/gtgyownzgf.html

class A: Base { override func f() {} }
来源：http://hz.xingfuxueyuan.xyz/gtaywnihev.html

[T27] Swift：错误处理
来源：http://hz.quarkkingdee.top/gtinchxnqc.html

do { try f() } catch { print(error) }
来源：http://hz.jiagoushi.top/gtkgmgssdx.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtlvzvmswb.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtgbpsrnes.html

[T29] Swift：guard 提前返回
来源：http://hz.aizwys.cn/gtajmtcrxp.html

guard let x = opt else { return }
来源：http://hz.hnqzz.top/gtzljtbtqy.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gttnbsekaf.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtcvwzipvp.html

[T31] Lua：Hello World
来源：http://hz.wangshuangyany.cn/gtjyajtfnq.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtpjjiaciz.html

[T32] Lua：局部变量
来源：http://hz.ybcxt.top/gtcqgzleog.html

local a = 1
来源：http://hz.gogol.net.cn/gtfmnehncp.html

[T33] Lua：表（数组）
来源：http://hz.xinyue.icu/gtetmjhric.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zycfv.cn/gtderswred.html

[T34] Lua：遍历表
来源：http://hz.zdqjudy.top/gtetzjatlx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.smart0.xyz/gtuofuonjd.html

[T35] Lua：字典表
来源：http://hz.zdqjudy.top/gtsgnsymyv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.52xcode.cn/gtuhjdsmnp.html

[T36] Lua：函数
来源：http://hz.wangdashe.top/gtyncznork.html

function add(a, b) return a + b end
来源：http://hz.zhongyouzk.top/gtckgmunco.html

[T37] Lua：字符串拼接
来源：http://hz.zhiwuduotai.top/gtyycthpct.html

"a" .. "b"
来源：http://hz.gotoacloud.top/gtnryhjkoc.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gtufflqzxl.html

if x > 0 then print("正") end
来源：http://hz.316326.xyz/gtgrrnwjkl.html

[T39] Lua：模式匹配
来源：http://hz.jinyuanbaomall.cn/gtigvppvst.html

string.find(s, "%d+")
来源：http://hz.fengsongda.top/gtbgisasuj.html

[T40] Lua：元表
来源：http://hz.jyoumei.cn/gtcmbqdxna.html

setmetatable({}, { __index = base })
来源：http://hz.zhixingplan.top/gtpwqmqjym.html

[T41] Perl：Hello World
来源：http://hz.zhijiandao.cn/gtnuhjjvfa.html

print "Hello\n";
来源：http://hz.havefunace.top/gthvslbyfb.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtlcndnzta.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.quarkkingdee.top/gtsbyjjctt.html

[T43] Perl：字符串插值
来源：http://hz.yvedp.cn/gtvcufrxej.html

"值: $a"
来源：http://hz.fengsongda.top/gtvaruddxi.html

[T44] Perl：条件
来源：http://hz.shzxlz.cn/gtevolxdqk.html

if ($a > 0) { print "正"; }
来源：http://hz.yj202588.top/gtmarskqku.html

[T45] Perl：数组遍历
来源：http://hz.yueranfly.top/gtwpivhenm.html

for my $x (@arr) { print $x; }
来源：http://hz.c1oappe.top/gteghdrhrn.html

[T46] Perl：哈希操作
来源：http://hz.iojbl.cn/gtqvacpysu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shanyushiyangtech.top/gtfwhcpurz.html

[T47] Perl：正则捕获
来源：http://hz.zhoulong.xyz/gtertkjsjd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.chenzaomai.com/gtwoyjyzye.html

[T48] Perl：正则替换
来源：http://hz.sufxvd.cn/gtqcwgmfil.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtkvtieqjy.html

[T49] Perl：函数
来源：http://hz.nwbrower.top/gtmxuuzaqt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtjxzbcgnu.html

[T50] Perl：逐行读文件
来源：http://hz.fengsongda.top/gtfaakbgkh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fengsongda.top/gtxabhzyeh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnxiangtu.top/gtsfmvzceg.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtqvagovfe.html

println("Hello")
来源：http://hz.zycfv.cn/gtttlwutki.html

[T52] Scala：变量
来源：http://hz.haohaochexian.top/gtshjxrskw.html

val a = 1;  var b = 2
来源：http://hz.chenjidiqi.icu/gtrooktonx.html

[T53] Scala：字符串插值
来源：http://hz.gogol.net.cn/gtjukkjhtk.html

s"值: $b"
来源：http://hz.c1oappe.top/gtcihlarrh.html

[T54] Scala：集合映射
来源：http://hz.feifeiyinyue.top/gtjxfwzvhn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.guannengcc.top/gtvkyxxtxs.html

[T55] Scala：集合过滤
来源：http://hz.redwolf501.top/gtufzbzahk.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtabldaqfz.html

[T56] Scala：样例类
来源：http://hz.gogol.net.cn/gtjeymhkol.html

case class User(name: String, age: Int)
来源：http://hz.dianchejie.cn/gtsmubiuaj.html

[T57] Scala：模式匹配
来源：http://hz.c1oappe.top/gtzwkjgyho.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.haohaochexian.top/gtcljtmbau.html

[T58] Scala：函数定义
来源：http://hz.aizwys.cn/gtuyrnyqot.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gtgpzmjkra.html

[T59] Scala：循环
来源：http://hz.yuanzhike.top/gtmmfvrmwt.html

for (i <- 1 to 10) println(i)
来源：http://hz.quarkkingdee.top/gtvmdnraeo.html

[T60] Scala：折叠
来源：http://hz.vqdsnc.cn/gtjebyylhn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.pengpengdd.cyou/gtdlwyyfto.html

================================================================================
来源：http://hz.dashuyun.cn/gtverdyhlr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cdnleiting.top/gtmhfbhjxe.html

================================================================================
来源：http://hz.ydzc1.top/gtoemurwmf.html

[U01] Py：创建虚拟环境
来源：http://hz.zhoulong.xyz/gtgdsetwvz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xinyue.icu/gthgkfubah.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gteohpnhgp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hongshengwenyu.top/gteglmqzmf.html

[U03] Py：加载 .env 配置
来源：http://hz.shuidangran.top/gtoqgzzuop.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhixingplan.top/gtunwrxctb.html

[U04] Py：变量调试打印
来源：http://hz.guannengcc.top/gtsfuvfotc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.andypj.xyz/gtzmpomaia.html

[U05] Py：列表去重且保序
来源：http://hz.gogol.net.cn/gtgssnnyye.html

list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gthvkbfprd.html

[U06] Py：合并两个字典
来源：http://hz.hywenlv.cn/gtkanpfybj.html

{**a, **b}
来源：http://hz.hnxiangtu.top/gtcqyncjls.html

[U07] Py：反转字典键值
来源：http://hz.cdnleiting.top/gtfqacjccy.html

{v: k for k, v in d.items()}
来源：http://hz.aibaodan.cn/gtpcppbnww.html

[U08] Py：展平二维列表
来源：http://hz.ydzc1.top/gtuarlstsv.html

[y for x in nested for y in x]
来源：http://hz.shzxlz.cn/gttebcquow.html

[U09] Py：字典取最大值的键
来源：http://hz.zhaomingkeji.xyz/gtpivfuxtm.html

max(d, key=d.get)
来源：http://hz.sysykeji.top/gtqiyljeww.html

[U10] Py：按值排序字典
来源：http://hz.sweek.top/gtevdgosiy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sxryk.cn/gtfjwmtjov.html

[U11] Py：生成器表达式
来源：http://hz.hfpthk.cn/gtwazeruzy.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gttawfxvuq.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ehwqpu.com/gtjgdlpvlg.html

Counter(arr).most_common(3)
来源：http://hz.yanxiufei.cn/gtablwqhxf.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gtmkfgbzph.html

deque(maxlen=10)
来源：http://hz.sweek.top/gtjttdbtfc.html

[U14] Py：分组收集到列表
来源：http://hz.haohaochexian.top/gtkojmfpgn.html

defaultdict(list)
来源：http://hz.vqdsnc.cn/gteefatswi.html

[U15] Py：高精度计时
来源：http://hz.0kj1m.cn/gtkwxpfjmd.html

t = time.perf_counter()
来源：http://hz.nanxinkj.top/gtbwahzucs.html

[U16] Py：命令行参数解析
来源：http://hz.yongpay.top/gttrqqiiks.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.meibo888.top/gttebksupa.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtbtqoykvd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gtbfeheezl.html

[U18] Py：预编译正则
来源：http://hz.hywenlv.cn/gtdaewfdou.html

pat = re.compile(r"\d+")
来源：http://hz.cdnleiting.top/gtlhzcsuex.html

[U19] Py：正则替换带回调
来源：http://hz.meibo888.top/gtllzbznjb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pycfn.com/gtpesqbpvr.html

[U20] Py：缓存函数结果
来源：http://hz.pycfn.com/gtjatenlde.html

@functools.lru_cache(maxsize=None)
来源：http://hz.redwolf501.top/gtxjlvpkvk.html

[U21] Py：自定义上下文管理器
来源：http://hz.tianlin.xyz/gtakknmesd.html

@contextlib.contextmanager
来源：http://hz.yangfankeji.com/gtkqpwrhmh.html

[U22] Py：矩阵转置
来源：http://hz.jinqigufen.top/gtfhhlmsnz.html

list(zip(*m))
来源：http://hz.guannengcc.top/gtwdeeabxs.html

[U23] Py：分块读取大文件
来源：http://hz.ywan-chungtsiang.top/gtawpxduta.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhoulong.xyz/gtnkztgmax.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangkeji.top/gtvqrscnxu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtmjjozeqi.html

[U25] Py：CSV 按字典读
来源：http://hz.nanxinkj.top/gtrnkskxbd.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtkqzhodfx.html

[U26] Py：并发下载
来源：http://hz.yueranfly.top/gtviwrcdwm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xziqi.cn/gtzoncvqvj.html

[U27] Py：异步 HTTP
来源：http://hz.ywan-chungtsiang.top/gtpuxnouut.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.daria6918.cn/gtltbcrets.html

[U28] Py：类型别名
来源：http://hz.hnxiangtu.top/gtmewcvdur.html

UserId = int
来源：http://hz.pycfn.com/gtulppntqd.html

[U29] Py：属性校验
来源：http://hz.dashuyun.cn/gtozkumebo.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtfbnhixjk.html

[U30] Py：数据类
来源：http://hz.tian-w.cn/gtrzpyogjm.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gteyteravt.html

[U31] Py：单测
来源：http://hz.cheryme.top/gtgkixqpxn.html

python -m pytest -q
来源：http://hz.snrcjt.cn/gtilzibgbq.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtunxbpmuj.html

ruff format . && ruff check --fix .
来源：http://hz.gaohongyu789.top/gtvribjygj.html

[U33] Py：打包发布
来源：http://hz.jqgufenzy.top/gtimtjgvwm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shanyushiyangtech.top/gtwklsuxoa.html

[U34] Py：判断编码
来源：http://hz.nanxinkj.top/gthychizum.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gtacngnphu.html

[U35] Py：发送邮件
来源：http://hz.xziqi.cn/gtcfeofqvb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.daxiang520.top/gthddglkmc.html

[U36] Py：定时任务
来源：http://hz.sysykeji.top/gtioqmmfkr.html

schedule.every(10).minutes.do(job)
来源：http://hz.chenjidiqi.icu/gtjpfsdazb.html

[U37] Py：读写 Excel
来源：http://hz.snrcjt.cn/gtmnvceeyy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xinyue.icu/gtmreubsjn.html

[U38] Py：获取脚本所在目录
来源：http://hz.316326.xyz/gtkzzcqevr.html

Path(__file__).resolve().parent
来源：http://hz.guowangkeji.top/gtaratymfn.html

[U39] Py：判断是否在交互环境
来源：http://hz.zdqjudy.top/gtzoxxyuty.html

sys.stdout.isatty()
来源：http://hz.andypj.xyz/gtuyhoehhd.html

[U40] Py：打印到标准错误
来源：http://hz.jianghu66.top/gtinpfummw.html

print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtyuvihvqj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.bjfxy.top/gthmiiaafu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtimhccsvg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtfsoehwbq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yangfankeji.com/gthtsdfgys.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtuncvfjvl.html

namespace App\Http;
来源：http://hz.yangfankeji.com/gttkjxebhs.html

[U44] PHP：开启严格类型
来源：http://hz.xinyue.icu/gtbuwmaaoh.html

declare(strict_types=1);
来源：http://hz.cqqwz.cn/gtnhlsislr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ywan-chungtsiang.top/gthpkgwnwg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtxmlxfauy.html

[U46] PHP：可空类型
来源：http://hz.jlsjyb.cn/gthlgsbexd.html

?string $name = null
来源：http://hz.pengpengdd.cyou/gtzjfznixr.html

[U47] PHP：联合类型
来源：http://hz.gogol.net.cn/gttedswhjr.html

int|string $id
来源：http://hz.shuidangran.top/gtfwfgiaut.html

[U48] PHP：纯枚举
来源：http://hz.dianchejie.cn/gtjkybxnll.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.tian-w.cn/gtsexgjjpj.html

[U49] PHP：只读属性
来源：http://hz.redwolf501.top/gtdkrpwqva.html

public readonly string $name
来源：http://hz.snrcjt.cn/gtjlkpnuaz.html

[U50] PHP：构造器属性提升
来源：http://hz.xuanzx.com/gtggajzbfr.html

public function __construct(private int $id) {}
来源：http://hz.ybcxt.top/gtzbodismr.html

[U51] PHP：数组解构
来源：http://hz.iojbl.cn/gtfxakfwng.html

[$a, $b] = $arr;
来源：http://hz.zhiwuduotai.top/gtolnwnobo.html

[U52] PHP：箭头函数
来源：http://hz.svipenyu.cn/gtmvyatjur.html

$double = fn($x) => $x * 2;
来源：http://hz.shangyingyoupin.top/gtoicedrvl.html

[U53] PHP：空合并运算符
来源：http://hz.haohaochexian.top/gtnakjprbe.html

$v = $a ?? $b ?? "default";
来源：http://hz.sxryk.cn/gtufyttnvw.html

[U54] PHP：空安全调用
来源：http://hz.jinqigufen.top/gtdyfozwqj.html

$obj?->method()
来源：http://hz.gogol.net.cn/gtnttlldro.html

[U55] PHP：match 表达式
来源：http://hz.cashguo.top/gtylirrrtb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ehwqpu.com/gtmjbbffie.html

[U56] PHP：命名参数
来源：http://hz.xylfe.cn/gtqrmxubie.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gtbqdsnpsk.html

[U57] PHP：字符串插值
来源：http://hz.daxiang520.top/gtaxhaktmn.html

"值: {$a}"
来源：http://hz.hfpthk.cn/gtruaifhoa.html

[U58] PHP：数组三件套
来源：http://hz.daria6918.cn/gtznrttnep.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.dashuyun.cn/gtlfjsewux.html

[U59] PHP：自定义排序
来源：http://hz.vqdsnc.cn/gtnjbdajjz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtevapmjta.html

[U60] PHP：JSON 编解码
来源：http://hz.gotoacloud.top/gtlsirwzxc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jiagoushi.top/gtyialwdoy.html

[U61] PHP：正则
来源：http://hz.0kj1m.cn/gtclxzcyso.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtpdddailq.html

[U62] PHP：日期对象
来源：http://hz.cashguo.top/gtmkgebrig.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sweek.top/gtylvnkfmp.html


<!-- 参考信息 -->