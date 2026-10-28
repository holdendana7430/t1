代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtbrkintou.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtqzxviqqt.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtbgffrido.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtqufjjgqk.html

[S41] C++：类与构造函数
来源：http://hz.c1oappe.top/gtoiqswpwj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daria6918.cn/gtjapjqaei.html

[S42] C++：继承与虚函数
来源：http://hz.jinghuilouyu.cn/gtbaxqltin.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhongyouzk.top/gtrsbmlnxx.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtzuihhpqe.html

auto p = std::make_unique<int>(5);
来源：http://hz.ybcxt.top/gtuhvoddve.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtvxaynqzc.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtgxbzhxeg.html

[S45] C++：lambda
来源：http://hz.havefunace.top/gtogopljae.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gttffakbcs.html

[S46] C++：函数模板
来源：http://hz.sweek.top/gtoynvhtlc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.guowangkeji.top/gtcwepwobo.html

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtkqpekttw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtoidjwlys.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gthlcyckwl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gtojcswncc.html

while (std::getline(in, line)) { }
来源：http://hz.xylfe.cn/gtdqrmvtcl.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gteenvalrm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtfcepgqkk.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtfsfzdggr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shanyushiyangtech.top/gtomexhahn.html

[S51] C++：显式类型转换
来源：http://hz.meibo888.top/gtlkaxrast.html

static_cast<double>(a) / b
来源：http://hz.sweek.top/gthsdwuwnd.html

[S52] C++：const 与 noexcept
来源：http://hz.sxryk.cn/gtknmdvrqf.html

int size() const noexcept { return n_; }
来源：http://hz.zhongyouzk.top/gtyynbalsx.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtjtfbjacy.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtgggovokj.html

[S54] C++：异常处理
来源：http://hz.yuxming.cn/gtwdhtoptd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtldhinive.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gtkvcheddl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtuskfhvao.html

[S56] C++：optional
来源：http://hz.yj202588.top/gtyirkazwe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sweek.top/gtzxpfxkhn.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gteksxhrao.html

constexpr int N = 10;
来源：http://hz.52xcode.cn/gtndqhwwli.html

[S58] C++：命名空间
来源：http://hz.jqgfzy.top/gtopneirmc.html

namespace ns { int f() { return 1; } }
来源：http://hz.fengsongda.top/gtpxebisst.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtqizztcae.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtoodtexrd.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtmytwobar.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gzhubu.top/gtsaiwxpik.html

================================================================================
来源：http://hz.hnxiangtu.top/gtruahhsgi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtsdrmsglv.html

================================================================================
来源：http://hz.yuxming.cn/gtpbgidnye.html

[T01] Kotlin：Hello World
来源：http://hz.yvedp.cn/gtvzzljwoi.html

println("Hello")
来源：http://hz.shzxlz.cn/gtgdodqxaz.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gtgqsnjyfi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinghuilouyu.cn/gtfjatanhj.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtonrgkxga.html

"值: $b"
来源：http://hz.meibo888.top/gtcsrvqvyc.html

[T04] Kotlin：空安全
来源：http://hz.xziqi.cn/gtvzypxkub.html

val n: String? = null;  n?.length
来源：http://hz.kuanghao11.cn/gtbtdwcsnt.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtpmdnsnod.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.andypj.xyz/gtvrgndmuw.html

[T06] Kotlin：集合映射
来源：http://hz.sufxvd.cn/gtxawbpqfl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nwbrower.top/gtjpderuxm.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangkeji.top/gttkjnmbta.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ehwqpu.com/gtgbczcwwq.html

[T08] Kotlin：数据类
来源：http://hz.xingfuxueyuan.xyz/gtpaspmjfj.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtlkpednnn.html

[T09] Kotlin：扩展函数
来源：http://hz.sufxvd.cn/gtwehnbinu.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtwugvrjmr.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gtlhegtfrb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuanzx.com/gthunrpgze.html

[T11] Kotlin：协程
来源：http://hz.yj20258888.top/gtizmgwolq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gthnmednnm.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtixqoyshr.html

val (a, b) = Pair(1, 2)
来源：http://hz.sweek.top/gtpylsmwxd.html

[T13] Kotlin：只读 Map
来源：http://hz.tanke756.top/gtxefhpfsn.html

