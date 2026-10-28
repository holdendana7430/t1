代发 wailian999

[S35] C++：map
来源：http://hz.zhengqikj.top/gteweiybkk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gtcpqiqlqg.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gtipvjsnhd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtabfzroiv.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtbdctudtv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ivvv.top/gttdawzfpq.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtrstlyqnq.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtoxlxlqfv.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtgxqlqope.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.quarkkingdee.top/gtdfzymiea.html

[S40] C++：查找元素
来源：http://hz.vqdsnc.cn/gtsskufygy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gzhubu.top/gtzyulcdxy.html

[S41] C++：类与构造函数
来源：http://hz.xingfuxueyuan.xyz/gtpyalogwj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xylfe.cn/gtwqkltqeu.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gtsngzgspj.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxinkj.top/gtdfzafjip.html

[S43] C++：智能指针
来源：http://hz.havefunace.top/gtwlhcmqqi.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtzsmazagi.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtdrostcbv.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gtwctklnlq.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtqzezxrws.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jyoumei.cn/gteebqqtiz.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtwkpqnkok.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xylfe.cn/gtmqrivtbn.html

[S47] C++：结构化绑定遍历
来源：http://hz.tian-w.cn/gtgikxdbom.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xylfe.cn/gtxzytixrz.html

[S48] C++：逐行读文件
来源：http://hz.yueranfly.top/gtjbyylyky.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtmiukzjjz.html

while (std::getline(in, line)) { }
来源：http://hz.yvedp.cn/gtddezzlzs.html

[S49] C++：写文件
来源：http://hz.hongshengwenyu.top/gtinojhrmc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtrfexzthe.html

[S50] C++：格式化数字
来源：http://hz.9152youxi.cn/gtqivjryvf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtcialenir.html

[S51] C++：显式类型转换
来源：http://hz.jinghuilouyu.cn/gttyglvbzq.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gtbrsszlcc.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtqjymgdci.html

int size() const noexcept { return n_; }
来源：http://hz.jqgufenzy.top/gtrkhervpw.html

[S53] C++：移动语义
来源：http://hz.ehwqpu.com/gtpebksety.html

std::vector<int> w = std::move(v);
来源：http://hz.chenlongwang.top/gthoavlbri.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtdxdpasbn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.iojbl.cn/gtdxzgucor.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtvtfjqwyd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jyoumei.cn/gtipwpktyk.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtrdablhub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtxcjxudei.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtuhnfcqah.html

constexpr int N = 10;
来源：http://hz.gogol.net.cn/gtvxtarjxg.html

[S58] C++：命名空间
来源：http://hz.sufxvd.cn/gtxvowernw.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtcbhdxpoq.html

[S59] C++：静态断言
来源：http://hz.snrcjt.cn/gtgkbiyvlo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shanyushiyangkeji.top/gtsuwufqdl.html

[S60] C++：遍历并删除元素
来源：http://hz.cdnleiting.top/gtbvdwqutv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guowangkeji.top/gtxsizzkpo.html

================================================================================
来源：http://hz.xuanzx.com/gtpxdpwatb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtfznslzrf.html

================================================================================
来源：http://hz.jinqigufen.top/gticjltwsb.html

[T01] Kotlin：Hello World
来源：http://hz.9152youxi.cn/gtvqiekyin.html

println("Hello")
来源：http://hz.cqqwz.cn/gtteamunyd.html

[T02] Kotlin：变量
来源：http://hz.birdmap.top/gtmraecupy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhijiandao.cn/gtbovlibru.html

[T03] Kotlin：字符串模板
来源：http://hz.hnqzz.top/gtoflyudgp.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtlhdivqjx.html

[T04] Kotlin：空安全
来源：http://hz.ydzc1.top/gtokoumgiq.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtrpdhpkid.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtetyvmpml.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hysaishi.cn/gtuzmxhfyu.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gtrxhyjogx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sweek.top/gtimazpneq.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gtaepmwkqf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.svipenyu.cn/gtalgggiyh.html

[T08] Kotlin：数据类
来源：http://hz.gzhubu.top/gtbivxzpdj.html

data class User(val name: String, val age: Int)
来源：http://hz.9152youxi.cn/gtenliedil.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtoqkuzrsr.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gttaauebyw.html

