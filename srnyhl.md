代发 wailian999

[S35] C++：map
来源：http://hz.snrcjt.cn/gthziwmjjn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtxboyzrgx.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtzjmkpkko.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.haohaochexian.top/gthwxgvcka.html

[S37] C++：set
来源：http://hz.jiagoushi.top/gteirdkbvv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jyoumei.cn/gtwbaunbkj.html

[S38] C++：排序
来源：http://hz.tianlin.xyz/gttdfyeqqr.html

std::sort(v.begin(), v.end());
来源：http://hz.chenjidiqi.icu/gtbdnliyqs.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtscqeqohc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shangyingyoupin.top/gtirojrcqm.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtasxsfizj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gttazdhmhr.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtghifwrmp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgfzy.top/gtslvklxku.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtdafcocmw.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gterntcnnj.html

[S43] C++：智能指针
来源：http://hz.feifeiyinyue.top/gtlheiphmx.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtnvxqfmii.html

[S44] C++：引用传参
来源：http://hz.ivvv.top/gtddafcljh.html

void inc(int &x) { ++x; }
来源：http://hz.gotoacloud.top/gtdeatvrkn.html

[S45] C++：lambda
来源：http://hz.cdnleiting.top/gteshnawrx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.kuanghao11.cn/gthmqbbtnx.html

[S46] C++：函数模板
来源：http://hz.ehwqpu.com/gtflmxcwus.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtykjyzbkc.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtxyxnefrn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtrhmubggm.html

[S48] C++：逐行读文件
来源：http://hz.meibo888.top/gthwxgriqp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gtgwrdgcjh.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtghciaqxc.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtsgmwkhyu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtpmtyrbzl.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtcuodlddl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cashguo.top/gtoitvwxxw.html

[S51] C++：显式类型转换
来源：http://hz.xingfuxueyuan.xyz/gtlxejkqwp.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtuolgdruj.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtbwxcxtaf.html

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gtgmowyxuu.html

[S53] C++：移动语义
来源：http://hz.jlsjyb.cn/gtygbcikuk.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtgoddvvrt.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtidcghpnp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtuhtfxprj.html

[S55] C++：结构化绑定
来源：http://hz.guannengcc.top/gtajsfjjcd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hongshengwenyu.top/gtpatifkvx.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtrhuixwdi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nwbrower.top/gtoxgsumwf.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gtfjugzoyw.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtyieqzqos.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gtfmdzksdj.html

namespace ns { int f() { return 1; } }
来源：http://hz.zdqjudy.top/gtoraqhicg.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtmltkbgfo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gtkbuxukli.html

[S60] C++：遍历并删除元素
来源：http://hz.yueranfly.top/gthswstmwe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtokcabxoo.html

================================================================================
来源：http://hz.yongpay.top/gtklevgxmq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtlngxjttw.html

================================================================================
来源：http://hz.0kj1m.cn/gtzxtbrcvl.html

[T01] Kotlin：Hello World
来源：http://hz.9152youxi.cn/gtseekfdxz.html

println("Hello")
来源：http://hz.yj20258.top/gtxrxtvijy.html

[T02] Kotlin：变量
来源：http://hz.guowangkeji.top/gtpicgwvfd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gttxobzvfj.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxuanxn.top/gtwafthpgc.html

"值: $b"
来源：http://hz.sufxvd.cn/gtkadywpwa.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtbhqavigi.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtndmcsfat.html

[T05] Kotlin：when 表达式
来源：http://hz.sysykeji.top/gtfctmgpte.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtthdmlmob.html

[T06] Kotlin：集合映射
来源：http://hz.chenlongwang.top/gtwvytwwai.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydzc1.top/gtebiecmah.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gtuyseezwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jiagoushi.top/gtkhgvqder.html

[T08] Kotlin：数据类
来源：http://hz.fengsongda.top/gtggdulpph.html

data class User(val name: String, val age: Int)
来源：http://hz.jinyuanbaomall.cn/gtzsdstxtj.html

[T09] Kotlin：扩展函数
来源：http://hz.shangyingyoupin.top/gtoukrsgxp.html

fun String.exclaim() = this + "!"
来源：http://hz.wangshuangyany.cn/gtmyxvyiui.html

[T10] Kotlin：默认参数
来源：http://hz.jianghu66.top/gtwyrllowp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.iojbl.cn/gttipljwmf.html