val m = mapOf("a" to 1)
来源：http://hz.wangdashe.top/gtpqcuhtor.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtbeqnszoj.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtaclvngmh.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtlnscyyzn.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtvokhbafc.html

[T16] Swift：Hello World
来源：http://hz.zhongyouzk.top/gthjzybmvp.html

print("Hello")
来源：http://hz.meibo888.top/gtucxolung.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtbtkvodsu.html

var a = 1;  let b = 2
来源：http://hz.zdqjudy.top/gtfaafejxu.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtotmtuvew.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtyunbkuhe.html

[T19] Swift：可选绑定
来源：http://hz.hysaishi.cn/gttadatlzx.html

if let n = opt { print(n) }
来源：http://hz.yonumen.top/gtvhstlmzn.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtrkyfvrve.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dianchejie.cn/gtcbnfecpx.html

[T21] Swift：遍历
来源：http://hz.yvedp.cn/gtaxcrsbqj.html

for x in a { print(x) }
来源：http://hz.jinghuilouyu.cn/gtqnvlyqsj.html

[T22] Swift：字典
来源：http://hz.xinyue.icu/gtrieoelll.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenjidiqi.icu/gtzteioonp.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gthvbaetxu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shuidangran.top/gtnircfciu.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtusmgfpql.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tianlin.xyz/gtaswxhbga.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtukboozav.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtrdptykfc.html

[T26] Swift：类与重写
来源：http://hz.tianlin.xyz/gtsshryfct.html

class A: Base { override func f() {} }
来源：http://hz.cqqwz.cn/gtpsrcxkej.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gtexxfivtk.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gthkmptkbi.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gtvzysiuaf.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gterhjeoeo.html

[T29] Swift：guard 提前返回
来源：http://hz.fzhhl.top/gtwsjbygvo.html

guard let x = opt else { return }
来源：http://hz.kuanghao11.cn/gtkjjjaviz.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtohycdofr.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtoprlcuyb.html

[T31] Lua：Hello World
来源：http://hz.jianghu66.top/gtlwgfemno.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtskosxmsq.html

[T32] Lua：局部变量
来源：http://hz.daria6918.cn/gtixmyfhnq.html

local a = 1
来源：http://hz.tianlin.xyz/gtkcudftqt.html

[T33] Lua：表（数组）
来源：http://hz.meibo888.top/gtifpbkvnm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hnxiangtu.top/gtngvepkvf.html

[T34] Lua：遍历表
来源：http://hz.yj20258.top/gthbeomsrr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnxiangtu.top/gtjxydkcfy.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gthjlcbhia.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ybcxt.top/gtlusgviwq.html

[T36] Lua：函数
来源：http://hz.guowangkeji.top/gtwdqcasjr.html

function add(a, b) return a + b end
来源：http://hz.sweek.top/gtdqhipdng.html

[T37] Lua：字符串拼接
来源：http://hz.zhongyouzk.top/gtbdqvhmsy.html

"a" .. "b"
来源：http://hz.cdnleiting.top/gtmralthgj.html

[T38] Lua：条件
来源：http://hz.gzhubu.top/gtulfsgoad.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtmitbxzud.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtuwbfjinu.html

string.find(s, "%d+")
来源：http://hz.zdqjudy.top/gtwkwxfvlx.html

[T40] Lua：元表
来源：http://hz.quarkkingdee.top/gtqbouppjm.html

setmetatable({}, { __index = base })
来源：http://hz.shuidangran.top/gttmwqzbey.html

[T41] Perl：Hello World
来源：http://hz.zhengqikj.top/gtdahlgapc.html

print "Hello\n";
来源：http://hz.nanxinkj.top/gttgrbvscu.html

[T42] Perl：变量类型
来源：http://hz.fzhhl.top/gtxtyajiko.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinyuanbaomall.cn/gtiemxbkoq.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtynxezvzh.html

"值: $a"
来源：http://hz.zhixingplan.top/gtsxqgecqo.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gttcloggtt.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gtcjxjdghg.html

[T45] Perl：数组遍历
来源：http://hz.yj20258888.top/gtxxttfamj.html

for my $x (@arr) { print $x; }
来源：http://hz.yuanzhike.top/gtdxyeylyv.html

[T46] Perl：哈希操作
来源：http://hz.jyoumei.cn/gtuvryjowm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yvedp.cn/gtqbukknqk.html