[T10] Kotlin：默认参数
来源：http://hz.nanxinkj.top/gthpwqeecv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtcnnqdecb.html

[T11] Kotlin：协程
来源：http://hz.hnxiangtu.top/gtxgyfofqp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hongshengwenyu.top/gthrlaztdq.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtgctrxzwi.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtflphmafk.html

[T13] Kotlin：只读 Map
来源：http://hz.guannengcc.top/gturlabugu.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtfscaekyc.html

[T14] Kotlin：循环
来源：http://hz.tanke756.top/gtwbtwlpsi.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtpimyhmfc.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtqnxumwhy.html

interface Shape { fun area(): Double }
来源：http://hz.zhongyouzk.top/gtpcdzfcvg.html

[T16] Swift：Hello World
来源：http://hz.ydjk.org.cn/gtbgzcbutt.html

print("Hello")
来源：http://hz.dashuyun.cn/gtpwkyjxun.html

[T17] Swift：变量与常量
来源：http://hz.xziqi.cn/gtelgtnbfj.html

var a = 1;  let b = 2
来源：http://hz.jiagoushi.top/gtpmdhlkbp.html

[T18] Swift：字符串插值
来源：http://hz.gogol.net.cn/gtwhyewjzw.html

"值: \(b)"
来源：http://hz.gogol.net.cn/gttvfjdntd.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gtlxythxoi.html

if let n = opt { print(n) }
来源：http://hz.kuanghao11.cn/gtlfutupuz.html

[T20] Swift：数组操作
来源：http://hz.xuanzx.com/gtnfsgdkwr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtmbsxbzmx.html

[T21] Swift：遍历
来源：http://hz.9152youxi.cn/gthsyqiymr.html

for x in a { print(x) }
来源：http://hz.ivvv.top/gtsvrwgvos.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtdyuhcdxc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtumomvxxn.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gtcaxcpqas.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtdqvjywfe.html

[T24] Swift：闭包
来源：http://hz.aizwys.cn/gtcknxkblb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtvxjjxetg.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtdnlpptcj.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtvukunnuy.html

[T26] Swift：类与重写
来源：http://hz.c1oappe.top/gtkpqzkpkz.html

class A: Base { override func f() {} }
来源：http://hz.316326.xyz/gtcpjjfezg.html

[T27] Swift：错误处理
来源：http://hz.hywenlv.cn/gthpjopgij.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gtgopnlsme.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtvxgrnslq.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtijggkorv.html

[T29] Swift：guard 提前返回
来源：http://hz.yonumen.top/gtmyunfcvl.html

guard let x = opt else { return }
来源：http://hz.redwolf501.top/gtdwjyjqsj.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtltfxogra.html

protocol Shape { func area() -> Double }
来源：http://hz.xziqi.cn/gtgjyluhwa.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gtzfwkfbqi.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtechoivqf.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtiqxszhhc.html

local a = 1
来源：http://hz.tianlin.xyz/gtgvcbiqxs.html

[T33] Lua：表（数组）
来源：http://hz.svipenyu.cn/gtwzusaxzt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gthaoikqsp.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtmhwnwhnn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dashuyun.cn/gtlmzzujbu.html

[T35] Lua：字典表
来源：http://hz.yj20258.top/gtxtqcofwf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtfrybawjb.html

[T36] Lua：函数
来源：http://hz.nanxuanxn.top/gtfyghhwje.html

function add(a, b) return a + b end
来源：http://hz.feifeiyinyue.top/gtmyivxzgp.html

[T37] Lua：字符串拼接
来源：http://hz.0kj1m.cn/gtnqnkqdou.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gtkphbdjbi.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gtivtsweml.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gtgmzozbyy.html

[T39] Lua：模式匹配
来源：http://hz.ywan-chungtsiang.top/gtokaywfhc.html

string.find(s, "%d+")
来源：http://hz.pengpengdd.cyou/gtrkjdqhou.html

[T40] Lua：元表
来源：http://hz.bjfxy.top/gtmzskfqed.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gttuifbjnc.html

[T41] Perl：Hello World
来源：http://hz.yanxiufei.cn/gttyqwdrgv.html

print "Hello\n";
来源：http://hz.shangyingyoupin.top/gtcmabswqm.html