[T11] Kotlin：协程
来源：http://hz.hnqzz.top/gtjrxumzya.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nwbrower.top/gttyybluqx.html

[T12] Kotlin：解构声明
来源：http://hz.zdqjudy.top/gtkdpyefku.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gtvyzzigcn.html

[T13] Kotlin：只读 Map
来源：http://hz.wangdashe.top/gtszniypvn.html

val m = mapOf("a" to 1)
来源：http://hz.jinyuanbaomall.cn/gtnkqlqrle.html

[T14] Kotlin：循环
来源：http://hz.shangyingyoupin.top/gtedbbbmri.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtoeakoizf.html

[T15] Kotlin：接口
来源：http://hz.hysaishi.cn/gtldcugcab.html

interface Shape { fun area(): Double }
来源：http://hz.sxryk.cn/gtckfoemei.html

[T16] Swift：Hello World
来源：http://hz.sysykeji.top/gtxxzyejpt.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtqjlxdkkt.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtbwlydbyb.html

var a = 1;  let b = 2
来源：http://hz.andypj.xyz/gtcsuksaui.html

[T18] Swift：字符串插值
来源：http://hz.9152youxi.cn/gtxpwnfwqc.html

"值: \(b)"
来源：http://hz.tanke756.top/gtstrkzaos.html

[T19] Swift：可选绑定
来源：http://hz.cheryme.top/gtouqnrugc.html

if let n = opt { print(n) }
来源：http://hz.quarkkingdee.top/gtrekogoms.html

[T20] Swift：数组操作
来源：http://hz.jinqigufen.top/gtdwnmsizm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtmmlgrncs.html

[T21] Swift：遍历
来源：http://hz.yanxiufei.cn/gtljynnwgm.html

for x in a { print(x) }
来源：http://hz.316326.xyz/gtjpadasuq.html

[T22] Swift：字典
来源：http://hz.zhoulong.xyz/gtdvyctewp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.havefunace.top/gtoqbhyfzm.html

[T23] Swift：函数
来源：http://hz.yj20258888.top/gthbsykpqh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtnyrgiroz.html

[T24] Swift：闭包
来源：http://hz.aibaodan.cn/gtftzgvatk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gtobvrqppy.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtsbxhogdf.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gteuayqmok.html

[T26] Swift：类与重写
来源：http://hz.xuanzx.com/gtyjrsfejo.html

class A: Base { override func f() {} }
来源：http://hz.daria6918.cn/gthkttirgd.html

[T27] Swift：错误处理
来源：http://hz.gzhubu.top/gtrdmkrkyg.html

do { try f() } catch { print(error) }
来源：http://hz.pycfn.com/gtnivcfylk.html

[T28] Swift：枚举
来源：http://hz.fengsongda.top/gtqlivtcgo.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gttanlxaiu.html

[T29] Swift：guard 提前返回
来源：http://hz.ydjk.org.cn/gtcsbynhej.html

guard let x = opt else { return }
来源：http://hz.sufxvd.cn/gtfauojetb.html

[T30] Swift：协议
来源：http://hz.fengsongda.top/gtctsmttbz.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtvlwibctr.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gtvowxvirz.html

print("Hello")
来源：http://hz.gogol.net.cn/gtpffepidq.html

[T32] Lua：局部变量
来源：http://hz.jiagoushi.top/gttkjwrgzu.html

local a = 1
来源：http://hz.52xcode.cn/gttktfzdap.html

[T33] Lua：表（数组）
来源：http://hz.birdmap.top/gtvfpwikst.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtsoehsrfb.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtrkdbkpph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.daxiang520.top/gtcxufrbus.html

[T35] Lua：字典表
来源：http://hz.yongpay.top/gtnfugwhmr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gotoacloud.top/gtmynpaazc.html

[T36] Lua：函数
来源：http://hz.shanyushiyangkeji.top/gtildrhfaz.html

function add(a, b) return a + b end
来源：http://hz.guowangkeji.top/gtbdzpahpz.html

[T37] Lua：字符串拼接
来源：http://hz.sweek.top/gtyrpctqku.html

"a" .. "b"
来源：http://hz.nwbrower.top/gtocriesft.html

[T38] Lua：条件
来源：http://hz.hywenlv.cn/gtuqexjfaw.html

if x > 0 then print("正") end
来源：http://hz.wangdashe.top/gtflkhbtyh.html

[T39] Lua：模式匹配
来源：http://hz.guannengcc.top/gtqluzlywi.html

