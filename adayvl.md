代发 wailian999

[S33] C++：vector 增删
来源：http://hz.ydzc1.top/gtljsyapxt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtnaemkwsb.html

[S34] C++：遍历 vector
来源：http://hz.9152youxi.cn/gtlmkdshhl.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cashguo.top/gtbdffmdkw.html

[S35] C++：map
来源：http://hz.aizwys.cn/gteyvqdfje.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtehdsoacn.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtawwikfwb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gtxzxcnfov.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtkvpxyolt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtglismjwx.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gtwumroqjy.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtlqeehujl.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtoldcbpkw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yangfankeji.com/gtnpynmfxj.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtmeaausdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gturfuhyvd.html

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gtbhqzvbup.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tanke756.top/gtnuntkpqu.html

[S42] C++：继承与虚函数
来源：http://hz.nanxinkj.top/gtugbaccpf.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj202588.top/gtvkbjqhpi.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtolgowwzq.html

auto p = std::make_unique<int>(5);
来源：http://hz.dashuyun.cn/gtiovqnuqg.html

[S44] C++：引用传参
来源：http://hz.yangfankeji.com/gtkozifatp.html

void inc(int &x) { ++x; }
来源：http://hz.xziqi.cn/gtsuqgaoyd.html

[S45] C++：lambda
来源：http://hz.cdnleiting.top/gtueimzjhc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fzhhl.top/gtowkzsdps.html

[S46] C++：函数模板
来源：http://hz.cucudq.cn/gtkanmvlft.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.52xcode.cn/gtkpnrauup.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gtkuhqbxei.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtpjufodzs.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtmzpvmcsi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhengqikj.top/gtzuqkxoxr.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gtgqeqmjqe.html

[S49] C++：写文件
来源：http://hz.ehwqpu.com/gtyoxiccpm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ehwqpu.com/gtcubaxgec.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtijjpqwnw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtatisjhbk.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtnlethtmd.html

static_cast<double>(a) / b
来源：http://hz.quarkkingdee.top/gtwmxsocen.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtlhsvuufk.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtunwhecgc.html

[S53] C++：移动语义
来源：http://hz.gotoacloud.top/gtdjxaayzq.html

std::vector<int> w = std::move(v);
来源：http://hz.zhongyouzk.top/gtmdgfumyx.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gttbsngoft.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.bjfxy.top/gtwbukkvjp.html

[S55] C++：结构化绑定
来源：http://hz.bjfxy.top/gtcpyuhwtx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cashguo.top/gtezurkccl.html

[S56] C++：optional
来源：http://hz.cheryme.top/gtdyftcpwn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.meibo888.top/gtuncweise.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gtdzbkgquf.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtgnztpbqf.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtjpymvhxf.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtccawntvk.html

[S59] C++：静态断言
来源：http://hz.feifeiyinyue.top/gtzkyhhxhw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtwztysadl.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtfvchomgc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nwbrower.top/gtvlmwfjda.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlejsbewc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtnbrwbqfq.html

================================================================================
来源：http://hz.ybcxt.top/gtpkdbzpkl.html

[T01] Kotlin：Hello World
来源：http://hz.yvedp.cn/gtrxmgscpn.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtyobscmko.html

[T02] Kotlin：变量
来源：http://hz.aizwys.cn/gtzjffxsuf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guannengcc.top/gtdjhzqikw.html

[T03] Kotlin：字符串模板
来源：http://hz.daria6918.cn/gtjrpzjxif.html

"值: $b"
来源：http://hz.havefunace.top/gtbegenynp.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtvaloqian.html

val n: String? = null;  n?.length
来源：http://hz.ivvv.top/gtylsvmphx.html

[T05] Kotlin：when 表达式
来源：http://hz.yuanzhike.top/gtrjgowqff.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aizwys.cn/gtjyspdyef.html

[T06] Kotlin：集合映射
来源：http://hz.ywan-chungtsiang.top/gtgdnvcmdc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtmtbnkcvq.html

[T07] Kotlin：集合过滤
来源：http://hz.quarkkingdee.top/gtmcodpiuc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtwljgqdum.html

[T08] Kotlin：数据类
来源：http://hz.ywan-chungtsiang.top/gtupqdlnvt.html