[T42] Perl：变量类型
来源：http://hz.daria6918.cn/gtumzmoxkr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.tian-w.cn/gtmnjejbjn.html

[T43] Perl：字符串插值
来源：http://hz.guannengcc.top/gthletceix.html

"值: $a"
来源：http://hz.gaohongyu789.top/gtgarpbbog.html

[T44] Perl：条件
来源：http://hz.0kj1m.cn/gtjawsdnuu.html

if ($a > 0) { print "正"; }
来源：http://hz.zhaomingkeji.xyz/gtlnngovyo.html

[T45] Perl：数组遍历
来源：http://hz.zdqjudy.top/gtfhqkiaat.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangtech.top/gtwxovvmkt.html

[T46] Perl：哈希操作
来源：http://hz.smart0.xyz/gtxsdlayjf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtppoobbvp.html

[T47] Perl：正则捕获
来源：http://hz.jqgufenzy.top/gtvdpfxktq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuanzhike.top/gtriefcgre.html

[T48] Perl：正则替换
来源：http://hz.nwbrower.top/gtiyrctoav.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtyysqbmfi.html

[T49] Perl：函数
来源：http://hz.ivvv.top/gtehejznyu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yuxming.cn/gtkncyfaai.html

[T50] Perl：逐行读文件
来源：http://hz.zhijiandao.cn/gthdltrubl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.havefunace.top/gtvyphteps.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.0kj1m.cn/gtfcoonauy.html

[T51] Scala：Hello World
来源：http://hz.daria6918.cn/gtixtfjlgk.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtomxnzhrd.html

[T52] Scala：变量
来源：http://hz.shanyushiyangkeji.top/gtzcoyqzwx.html

val a = 1;  var b = 2
来源：http://hz.aizwys.cn/gtvvfvfleh.html

[T53] Scala：字符串插值
来源：http://hz.xuanzx.com/gtuxorsbvd.html

s"值: $b"
来源：http://hz.yueranfly.top/gtbpnsutjd.html

[T54] Scala：集合映射
来源：http://hz.yvedp.cn/gtytxsmdpt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cheryme.top/gtckatgrwb.html

[T55] Scala：集合过滤
来源：http://hz.hfpthk.cn/gtjzdxfdbh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tanke756.top/gtwwjozwoe.html

[T56] Scala：样例类
来源：http://hz.yanxiufei.cn/gtthhzsuxd.html

case class User(name: String, age: Int)
来源：http://hz.wangshuangyany.cn/gtkxsevozl.html

[T57] Scala：模式匹配
来源：http://hz.tanke756.top/gtmychwvcl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gtvmtsvcdm.html

[T58] Scala：函数定义
来源：http://hz.gotoacloud.top/gtetqzatmh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangkeji.top/gtpqzglncc.html

[T59] Scala：循环
来源：http://hz.yvedp.cn/gteeuxgeob.html

for (i <- 1 to 10) println(i)
来源：http://hz.mhx1999.top/gtgayjiiyp.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtjlkrqets.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cashguo.top/gtxqrdhann.html

================================================================================
来源：http://hz.jqgfzy.top/gtspoboces.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.cheryme.top/gttxckypxe.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxnfhikca.html

[U01] Py：创建虚拟环境
来源：http://hz.ydjk.org.cn/gtyaydnvkj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.52xcode.cn/gtpbjhmxtw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shzxlz.cn/gtqfmiinxv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtnkjszema.html

[U03] Py：加载 .env 配置
来源：http://hz.daxiang520.top/gteodqcqaq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtixrjqkok.html

[U04] Py：变量调试打印
来源：http://hz.zhixingplan.top/gtwetvikob.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pycfn.com/gtvtshvypq.html

[U05] Py：列表去重且保序
来源：http://hz.gaohongyu789.top/gtzvoreagr.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtsjbhquwg.html

[U06] Py：合并两个字典
来源：http://hz.smart0.xyz/gtylmnpiak.html

{**a, **b}
来源：http://hz.gogol.net.cn/gthyrmzesf.html

[U07] Py：反转字典键值
来源：http://hz.wangshuangyany.cn/gtkadwdbei.html

{v: k for k, v in d.items()}
来源：http://hz.zhengqikj.top/gtunwlhfat.html