string.find(s, "%d+")
来源：http://hz.ywan-chungtsiang.top/gtemwqfarz.html

[T40] Lua：元表
来源：http://hz.yvedp.cn/gtptsqcdta.html

setmetatable({}, { __index = base })
来源：http://hz.wangdashe.top/gtvtrplyqu.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtlzbvybvx.html

print "Hello\n";
来源：http://hz.yj20258.top/gtevhtotpp.html

[T42] Perl：变量类型
来源：http://hz.fzhhl.top/gtcvtodcov.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guowangkeji.top/gtzwiiiqsr.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gteeisczou.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtpttfdrlw.html

[T44] Perl：条件
来源：http://hz.jinqigfzy.top/gtirtslqey.html

if ($a > 0) { print "正"; }
来源：http://hz.fzhhl.top/gtarujjptn.html

[T45] Perl：数组遍历
来源：http://hz.yuanzhike.top/gtzygxsrve.html

for my $x (@arr) { print $x; }
来源：http://hz.0kj1m.cn/gtggfsckrk.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtlbrbmsws.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhiwuduotai.top/gtwgbgtewd.html

[T47] Perl：正则捕获
来源：http://hz.chenlongwang.top/gtwtcgwjvy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gteoarxfsh.html

[T48] Perl：正则替换
来源：http://hz.xylfe.cn/gtkariflih.html

$s =~ s/old/new/g;
来源：http://hz.52xcode.cn/gtqtvvlfyb.html

[T49] Perl：函数
来源：http://hz.sxryk.cn/gtjtcodktd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtuoaddpou.html

[T50] Perl：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtncfhjyas.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinyuanbaomall.cn/gtozjtxmrg.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yuanzhike.top/gtpxfqpjfh.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gtkooyypek.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtyuedgwis.html

[T52] Scala：变量
来源：http://hz.hongshengwenyu.top/gtqbwbubtt.html

val a = 1;  var b = 2
来源：http://hz.ydjk.org.cn/gtkzrwimes.html

[T53] Scala：字符串插值
来源：http://hz.chenjidiqi.icu/gtuoauixdn.html

s"值: $b"
来源：http://hz.pengpengdd.cyou/gtozxjeasc.html

[T54] Scala：集合映射
来源：http://hz.quarkkingdee.top/gtzhsxhldn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sufxvd.cn/gtrbhmrkwg.html

[T55] Scala：集合过滤
来源：http://hz.c1oappe.top/gtnujhumxj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtdcujwkbf.html

[T56] Scala：样例类
来源：http://hz.redwolf501.top/gtndbnxwvk.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gtfoutqbxf.html

[T57] Scala：模式匹配
来源：http://hz.daria6918.cn/gtfppeyfhs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhaomingkeji.xyz/gtnmjbpssx.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtdueyegmz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.iojbl.cn/gtpdscpxax.html

[T59] Scala：循环
来源：http://hz.mhx1999.top/gtprqpxxfc.html

for (i <- 1 to 10) println(i)
来源：http://hz.c1oappe.top/gtqijjuzhm.html

[T60] Scala：折叠
来源：http://hz.xingfuxueyuan.xyz/gtthelqgyk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.fengsongda.top/gtnsfduhhw.html

================================================================================
来源：http://hz.andypj.xyz/gtjjqbbmyx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.guowangkeji.top/gtullvbytz.html

================================================================================
来源：http://hz.nwbrower.top/gtxelajfia.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtgrcqxwxz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.52xcode.cn/gtngkdpiae.html

[U02] Py：导出 / 安装依赖
来源：http://hz.haohaochexian.top/gtrxqudura.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daria6918.cn/gtcmfzhnat.html

[U03] Py：加载 .env 配置
来源：http://hz.cheryme.top/gteznsgenu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gtzdqepwzq.html

[U04] Py：变量调试打印
来源：http://hz.gaohongyu789.top/gtbdlsscfx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.c1oappe.top/gthbhnwcpw.html

[U05] Py：列表去重且保序
来源：http://hz.yj20258888.top/gtszmbvdul.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtylnviela.html

[U06] Py：合并两个字典
来源：http://hz.redwolf501.top/gtwdkbcede.html

{**a, **b}
来源：http://hz.yuxming.cn/gtjuunqhkz.html

[U07] Py：反转字典键值
来源：http://hz.hnxiangtu.top/gtpfpgwscw.html