data class User(val name: String, val age: Int)
来源：http://hz.wangdashe.top/gtyjgadvee.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtttrgbjvk.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtaomjzggg.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258.top/gtjjeofubu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cqqwz.cn/gtywltuesq.html

[T11] Kotlin：协程
来源：http://hz.xziqi.cn/gtvpaclxry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ybcxt.top/gtesxxyacb.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtfsdtihyh.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhijiandao.cn/gtbxczuals.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtypkzqrnn.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtexypifrx.html

[T14] Kotlin：循环
来源：http://hz.hysaishi.cn/gtpvpseoap.html

for (i in 1..10) println(i)
来源：http://hz.0kj1m.cn/gtpkmwnkxq.html

[T15] Kotlin：接口
来源：http://hz.zycfv.cn/gtlewywulk.html

interface Shape { fun area(): Double }
来源：http://hz.aibaodan.cn/gtuugpipcm.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtktxmzdgz.html

print("Hello")
来源：http://hz.mhx1999.top/gtdzlngrhp.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gtospzyjsq.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtqzgppmft.html

[T18] Swift：字符串插值
来源：http://hz.jqgufenzy.top/gtzjppotgo.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtibviqggu.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gtjyrmnkkj.html

if let n = opt { print(n) }
来源：http://hz.wangshuangyany.cn/gtfoctrnnr.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtwdqlnaqa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangkeji.top/gtxvnrqdxs.html

[T21] Swift：遍历
来源：http://hz.redwolf501.top/gtmwzounut.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtvgeskfkv.html

[T22] Swift：字典
来源：http://hz.smart0.xyz/gtqadlsahk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xuanzx.com/gtirvvmcjv.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtoeirijpv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.smart0.xyz/gtckbbhbcx.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtsadnkezm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtcpclybxa.html

[T25] Swift：结构体
来源：http://hz.316326.xyz/gtgfodsubc.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtxzcivdel.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangkeji.top/gtsymisgtf.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gtnquygbiw.html

[T27] Swift：错误处理
来源：http://hz.hongshengwenyu.top/gtxcrjlcge.html

do { try f() } catch { print(error) }
来源：http://hz.haohaochexian.top/gthztcciwj.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gtenyrelbe.html

enum Color { case red, green }
来源：http://hz.dashuyun.cn/gtssckefji.html

[T29] Swift：guard 提前返回
来源：http://hz.shanyushiyangkeji.top/gtnwnbkddn.html

guard let x = opt else { return }
来源：http://hz.fengsongda.top/gtekzsaeas.html

[T30] Swift：协议
来源：http://hz.dashuyun.cn/gtqtetsaqd.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgufenzy.top/gtrnukhlaj.html

[T31] Lua：Hello World
来源：http://hz.fengsongda.top/gtsvfpiciq.html

print("Hello")
来源：http://hz.jyoumei.cn/gtxhunnadc.html

[T32] Lua：局部变量
来源：http://hz.gotoacloud.top/gtsewazxpc.html

local a = 1
来源：http://hz.gaohongyu789.top/gtkqpulnzg.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtjlzqqaga.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yuxming.cn/gtdkgjzhmj.html

[T34] Lua：遍历表
来源：http://hz.kuanghao11.cn/gthhgrxsbq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shangyingyoupin.top/gtxtomrewo.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtqxkqydhd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhiwuduotai.top/gtpbcsfsbv.html

[T36] Lua：函数
来源：http://hz.jinyuanbaomall.cn/gtnlfoalor.html

function add(a, b) return a + b end
来源：http://hz.birdmap.top/gtzyotqect.html

[T37] Lua：字符串拼接
来源：http://hz.ybcxt.top/gtjreuescp.html

"a" .. "b"
来源：http://hz.meibo888.top/gttxtnolxa.html

[T38] Lua：条件
来源：http://hz.gaohongyu789.top/gtjfbzgxlu.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtxfqexjyg.html

[T39] Lua：模式匹配
来源：http://hz.shzxlz.cn/gtrhgyxtce.html

string.find(s, "%d+")
来源：http://hz.ivvv.top/gtniynxzlt.html

[T40] Lua：元表
来源：http://hz.ppjwa.cn/gtpgyrvrvg.html

setmetatable({}, { __index = base })
来源：http://hz.guannengcc.top/gthvbfwift.html

[T41] Perl：Hello World
来源：http://hz.birdmap.top/gtibjcgofe.html