[U08] Py：展平二维列表
来源：http://hz.cashguo.top/gttbzrbjwz.html

[y for x in nested for y in x]
来源：http://hz.xuetiantiany.cn/gthzubnuqi.html

[U09] Py：字典取最大值的键
来源：http://hz.daxiang520.top/gtzwtqxqwu.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtciszyexb.html

[U10] Py：按值排序字典
来源：http://hz.yonumen.top/gtoyafddul.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.pengpengdd.cyou/gtorcgmjmm.html

[U11] Py：生成器表达式
来源：http://hz.haohaochexian.top/gtdjciaepq.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtrnwkrxwh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigufen.top/gtueadshti.html

Counter(arr).most_common(3)
来源：http://hz.tanke756.top/gtbvrtsjoq.html

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gteooqwxsc.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtnymwpdpk.html

[U14] Py：分组收集到列表
来源：http://hz.guannengcc.top/gtvpxldbxr.html

defaultdict(list)
来源：http://hz.quarkkingdee.top/gtfyyrjkpd.html

[U15] Py：高精度计时
来源：http://hz.kuanghao11.cn/gtjpwuvxxb.html

t = time.perf_counter()
来源：http://hz.fzhhl.top/gtboefwqtv.html

[U16] Py：命令行参数解析
来源：http://hz.birdmap.top/gtykvbbxvn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.meibo888.top/gtzmmteqjg.html

[U17] Py：初始化日志
来源：http://hz.yj20258888.top/gtkkhucgrn.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gttewpflsy.html

[U18] Py：预编译正则
来源：http://hz.nanxinkj.top/gtlzcuplwt.html

pat = re.compile(r"\d+")
来源：http://hz.kuanghao11.cn/gttgjpplcq.html

[U19] Py：正则替换带回调
来源：http://hz.sufxvd.cn/gtugahbaln.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jyoumei.cn/gtspglcwvk.html

[U20] Py：缓存函数结果
来源：http://hz.zhengqikj.top/gtqnojmhuu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxuanxn.top/gtrgivuygd.html

[U21] Py：自定义上下文管理器
来源：http://hz.gotoacloud.top/gtjpgrsgfo.html

@contextlib.contextmanager
来源：http://hz.zhijiandao.cn/gtpsnitsel.html

[U22] Py：矩阵转置
来源：http://hz.chenlongwang.top/gtbjrrolzm.html

list(zip(*m))
来源：http://hz.chenlongwang.top/gtkhxdlzfo.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtaxxhvpoq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.52xcode.cn/gtefueyvau.html

[U24] Py：路径操作
来源：http://hz.bjfxy.top/gtvllmqrsp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.9152youxi.cn/gttfunvreh.html

[U25] Py：CSV 按字典读
来源：http://hz.redwolf501.top/gtslwudbcf.html

csv.DictReader(f)
来源：http://hz.dianchejie.cn/gtveljacfv.html

[U26] Py：并发下载
来源：http://hz.nwbrower.top/gtfwecjurm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtxqagjmbd.html

[U27] Py：异步 HTTP
来源：http://hz.zhoulong.xyz/gtviskglom.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xuetiantiany.cn/gtfstbwsso.html

[U28] Py：类型别名
来源：http://hz.meibo888.top/gttmoqnwit.html

UserId = int
来源：http://hz.daxiang520.top/gtgilkfltg.html

[U29] Py：属性校验
来源：http://hz.guowangkeji.top/gtgivdugqq.html

@property 与 @x.setter 配合
来源：http://hz.yongpay.top/gtqpwwdsog.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtqaarjtoe.html

@dataclass(slots=True)
来源：http://hz.guowangkeji.top/gtdeqbeurm.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtudenaioz.html

python -m pytest -q
来源：http://hz.nanxuanxn.top/gtswbppwuk.html

[U32] Py：代码格式化
来源：http://hz.quarkkingdee.top/gtleuzvvzf.html

ruff format . && ruff check --fix .
来源：http://hz.shanyushiyangtech.top/gtahntgaet.html

[U33] Py：打包发布
来源：http://hz.zhongyouzk.top/gtugmtwomt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.aibaodan.cn/gtwmefelmx.html

[U34] Py：判断编码
来源：http://hz.xuetiantiany.cn/gtwksmgtcy.html