{v: k for k, v in d.items()}
来源：http://hz.nanxuanxn.top/gtcokhxwhi.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtjeawnqrn.html

[y for x in nested for y in x]
来源：http://hz.jqgufenzy.top/gtaawxqjvj.html

[U09] Py：字典取最大值的键
来源：http://hz.yangfankeji.com/gtfufxlrro.html

max(d, key=d.get)
来源：http://hz.xziqi.cn/gtvhahwmuo.html

[U10] Py：按值排序字典
来源：http://hz.pengpengdd.cyou/gtdapabrfm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cdnleiting.top/gtmpalqrsb.html

[U11] Py：生成器表达式
来源：http://hz.hongshengwenyu.top/gtjsqjpheh.html

(x * 2 for x in arr)
来源：http://hz.guowangkeji.top/gtyhqrzafg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj202588.top/gtadbaxjzr.html

Counter(arr).most_common(3)
来源：http://hz.jianghu66.top/gtjnawlicp.html

[U13] Py：固定长度队列
来源：http://hz.hammf.cn/gtabmhvplw.html

deque(maxlen=10)
来源：http://hz.cqqwz.cn/gtjtggkhei.html

[U14] Py：分组收集到列表
来源：http://hz.cheryme.top/gtkbgupsnq.html

defaultdict(list)
来源：http://hz.birdmap.top/gtwnxxvfnt.html

[U15] Py：高精度计时
来源：http://hz.yvedp.cn/gtizrdytvi.html

t = time.perf_counter()
来源：http://hz.chenzaomai.com/gtfensodoz.html

[U16] Py：命令行参数解析
来源：http://hz.shuidangran.top/gtkqmltsle.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sweek.top/gtxqhygcrc.html

[U17] Py：初始化日志
来源：http://hz.9152youxi.cn/gtsrzgmuhz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jianghu66.top/gtxpvztags.html

[U18] Py：预编译正则
来源：http://hz.pycfn.com/gtofwkuonj.html

pat = re.compile(r"\d+")
来源：http://hz.jinyuanbaomall.cn/gtfhsprccp.html

[U19] Py：正则替换带回调
来源：http://hz.yonumen.top/gtrqrddwei.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhengqikj.top/gttgiscljg.html

[U20] Py：缓存函数结果
来源：http://hz.andypj.xyz/gtaktagiid.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xziqi.cn/gtumfbpwrg.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinghuilouyu.cn/gtqrdtitix.html

@contextlib.contextmanager
来源：http://hz.zhaomingkeji.xyz/gtcuudgsbw.html

[U22] Py：矩阵转置
来源：http://hz.hysaishi.cn/gtoopwtkib.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtoqqeskbm.html

[U23] Py：分块读取大文件
来源：http://hz.jyoumei.cn/gtifaqhzrp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.svipenyu.cn/gtkrljxdcp.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtkwffdftb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtzcguevfs.html

[U25] Py：CSV 按字典读
来源：http://hz.chenlongwang.top/gtwjfnrhnj.html

csv.DictReader(f)
来源：http://hz.yj20258.top/gtffrimbxh.html

[U26] Py：并发下载
来源：http://hz.xuanzx.com/gtxtbhdkxs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.snrcjt.cn/gtsaghmrmu.html

[U27] Py：异步 HTTP
来源：http://hz.andypj.xyz/gtjxkusbjr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtpxplzmsb.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtwmwfzpjb.html

UserId = int
来源：http://hz.daria6918.cn/gtkrucfvvc.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gttpetnlvg.html

@property 与 @x.setter 配合
来源：http://hz.kuanghao11.cn/gtyfutflzj.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtwskskosn.html

@dataclass(slots=True)
来源：http://hz.jqgufenzy.top/gtnzqawdgb.html

[U31] Py：单测
来源：http://hz.shangyingyoupin.top/gtpuogdamu.html

python -m pytest -q
来源：http://hz.svipenyu.cn/gtljuwmoed.html

[U32] Py：代码格式化
来源：http://hz.jqgfzy.top/gtbieehixc.html

ruff format . && ruff check --fix .
来源：http://hz.jqgfzy.top/gtcjpdfszp.html

[U33] Py：打包发布
来源：http://hz.zhijiandao.cn/gtkrviadsz.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gzhubu.top/gtdsuxnovv.html

[U34] Py：判断编码
来源：http://hz.ywan-chungtsiang.top/gtveiozrdv.html