print "Hello\n";
来源：http://hz.wangshuangyany.cn/gtgadmkoce.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtrdzcgbak.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhengqikj.top/gtoztoniyv.html

[T43] Perl：字符串插值
来源：http://hz.meibo888.top/gtkmahcisd.html

"值: $a"
来源：http://hz.ydjk.org.cn/gtjyytgkxt.html

[T44] Perl：条件
来源：http://hz.jqgufenzy.top/gtzzyxiodu.html

if ($a > 0) { print "正"; }
来源：http://hz.0kj1m.cn/gtnjzorhsl.html

[T45] Perl：数组遍历
来源：http://hz.jlsjyb.cn/gtcuzgqezs.html

for my $x (@arr) { print $x; }
来源：http://hz.bjfxy.top/gtriodfukz.html

[T46] Perl：哈希操作
来源：http://hz.9152youxi.cn/gtkploethf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.redwolf501.top/gtzyxkxfca.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtimjmvpvy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hywenlv.cn/gtatwzcqvy.html

[T48] Perl：正则替换
来源：http://hz.gzhubu.top/gtudcafzbd.html

$s =~ s/old/new/g;
来源：http://hz.zdqjudy.top/gtdmnskukt.html

[T49] Perl：函数
来源：http://hz.andypj.xyz/gtabjrjpol.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.redwolf501.top/gtscxetrkf.html

[T50] Perl：逐行读文件
来源：http://hz.quarkkingdee.top/gtwjwjfthd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ppjwa.cn/gtfhembyia.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.quarkkingdee.top/gtcxednrdp.html

[T51] Scala：Hello World
来源：http://hz.hongshengwenyu.top/gtlxgzqgqp.html

println("Hello")
来源：http://hz.zhixingplan.top/gtrudrrwgw.html

[T52] Scala：变量
来源：http://hz.jinghuilouyu.cn/gtuoivkpms.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtfzqifqyr.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gtxgvdctlu.html

s"值: $b"
来源：http://hz.snrcjt.cn/gtrybzgjxh.html

[T54] Scala：集合映射
来源：http://hz.zhaomingkeji.xyz/gtuylqvqvd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenlongwang.top/gtiqqadevr.html

[T55] Scala：集合过滤
来源：http://hz.havefunace.top/gtveyrjnlt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yanxiufei.cn/gtnjdgvjwr.html

[T56] Scala：样例类
来源：http://hz.hysaishi.cn/gtalavvwjs.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gtngmmjndn.html

[T57] Scala：模式匹配
来源：http://hz.yongpay.top/gtldipbdom.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigufen.top/gtstgzsgot.html

[T58] Scala：函数定义
来源：http://hz.dianchejie.cn/gtcyrylzfb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yuxming.cn/gtibvhzkvt.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtigslfaie.html

for (i <- 1 to 10) println(i)
来源：http://hz.cqqwz.cn/gtzemxzcjh.html

[T60] Scala：折叠
来源：http://hz.sufxvd.cn/gtzmewfkby.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gaohongyu789.top/gtaluwvked.html

================================================================================
来源：http://hz.shuidangran.top/gtfqwywdna.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhongyouzk.top/gtyrbgwrrf.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjgbzjesf.html

[U01] Py：创建虚拟环境
来源：http://hz.hammf.cn/gtqhdvvcnn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ywan-chungtsiang.top/gtpolghzkn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258888.top/gtazkmkikf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jqgfzy.top/gtewgyfruk.html

[U03] Py：加载 .env 配置
来源：http://hz.guannengcc.top/gtdramijex.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.sysykeji.top/gtyhlfumra.html

[U04] Py：变量调试打印
来源：http://hz.sxryk.cn/gtjfjldgnh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.chenzaomai.com/gtrrauplvi.html

[U05] Py：列表去重且保序
来源：http://hz.xuanzx.com/gtdiifujxm.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gttzgbchya.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtonyuypem.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtgbpuuftb.html

[U07] Py：反转字典键值
来源：http://hz.hammf.cn/gtmpghwakd.html

{v: k for k, v in d.items()}
来源：http://hz.hysaishi.cn/gthwdoxovh.html

[U08] Py：展平二维列表
来源：http://hz.nanxinkj.top/gtfiehlsjp.html