chardet.detect(raw)
来源：http://hz.wangshuangyany.cn/gtvnorhtkn.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangkeji.top/gtncsgjfps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cdnleiting.top/gtbcwliied.html

[U36] Py：定时任务
来源：http://hz.cdnleiting.top/gtphuunbpe.html

schedule.every(10).minutes.do(job)
来源：http://hz.zdqjudy.top/gtfupqosdz.html

[U37] Py：读写 Excel
来源：http://hz.jiagoushi.top/gtsvkwsrsb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xuanzx.com/gtjyuqtkwy.html

[U38] Py：获取脚本所在目录
来源：http://hz.nwbrower.top/gtappdcaxj.html

Path(__file__).resolve().parent
来源：http://hz.chenzaomai.com/gtrrxwmdve.html

[U39] Py：判断是否在交互环境
来源：http://hz.gzhubu.top/gtddvigbdw.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtruhizdvl.html

[U40] Py：打印到标准错误
来源：http://hz.nwbrower.top/gtxgczhplm.html

print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtkokocwcs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xylfe.cn/gtclqacnga.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ppjwa.cn/gtzckhdqxk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ydzc1.top/gtykvognbs.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gtmygbtwjc.html

[U43] PHP：声明命名空间
来源：http://hz.jinyuanbaomall.cn/gtbrmxgken.html

namespace App\Http;
来源：http://hz.ydjk.org.cn/gtflctsvnn.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtuwtbzelt.html

declare(strict_types=1);
来源：http://hz.yuanzhike.top/gtqkvzwjdb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.dianchejie.cn/gtbmiubefb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtkoigvjjv.html

[U46] PHP：可空类型
来源：http://hz.dianchejie.cn/gtmbmmswyn.html

?string $name = null
来源：http://hz.ydzc1.top/gtbyvcauzs.html

[U47] PHP：联合类型
来源：http://hz.dianchejie.cn/gtmtuwemvr.html

int|string $id
来源：http://hz.andypj.xyz/gtgkawvyku.html

[U48] PHP：纯枚举
来源：http://hz.dashuyun.cn/gthmogpmya.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yonumen.top/gtynxsozkt.html

[U49] PHP：只读属性
来源：http://hz.cqqwz.cn/gtscsqdrun.html

public readonly string $name
来源：http://hz.jqgufenzy.top/gthesomyjz.html

[U50] PHP：构造器属性提升
来源：http://hz.jlsjyb.cn/gtxogztncg.html

public function __construct(private int $id) {}
来源：http://hz.zdqjudy.top/gtltmavrbg.html

[U51] PHP：数组解构
来源：http://hz.9152youxi.cn/gtgyuhvnnl.html

[$a, $b] = $arr;
来源：http://hz.cucudq.cn/gtfunqzjut.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtlewevmxz.html

$double = fn($x) => $x * 2;
来源：http://hz.c1oappe.top/gtagaociud.html

[U53] PHP：空合并运算符
来源：http://hz.svipenyu.cn/gtwfbytbyz.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj20258888.top/gtelpxkdcw.html

[U54] PHP：空安全调用
来源：http://hz.52xcode.cn/gtfcplbmlu.html

$obj?->method()
来源：http://hz.shangyingyoupin.top/gtsdqznkce.html

[U55] PHP：match 表达式
来源：http://hz.xylfe.cn/gtyozifepm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tanke756.top/gttcsmujho.html

[U56] PHP：命名参数
来源：http://hz.gogol.net.cn/gtjlfdvcjf.html

f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtuugpoqpk.html

[U57] PHP：字符串插值
来源：http://hz.haohaochexian.top/gthyxwpfhw.html

"值: {$a}"
来源：http://hz.9152youxi.cn/gtoiqkfynv.html

[U58] PHP：数组三件套
来源：http://hz.ybcxt.top/gtgccbrkmt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cdnleiting.top/gthwpsabua.html

[U59] PHP：自定义排序
来源：http://hz.shzxlz.cn/gtrkyqghbt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtliilhkyo.html

[U60] PHP：JSON 编解码
来源：http://hz.redwolf501.top/gtenrrkwtq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gogol.net.cn/gthxersmrr.html


<!-- 参考信息 -->