[T47] Perl：正则捕获
来源：http://hz.kuanghao11.cn/gtahdpaqul.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ehwqpu.com/gtptqnfkug.html

[T48] Perl：正则替换
来源：http://hz.yvedp.cn/gtqsyxxreo.html

$s =~ s/old/new/g;
来源：http://hz.xziqi.cn/gtadrmxwfl.html

[T49] Perl：函数
来源：http://hz.wangdashe.top/gtdtjhgppr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xziqi.cn/gtvvhtppux.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtpjwronpm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtvgzhpwnm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gthmfnkknm.html

[T51] Scala：Hello World
来源：http://hz.xylfe.cn/gtjfvxettt.html

println("Hello")
来源：http://hz.jinqigufen.top/gtlgcvjxjq.html

[T52] Scala：变量
来源：http://hz.ybcxt.top/gtvuptemtr.html

val a = 1;  var b = 2
来源：http://hz.wangdashe.top/gtdcbpwkau.html

[T53] Scala：字符串插值
来源：http://hz.dashuyun.cn/gturqeavsz.html

s"值: $b"
来源：http://hz.fengsongda.top/gtfwdobwdt.html

[T54] Scala：集合映射
来源：http://hz.hysaishi.cn/gtbncdfoij.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gzhubu.top/gttavxkhtl.html

[T55] Scala：集合过滤
来源：http://hz.316326.xyz/gtxvuuokyz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gotoacloud.top/gtnfhraiwi.html

[T56] Scala：样例类
来源：http://hz.mhx1999.top/gtyqtbmwdw.html

case class User(name: String, age: Int)
来源：http://hz.daxiang520.top/gtaeuhojrk.html

[T57] Scala：模式匹配
来源：http://hz.zhiwuduotai.top/gtxpvdryux.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhixingplan.top/gtzdmiigao.html

[T58] Scala：函数定义
来源：http://hz.tian-w.cn/gtuoxvbnkc.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aibaodan.cn/gtzgcswsrv.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtilmcqzzb.html

for (i <- 1 to 10) println(i)
来源：http://hz.gogol.net.cn/gtrqrrpwxh.html

[T60] Scala：折叠
来源：http://hz.hammf.cn/gtpyhsrutt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shuidangran.top/gttzefdgtm.html

================================================================================
来源：http://hz.yvedp.cn/gtcgxkqpsz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtgsyskegq.html

================================================================================
来源：http://hz.hnqzz.top/gtpbykhyik.html

[U01] Py：创建虚拟环境
来源：http://hz.ybcxt.top/gtisqcsnsx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nwbrower.top/gtnvlrvzgg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtpdtfdqja.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dianchejie.cn/gtoxqbagnu.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtbbrumswt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gtkoblqkxh.html

[U04] Py：变量调试打印
来源：http://hz.svipenyu.cn/gtjbvlbqne.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.bjfxy.top/gtxmjzsfug.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtkwuxhski.html

list(dict.fromkeys(arr))
来源：http://hz.sweek.top/gtnwivyvdi.html

[U06] Py：合并两个字典
来源：http://hz.yj20258888.top/gtppdrnymq.html

{**a, **b}
来源：http://hz.jiagoushi.top/gtmjvhrkrj.html

[U07] Py：反转字典键值
来源：http://hz.jlsjyb.cn/gtzqblcstl.html

{v: k for k, v in d.items()}
来源：http://hz.gogol.net.cn/gtoiqwogfa.html

[U08] Py：展平二维列表
来源：http://hz.cucudq.cn/gtqsvlepqt.html

[y for x in nested for y in x]
来源：http://hz.gzhubu.top/gtmfpkwckw.html

[U09] Py：字典取最大值的键
来源：http://hz.iojbl.cn/gtqygznpol.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtvcyuggaf.html

[U10] Py：按值排序字典
来源：http://hz.iojbl.cn/gtvbdiaxbv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sysykeji.top/gtcqlxutgi.html

[U11] Py：生成器表达式
来源：http://hz.ydzc1.top/gtiqrcvyiu.html

(x * 2 for x in arr)
来源：http://hz.bjfxy.top/gtorjfmmtz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.0kj1m.cn/gtgujgnozu.html

Counter(arr).most_common(3)
来源：http://hz.kuanghao11.cn/gtsjuowpoo.html

[U13] Py：固定长度队列
来源：http://hz.kuanghao11.cn/gtchnjvweh.html