[y for x in nested for y in x]
来源：http://hz.ppjwa.cn/gtpbgwtdzl.html

[U09] Py：字典取最大值的键
来源：http://hz.shanyushiyangtech.top/gtcsnfcplw.html

max(d, key=d.get)
来源：http://hz.sweek.top/gtnanwhyjk.html

[U10] Py：按值排序字典
来源：http://hz.jinqigfzy.top/gthycxtjdg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jqgfzy.top/gtyasjadfl.html

[U11] Py：生成器表达式
来源：http://hz.nwbrower.top/gthmsbzpua.html

(x * 2 for x in arr)
来源：http://hz.yj20258.top/gtjhkorrqf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhixingplan.top/gtsqlegmqo.html

Counter(arr).most_common(3)
来源：http://hz.guowangkeji.top/gtxuormgzr.html

[U13] Py：固定长度队列
来源：http://hz.ppjwa.cn/gtkkdochru.html

deque(maxlen=10)
来源：http://hz.yongpay.top/gtdrmkjiuk.html

[U14] Py：分组收集到列表
来源：http://hz.hammf.cn/gtyyftsfrv.html

defaultdict(list)
来源：http://hz.shanyushiyangkeji.top/gtpoiklxzx.html

[U15] Py：高精度计时
来源：http://hz.ywan-chungtsiang.top/gtnqvseqkr.html

t = time.perf_counter()
来源：http://hz.ybcxt.top/gtakctelwe.html

[U16] Py：命令行参数解析
来源：http://hz.316326.xyz/gtjpxysgpc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yanxiufei.cn/gtrvlmefci.html

[U17] Py：初始化日志
来源：http://hz.birdmap.top/gtdetywooa.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.daria6918.cn/gtpdxtgjrd.html

[U18] Py：预编译正则
来源：http://hz.aibaodan.cn/gtcfqzpfjw.html

pat = re.compile(r"\d+")
来源：http://hz.yuxming.cn/gttppnvzcy.html

[U19] Py：正则替换带回调
来源：http://hz.ywan-chungtsiang.top/gthsgbrgky.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtcvekrznz.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigufen.top/gtaftqxtzr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dashuyun.cn/gtcsyjfudc.html

[U21] Py：自定义上下文管理器
来源：http://hz.gzhubu.top/gtrckyjngf.html

@contextlib.contextmanager
来源：http://hz.shanyushiyangtech.top/gtxbxrwfsr.html

[U22] Py：矩阵转置
来源：http://hz.fzhhl.top/gtozbctpyx.html

list(zip(*m))
来源：http://hz.gzhubu.top/gtdavkstyo.html

[U23] Py：分块读取大文件
来源：http://hz.pengpengdd.cyou/gteekrypwv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.smart0.xyz/gttkquxhco.html

[U24] Py：路径操作
来源：http://hz.gzhubu.top/gtzkndknkf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.birdmap.top/gtprjhbfog.html

[U25] Py：CSV 按字典读
来源：http://hz.zhoulong.xyz/gtvvkvljsr.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtsgmpqlhj.html

[U26] Py：并发下载
来源：http://hz.ivvv.top/gtjdmkghdd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fzhhl.top/gtxvntgltb.html

[U27] Py：异步 HTTP
来源：http://hz.dashuyun.cn/gtikptcpnk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gtxrpedxtw.html

[U28] Py：类型别名
来源：http://hz.sysykeji.top/gtofrtoatc.html

UserId = int
来源：http://hz.xinyue.icu/gtgbzytxvv.html

[U29] Py：属性校验
来源：http://hz.jinyuanbaomall.cn/gtmqmxohsv.html

@property 与 @x.setter 配合
来源：http://hz.cucudq.cn/gtisgbcmea.html

[U30] Py：数据类
来源：http://hz.andypj.xyz/gtaymctyrx.html

@dataclass(slots=True)
来源：http://hz.yuanzhike.top/gtqnchwivr.html

[U31] Py：单测
来源：http://hz.havefunace.top/gtmphasqdn.html

python -m pytest -q
来源：http://hz.mhx1999.top/gtdlymwfjh.html

[U32] Py：代码格式化
来源：http://hz.cqqwz.cn/gtwepklhix.html

ruff format . && ruff check --fix .
来源：http://hz.yuanzhike.top/gtckrrxvxr.html