chardet.detect(raw)
来源：http://hz.shzxlz.cn/gtabyjumzz.html

[U35] Py：发送邮件
来源：http://hz.sxryk.cn/gtumctzdca.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.guowangkeji.top/gtlrbqxvzn.html

[U36] Py：定时任务
来源：http://hz.aibaodan.cn/gtbejqzyxo.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gttsphgdkl.html

[U37] Py：读写 Excel
来源：http://hz.jinqigfzy.top/gtzgzhppnf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cheryme.top/gttkyxkano.html

[U38] Py：获取脚本所在目录
来源：http://hz.ydzc1.top/gtpxdwwadp.html

Path(__file__).resolve().parent
来源：http://hz.nwbrower.top/gtvmzvnhos.html

[U39] Py：判断是否在交互环境
来源：http://hz.guowangkeji.top/gtiwifuvkg.html

sys.stdout.isatty()
来源：http://hz.gzhubu.top/gtayugaxce.html

[U40] Py：打印到标准错误
来源：http://hz.aizwys.cn/gtsrnmbdgx.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtaqtiubmx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yonumen.top/gtszkmbqve.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xingfuxueyuan.xyz/gtqegwrrpj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtxdswpeib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhixingplan.top/gtdcsagwfa.html

[U43] PHP：声明命名空间
来源：http://hz.yanxiufei.cn/gtfdxlzydd.html

namespace App\Http;
来源：http://hz.ydzc1.top/gtqlvsitmc.html

[U44] PHP：开启严格类型
来源：http://hz.nanxinkj.top/gtiodovbpo.html

declare(strict_types=1);
来源：http://hz.haohaochexian.top/gtlqmzmdgn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.c1oappe.top/gtxnvjbflv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtmzhspfci.html

[U46] PHP：可空类型
来源：http://hz.guowangkeji.top/gtvvdescwz.html

?string $name = null
来源：http://hz.zhongyouzk.top/gtjyxtqanb.html

[U47] PHP：联合类型
来源：http://hz.aibaodan.cn/gtwawlkbmm.html

int|string $id
来源：http://hz.hfpthk.cn/gtljdylhez.html

[U48] PHP：纯枚举
来源：http://hz.zhongyouzk.top/gthbwyhpca.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.pycfn.com/gtqtmghbnw.html

[U49] PHP：只读属性
来源：http://hz.xinyue.icu/gtpnqfsynr.html

public readonly string $name
来源：http://hz.jinqigufen.top/gtiumkkfen.html

[U50] PHP：构造器属性提升
来源：http://hz.svipenyu.cn/gtszauerfw.html

public function __construct(private int $id) {}
来源：http://hz.guowangkeji.top/gtjvufztpq.html

[U51] PHP：数组解构
来源：http://hz.andypj.xyz/gttgpsbknx.html

[$a, $b] = $arr;
来源：http://hz.hfpthk.cn/gtdiussnfn.html

[U52] PHP：箭头函数
来源：http://hz.bjfxy.top/gtealrxqmj.html

$double = fn($x) => $x * 2;
来源：http://hz.jlsjyb.cn/gtideweecs.html

[U53] PHP：空合并运算符
来源：http://hz.jyoumei.cn/gtojfhisaf.html

$v = $a ?? $b ?? "default";
来源：http://hz.yvedp.cn/gtkeuhpfqp.html

[U54] PHP：空安全调用
来源：http://hz.ydjk.org.cn/gtkqbpntgh.html

$obj?->method()
来源：http://hz.yj20258.top/gteskxuwzt.html

[U55] PHP：match 表达式
来源：http://hz.xuetiantiany.cn/gtobpwpdqr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sweek.top/gtesjwlout.html

[U56] PHP：命名参数
来源：http://hz.cashguo.top/gtykfjrqsc.html

f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtrjkettsh.html

[U57] PHP：字符串插值
来源：http://hz.pycfn.com/gtdtfsbbgo.html

"值: {$a}"
来源：http://hz.xuanzx.com/gtrdgnhikb.html

[U58] PHP：数组三件套
来源：http://hz.316326.xyz/gtmbiuanib.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aizwys.cn/gtehvadved.html

[U59] PHP：自定义排序
来源：http://hz.svipenyu.cn/gtpofjfejt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtbbthsdrn.html

[U60] PHP：JSON 编解码
来源：http://hz.ppjwa.cn/gtunpfwfqi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhijiandao.cn/gtuttontjs.html


<!-- 参考信息 -->