deque(maxlen=10)
来源：http://hz.bjfxy.top/gtlutgnafx.html

[U14] Py：分组收集到列表
来源：http://hz.tanke756.top/gtrjxdufvv.html

defaultdict(list)
来源：http://hz.jyoumei.cn/gtlnvevfre.html

[U15] Py：高精度计时
来源：http://hz.havefunace.top/gtmilapwpn.html

t = time.perf_counter()
来源：http://hz.tanke756.top/gtyzvkgtkr.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtyqrhlduk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.shangyingyoupin.top/gtyuvmycbv.html

[U17] Py：初始化日志
来源：http://hz.nanxuanxn.top/gtxkrqwbgp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tianlin.xyz/gtflvorteq.html

[U18] Py：预编译正则
来源：http://hz.nwbrower.top/gtfanrocgc.html

pat = re.compile(r"\d+")
来源：http://hz.ydzc1.top/gtbuzzrqwb.html

[U19] Py：正则替换带回调
来源：http://hz.cucudq.cn/gtqlnobmxy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hysaishi.cn/gtjsrmhope.html

[U20] Py：缓存函数结果
来源：http://hz.kuanghao11.cn/gtkserrpkz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhoulong.xyz/gtvjjwjqcs.html

[U21] Py：自定义上下文管理器
来源：http://hz.nanxinkj.top/gtgoaxlsfr.html

@contextlib.contextmanager
来源：http://hz.zhoulong.xyz/gtjdpxjuol.html

[U22] Py：矩阵转置
来源：http://hz.nanxinkj.top/gtcewgchof.html

list(zip(*m))
来源：http://hz.shanyushiyangtech.top/gtsmuskkza.html

[U23] Py：分块读取大文件
来源：http://hz.guannengcc.top/gtmhxzwbfs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xuetiantiany.cn/gttsxhlvkz.html

[U24] Py：路径操作
来源：http://hz.xinyue.icu/gthlpmjijt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.snrcjt.cn/gtztkpliru.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtyqbpydfw.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtsvnkozlv.html

[U26] Py：并发下载
来源：http://hz.zhijiandao.cn/gtjatduzou.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.feifeiyinyue.top/gtrhijdojp.html

[U27] Py：异步 HTTP
来源：http://hz.ppjwa.cn/gtsqimtomd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.mhx1999.top/gtdfscywjv.html

[U28] Py：类型别名
来源：http://hz.shuidangran.top/gttpbiqjbw.html

UserId = int
来源：http://hz.9152youxi.cn/gtsokahadn.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gthldbnfrl.html

@property 与 @x.setter 配合
来源：http://hz.yj20258.top/gtpoxecgep.html

[U30] Py：数据类
来源：http://hz.xylfe.cn/gtubmtowog.html

@dataclass(slots=True)
来源：http://hz.tianlin.xyz/gtkizlfcrm.html

[U31] Py：单测
来源：http://hz.jyoumei.cn/gtmiubwnmc.html

python -m pytest -q
来源：http://hz.ydjk.org.cn/gtauydvhfg.html

[U32] Py：代码格式化
来源：http://hz.zhengqikj.top/gteawgxihm.html

ruff format . && ruff check --fix .
来源：http://hz.nanxinkj.top/gtgztdfjka.html

[U33] Py：打包发布
来源：http://hz.jinghuilouyu.cn/gtvfcprsls.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cucudq.cn/gtxbudljsv.html

[U34] Py：判断编码
来源：http://hz.jinqigfzy.top/gtuedialgt.html

chardet.detect(raw)
来源：http://hz.xuanzx.com/gtwvhnbpqz.html

[U35] Py：发送邮件
来源：http://hz.bjfxy.top/gttufhoykr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.redwolf501.top/gtokpdeylu.html

[U36] Py：定时任务
来源：http://hz.ydzc1.top/gtrwozfgjx.html

schedule.every(10).minutes.do(job)
来源：http://hz.c1oappe.top/gtqvpbaykx.html

[U37] Py：读写 Excel
来源：http://hz.ywan-chungtsiang.top/gtzrfcecow.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.dianchejie.cn/gtkldqruft.html

[U38] Py：获取脚本所在目录
来源：http://hz.quarkkingdee.top/gtssngcnbp.html

Path(__file__).resolve().parent
来源：http://hz.shangyingyoupin.top/gtnaaiqljy.html