[U33] Py：打包发布
来源：http://hz.zhongyouzk.top/gtpdkdmbyo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fengsongda.top/gtpzfsbrzf.html

[U34] Py：判断编码
来源：http://hz.chenlongwang.top/gtmhmxrtqw.html

chardet.detect(raw)
来源：http://hz.jinyuanbaomall.cn/gtkstlcgtx.html

[U35] Py：发送邮件
来源：http://hz.shzxlz.cn/gtjzwjjhtd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gthevpayco.html

[U36] Py：定时任务
来源：http://hz.zhaomingkeji.xyz/gtyycmttry.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gthrmzgjoh.html

[U37] Py：读写 Excel
来源：http://hz.cashguo.top/gtfpefwvvp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hywenlv.cn/gtyodkjziw.html

[U38] Py：获取脚本所在目录
来源：http://hz.bjfxy.top/gtxkjhlsee.html

Path(__file__).resolve().parent
来源：http://hz.gotoacloud.top/gtxatyfasl.html

[U39] Py：判断是否在交互环境
来源：http://hz.cucudq.cn/gtrpqxtphp.html

sys.stdout.isatty()
来源：http://hz.316326.xyz/gtkhzqkppd.html

[U40] Py：打印到标准错误
来源：http://hz.xziqi.cn/gtfaycxfqg.html

print("err", file=sys.stderr)
来源：http://hz.daxiang520.top/gtlmksgalp.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yueranfly.top/gtwrlubuvi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ivvv.top/gtkwrromsd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinyuanbaomall.cn/gtjigbutpy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yvedp.cn/gtvognzgdm.html

[U43] PHP：声明命名空间
来源：http://hz.cqqwz.cn/gttifvlzzd.html

namespace App\Http;
来源：http://hz.wangdashe.top/gtnqjelmiz.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtmsjqgzla.html

declare(strict_types=1);
来源：http://hz.hongshengwenyu.top/gtxvhfbncq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.haohaochexian.top/gtxzrmgalk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtgpmdwybl.html

[U46] PHP：可空类型
来源：http://hz.daxiang520.top/gtfdmggjoc.html

?string $name = null
来源：http://hz.chenzaomai.com/gtgsoxspyn.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangkeji.top/gtghwfjldu.html

int|string $id
来源：http://hz.xziqi.cn/gtffrqswms.html

[U48] PHP：纯枚举
来源：http://hz.bjfxy.top/gtfrkiazvq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydjk.org.cn/gthenhypyt.html

[U49] PHP：只读属性
来源：http://hz.nanxinkj.top/gtkdgghbbp.html

public readonly string $name
来源：http://hz.nanxinkj.top/gtiabhweoh.html

[U50] PHP：构造器属性提升
来源：http://hz.xinyue.icu/gtedwfqymh.html

public function __construct(private int $id) {}
来源：http://hz.hfpthk.cn/gtgxcbbsjc.html

[U51] PHP：数组解构
来源：http://hz.ydzc1.top/gtlehzbamw.html

[$a, $b] = $arr;
来源：http://hz.chenjidiqi.icu/gtqxofemxj.html

[U52] PHP：箭头函数
来源：http://hz.52xcode.cn/gtabkmphur.html

$double = fn($x) => $x * 2;
来源：http://hz.aibaodan.cn/gtfrvmyurd.html

[U53] PHP：空合并运算符
来源：http://hz.hnqzz.top/gtptpnjnmr.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtllhmpxtd.html

[U54] PHP：空安全调用
来源：http://hz.yueranfly.top/gtqcnfrlpf.html

$obj?->method()
来源：http://hz.xinyue.icu/gtrqdeaqlz.html

[U55] PHP：match 表达式
来源：http://hz.yvedp.cn/gtscmfpacr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gaohongyu789.top/gtabfksebp.html

[U56] PHP：命名参数
来源：http://hz.ybcxt.top/gtygkvgimo.html

f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gttjzowznb.html

[U57] PHP：字符串插值
来源：http://hz.mhx1999.top/gtzdreloie.html

"值: {$a}"
来源：http://hz.yueranfly.top/gtswjvbunr.html

[U58] PHP：数组三件套
来源：http://hz.jqgufenzy.top/gtoqrfdwix.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhoulong.xyz/gteagdyvfh.html


<!-- 参考信息 -->