[U39] Py：判断是否在交互环境
来源：http://hz.sufxvd.cn/gthtwjiges.html

sys.stdout.isatty()
来源：http://hz.dianchejie.cn/gttpagpwfz.html

[U40] Py：打印到标准错误
来源：http://hz.zycfv.cn/gtmzwynepn.html

print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtligazgxu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sufxvd.cn/gtudtgabuo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.smart0.xyz/gtlrhvobrf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aizwys.cn/gttvxtvygn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.chenjidiqi.icu/gtqjdkiuuq.html

[U43] PHP：声明命名空间
来源：http://hz.xuetiantiany.cn/gtvlanriwq.html

namespace App\Http;
来源：http://hz.hnqzz.top/gtxwxugses.html

[U44] PHP：开启严格类型
来源：http://hz.tianlin.xyz/gtdiygmceo.html

declare(strict_types=1);
来源：http://hz.xuetiantiany.cn/gtkbzfbtki.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hammf.cn/gtciaoqwht.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gttdwzvrho.html

[U46] PHP：可空类型
来源：http://hz.yuxming.cn/gtmimrpbxe.html

?string $name = null
来源：http://hz.daxiang520.top/gtnvpgjbmg.html

[U47] PHP：联合类型
来源：http://hz.yueranfly.top/gttrjfyhwh.html

int|string $id
来源：http://hz.tanke756.top/gtfqhwdrjz.html

[U48] PHP：纯枚举
来源：http://hz.jyoumei.cn/gtuaegjpsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hysaishi.cn/gtflmvwuvm.html

[U49] PHP：只读属性
来源：http://hz.iojbl.cn/gtgsxxedmk.html

public readonly string $name
来源：http://hz.zhiwuduotai.top/gtlhbaazaf.html

[U50] PHP：构造器属性提升
来源：http://hz.bjfxy.top/gtyrqoawof.html

public function __construct(private int $id) {}
来源：http://hz.ydjk.org.cn/gtvqsszvvm.html

[U51] PHP：数组解构
来源：http://hz.hongshengwenyu.top/gtqotntafi.html

[$a, $b] = $arr;
来源：http://hz.dianchejie.cn/gtgrorzqbl.html

[U52] PHP：箭头函数
来源：http://hz.zycfv.cn/gtofhpgyzi.html

$double = fn($x) => $x * 2;
来源：http://hz.svipenyu.cn/gtilrrmqbw.html

[U53] PHP：空合并运算符
来源：http://hz.smart0.xyz/gthxaszygv.html

$v = $a ?? $b ?? "default";
来源：http://hz.redwolf501.top/gtdsqkpnsx.html

[U54] PHP：空安全调用
来源：http://hz.zycfv.cn/gteqvajlwr.html

$obj?->method()
来源：http://hz.jinqigufen.top/gtzyscsoks.html

[U55] PHP：match 表达式
来源：http://hz.sufxvd.cn/gtyjcpfchg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.daxiang520.top/gtyfpbpelc.html

[U56] PHP：命名参数
来源：http://hz.yj20258.top/gtztmfnwuk.html

f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtrblqlued.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gtssffpkwu.html

"值: {$a}"
来源：http://hz.ywan-chungtsiang.top/gtimftwnvp.html

[U58] PHP：数组三件套
来源：http://hz.wangdashe.top/gtwfqfjajd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xuanzx.com/gtxbasrywq.html

[U59] PHP：自定义排序
来源：http://hz.zhiwuduotai.top/gtyptfydwz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtolbtfyhd.html

[U60] PHP：JSON 编解码
来源：http://hz.hywenlv.cn/gtqwhfwrtz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gtivrokiyx.html

[U61] PHP：正则
来源：http://hz.shangyingyoupin.top/gtggpncggc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.shzxlz.cn/gtekeixhsy.html

[U62] PHP：日期对象
来源：http://hz.nwbrower.top/gtzjzwzpbj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hywenlv.cn/gtkdidjulk.html

[U63] PHP：文件读写
来源：http://hz.dianchejie.cn/gtdusiorhi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.nanxinkj.top/gthmxqnhxj.html

[U64] PHP：目录遍历
来源：http://hz.zhaomingkeji.xyz/gtjlgjqvab.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nwbrower.top/gtkxlltjke.html


<!-- 参考信息 -->