代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gtunjifadc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hfpthk.cn/gtzuqpqolq.html

[S40] C++：查找元素
来源：http://hz.hongshengwenyu.top/gtsymiidry.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sysykeji.top/gtrxvgggvp.html

[S41] C++：类与构造函数
来源：http://hz.cheryme.top/gtypjnfjdt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gtqplxlcjr.html

[S42] C++：继承与虚函数
来源：http://hz.0kj1m.cn/gtboguqebj.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtbqrwqkpm.html

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtynoyqwct.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gtsvgbespp.html

[S44] C++：引用传参
来源：http://hz.jyoumei.cn/gtpppkbcpy.html

void inc(int &x) { ++x; }
来源：http://hz.quarkkingdee.top/gtgabzpcbo.html

[S45] C++：lambda
来源：http://hz.jlsjyb.cn/gtjyyafvhs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenlongwang.top/gtvkockeer.html

[S46] C++：函数模板
来源：http://hz.9152youxi.cn/gthjpzvqja.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nwbrower.top/gtrrzdbfws.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gtdjidnbic.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gttmbesent.html

[S48] C++：逐行读文件
来源：http://hz.jiagoushi.top/gtptumjwnx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhijiandao.cn/gtzvfufohl.html

while (std::getline(in, line)) { }
来源：http://hz.feifeiyinyue.top/gtvbdqrvai.html

[S49] C++：写文件
来源：http://hz.ydzc1.top/gtlqdlgvvp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ivvv.top/gtmitufraf.html

[S50] C++：格式化数字
来源：http://hz.havefunace.top/gtbislowhi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cheryme.top/gtdphiaekq.html

[S51] C++：显式类型转换
来源：http://hz.shangyingyoupin.top/gtneumurjy.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtzgdgvpml.html

[S52] C++：const 与 noexcept
来源：http://hz.shuidangran.top/gttioibsnp.html

int size() const noexcept { return n_; }
来源：http://hz.jianghu66.top/gtftifyijx.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtykzluyde.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtcjtiuqge.html

[S54] C++：异常处理
来源：http://hz.316326.xyz/gtnyrbpszp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhongyouzk.top/gtdftpphha.html

[S55] C++：结构化绑定
来源：http://hz.jinghuilouyu.cn/gtyxjtifdp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtsqqubabs.html

[S56] C++：optional
来源：http://hz.mhx1999.top/gtwgogvknh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shanyushiyangkeji.top/gtqewjaqaj.html

[S57] C++：编译期常量
来源：http://hz.dianchejie.cn/gtxdohjuzm.html

constexpr int N = 10;
来源：http://hz.zhoulong.xyz/gtztjeoiri.html

[S58] C++：命名空间
来源：http://hz.zhoulong.xyz/gtgtgcogtk.html

namespace ns { int f() { return 1; } }
来源：http://hz.jiagoushi.top/gtkmwduqiv.html

[S59] C++：静态断言
来源：http://hz.jianghu66.top/gtgrdhdrbd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxinkj.top/gtzkrqscuy.html

[S60] C++：遍历并删除元素
来源：http://hz.c1oappe.top/gtcjbiyegi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtnmvtqqzk.html

================================================================================
来源：http://hz.quarkkingdee.top/gthzijfhbu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtmwwdwpgf.html

================================================================================
来源：http://hz.yongpay.top/gtqxyfdyln.html

[T01] Kotlin：Hello World
来源：http://hz.yj202588.top/gtjvxbqcrj.html

println("Hello")
来源：http://hz.ydzc1.top/gtobjuchpa.html

[T02] Kotlin：变量
来源：http://hz.zycfv.cn/gtrjwgozzh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.svipenyu.cn/gtgzjputjf.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gtzsxfboqb.html

"值: $b"
来源：http://hz.hysaishi.cn/gtrmnfgeqa.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtsxiahibh.html

val n: String? = null;  n?.length
来源：http://hz.xuanzx.com/gtwzdvgfow.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gtzaimqjxp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtvnluleqt.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtjfmrdzwm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhongyouzk.top/gtwbrsxxxy.html

[T07] Kotlin：集合过滤
来源：http://hz.snrcjt.cn/gttdyznzct.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtnpeuazyh.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtxomxidik.html

data class User(val name: String, val age: Int)
来源：http://hz.jlsjyb.cn/gtfsiqwqjg.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtdtxcyoun.html

fun String.exclaim() = this + "!"
来源：http://hz.cqqwz.cn/gtusumhluf.html

[T10] Kotlin：默认参数
来源：http://hz.yj202588.top/gtsbalpfsq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pengpengdd.cyou/gtoweoiuxn.html

[T11] Kotlin：协程
来源：http://hz.316326.xyz/gtjyldvnua.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gttqdxadgf.html

[T12] Kotlin：解构声明
来源：http://hz.cqqwz.cn/gtaezxskfx.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtxygpcpou.html

[T13] Kotlin：只读 Map
来源：http://hz.c1oappe.top/gtaxoshvcd.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigfzy.top/gtujlayonf.html

[T14] Kotlin：循环
来源：http://hz.guowangkeji.top/gtevmuyaci.html

for (i in 1..10) println(i)
来源：http://hz.nanxuanxn.top/gtwriqfxyu.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtyycvfdag.html

interface Shape { fun area(): Double }
来源：http://hz.jianghu66.top/gtfhjhancw.html

[T16] Swift：Hello World
来源：http://hz.hnqzz.top/gtdvyynovw.html

print("Hello")
来源：http://hz.ehwqpu.com/gtujjfshpt.html

[T17] Swift：变量与常量
来源：http://hz.tian-w.cn/gtsxyoxpel.html

var a = 1;  let b = 2
来源：http://hz.shuidangran.top/gtlhktaqlv.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gtlzgyfalb.html

"值: \(b)"
来源：http://hz.hammf.cn/gtztkmojjy.html

[T19] Swift：可选绑定
来源：http://hz.jianghu66.top/gtmnxtfbcd.html

if let n = opt { print(n) }
来源：http://hz.chenlongwang.top/gtrzcxdvlx.html

[T20] Swift：数组操作
来源：http://hz.ppjwa.cn/gtfqpeqvpi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtnjbuwqvp.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtmjdcxrwk.html

for x in a { print(x) }
来源：http://hz.cucudq.cn/gtnegrvruj.html

[T22] Swift：字典
来源：http://hz.yonumen.top/gthymfswpd.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fzhhl.top/gtuundcuou.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtiyzhstmb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ppjwa.cn/gtfangdork.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtdbludgar.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtttlghfrr.html

[T25] Swift：结构体
来源：http://hz.zhixingplan.top/gtvklkjdjy.html

struct P { var x: Int }
来源：http://hz.haohaochexian.top/gtypgxowsh.html

[T26] Swift：类与重写
来源：http://hz.mhx1999.top/gtvmwanhwc.html

class A: Base { override func f() {} }
来源：http://hz.yuxming.cn/gtuwslrvlm.html

[T27] Swift：错误处理
来源：http://hz.chenlongwang.top/gtxrdwkyqs.html

do { try f() } catch { print(error) }
来源：http://hz.hammf.cn/gtqqvphzdw.html

[T28] Swift：枚举
来源：http://hz.yj202588.top/gtsflvcfah.html

enum Color { case red, green }
来源：http://hz.shuidangran.top/gtxfdoency.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtdwzejstu.html

guard let x = opt else { return }
来源：http://hz.aibaodan.cn/gtiiltfalc.html

[T30] Swift：协议
来源：http://hz.jinqigufen.top/gtnnouogwj.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gtwohlyjwn.html

[T31] Lua：Hello World
来源：http://hz.ppjwa.cn/gtjvqxvtiy.html

print("Hello")
来源：http://hz.guowangkeji.top/gtvudaenac.html

[T32] Lua：局部变量
来源：http://hz.zhengqikj.top/gtryujmdfb.html

local a = 1
来源：http://hz.sysykeji.top/gtajmukhtw.html

[T33] Lua：表（数组）
来源：http://hz.hongshengwenyu.top/gtzfdqlxlm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jlsjyb.cn/gtjavpbggu.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtkbiyajmw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangshuangyany.cn/gtxbzwxmzu.html

[T35] Lua：字典表
来源：http://hz.feifeiyinyue.top/gthafesyxw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cheryme.top/gtyuplzusy.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gtzolwtuza.html

function add(a, b) return a + b end
来源：http://hz.cashguo.top/gtrxvvumgq.html

[T37] Lua：字符串拼接
来源：http://hz.yuxming.cn/gtimkgtzil.html

"a" .. "b"
来源：http://hz.jlsjyb.cn/gtvcjyhruz.html

[T38] Lua：条件
来源：http://hz.nanxuanxn.top/gtdzftxetl.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtkcpnsius.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtmsyxwvfo.html

string.find(s, "%d+")
来源：http://hz.jinqigfzy.top/gtacqunvms.html

[T40] Lua：元表
来源：http://hz.cashguo.top/gtoelrrpxh.html

setmetatable({}, { __index = base })
来源：http://hz.cqqwz.cn/gtmrkgixmj.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtmpfkczgk.html

print "Hello\n";
来源：http://hz.tian-w.cn/gtfcerhonr.html

[T42] Perl：变量类型
来源：http://hz.tianlin.xyz/gtdqvwbtak.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hnxiangtu.top/gtcmdggick.html

[T43] Perl：字符串插值
来源：http://hz.jianghu66.top/gtooperozv.html

"值: $a"
来源：http://hz.yongpay.top/gtrhpbaynn.html

[T44] Perl：条件
来源：http://hz.gzhubu.top/gtrgsuyjlp.html

if ($a > 0) { print "正"; }
来源：http://hz.iojbl.cn/gtaqbecxla.html

[T45] Perl：数组遍历
来源：http://hz.0kj1m.cn/gtufhdehhb.html

for my $x (@arr) { print $x; }
来源：http://hz.redwolf501.top/gteqlelqtg.html

[T46] Perl：哈希操作
来源：http://hz.shuidangran.top/gtufjvbdyy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.dashuyun.cn/gtmttmjaqz.html

[T47] Perl：正则捕获
来源：http://hz.c1oappe.top/gtcpfsiqiq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hongshengwenyu.top/gtwxuckidv.html

[T48] Perl：正则替换
来源：http://hz.yangfankeji.com/gtdaazlpja.html

$s =~ s/old/new/g;
来源：http://hz.nwbrower.top/gtdbsmnbtt.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtxahqdctt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gtofnxvrzd.html

[T50] Perl：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtlmwklqxq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuanzhike.top/gtsdrntohu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jyoumei.cn/gtzdlzgypq.html

[T51] Scala：Hello World
来源：http://hz.shangyingyoupin.top/gtggfbicqi.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtunfgrtzz.html

[T52] Scala：变量
来源：http://hz.zdqjudy.top/gtxdvdaxzc.html

val a = 1;  var b = 2
来源：http://hz.gogol.net.cn/gtlrrcnxze.html

[T53] Scala：字符串插值
来源：http://hz.snrcjt.cn/gtmspyukil.html

s"值: $b"
来源：http://hz.ydjk.org.cn/gtetmahuld.html

[T54] Scala：集合映射
来源：http://hz.hnxiangtu.top/gtnzxcvomn.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.andypj.xyz/gthemchxmk.html

[T55] Scala：集合过滤
来源：http://hz.shangyingyoupin.top/gtyqrtxiit.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.andypj.xyz/gtfukettgz.html

[T56] Scala：样例类
来源：http://hz.zhixingplan.top/gtrroclulz.html

case class User(name: String, age: Int)
来源：http://hz.xylfe.cn/gtzdopltgc.html

[T57] Scala：模式匹配
来源：http://hz.yj20258.top/gtnepfilnh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.52xcode.cn/gtquefigxv.html

[T58] Scala：函数定义
来源：http://hz.birdmap.top/gttpcscuyz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jianghu66.top/gtpccmmbqm.html

[T59] Scala：循环
来源：http://hz.pycfn.com/gtodifcajj.html

for (i <- 1 to 10) println(i)
来源：http://hz.jyoumei.cn/gtpcxixolo.html

[T60] Scala：折叠
来源：http://hz.c1oappe.top/gtetfgbick.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daria6918.cn/gtuwsygraw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtzbchfpts.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtatvqnkun.html

================================================================================
来源：http://hz.yj20258.top/gtezwtxlkl.html

[U01] Py：创建虚拟环境
来源：http://hz.cheryme.top/gtjvnhaqlx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gtcyavrflb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydjk.org.cn/gtewfgfwbt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.9152youxi.cn/gtsgvnzxpi.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gtvyrmwsgh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jlsjyb.cn/gtkubfdcej.html

[U04] Py：变量调试打印
来源：http://hz.tanke756.top/gtjtplmtly.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.quarkkingdee.top/gtawnztzpo.html

[U05] Py：列表去重且保序
来源：http://hz.yonumen.top/gtpyqgmvba.html

list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtvqnxezym.html

[U06] Py：合并两个字典
来源：http://hz.bjfxy.top/gtcwfkzuiz.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtlkthonrm.html

[U07] Py：反转字典键值
来源：http://hz.yanxiufei.cn/gtpkmbhuoy.html

{v: k for k, v in d.items()}
来源：http://hz.yangfankeji.com/gtwlfqfzbu.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtzeyvffyn.html

[y for x in nested for y in x]
来源：http://hz.yangfankeji.com/gtdfecragi.html

[U09] Py：字典取最大值的键
来源：http://hz.bjfxy.top/gtwazqgjyn.html

max(d, key=d.get)
来源：http://hz.xinyue.icu/gtjllqznrz.html

[U10] Py：按值排序字典
来源：http://hz.haohaochexian.top/gtiqahrfnr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shanyushiyangtech.top/gtpbvzqcbp.html

[U11] Py：生成器表达式
来源：http://hz.shanyushiyangkeji.top/gtkthmpzbb.html

(x * 2 for x in arr)
来源：http://hz.redwolf501.top/gtpsnibvdv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daria6918.cn/gtywhhkzvu.html

Counter(arr).most_common(3)
来源：http://hz.shanyushiyangkeji.top/gtearjvjvv.html

[U13] Py：固定长度队列
来源：http://hz.ybcxt.top/gtvpywotnn.html

deque(maxlen=10)
来源：http://hz.daria6918.cn/gtxdpjnihk.html

[U14] Py：分组收集到列表
来源：http://hz.dashuyun.cn/gtsntqvuoh.html

defaultdict(list)
来源：http://hz.sweek.top/gtwthtjwvd.html

[U15] Py：高精度计时
来源：http://hz.zhijiandao.cn/gtpubvgnlu.html

t = time.perf_counter()
来源：http://hz.dashuyun.cn/gtckrfahlx.html

[U16] Py：命令行参数解析
来源：http://hz.dashuyun.cn/gtqnctjgly.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jqgufenzy.top/gtlrcgfkem.html

[U17] Py：初始化日志
来源：http://hz.hammf.cn/gtuaygkqot.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jqgufenzy.top/gtxzbtuijv.html

[U18] Py：预编译正则
来源：http://hz.guowangkeji.top/gtzrfyvlnn.html

pat = re.compile(r"\d+")
来源：http://hz.birdmap.top/gthtalffeo.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtszblhxpe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gogol.net.cn/gtosvhgbej.html

[U20] Py：缓存函数结果
来源：http://hz.vqdsnc.cn/gtwimizmie.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xylfe.cn/gtxuszjhlt.html

[U21] Py：自定义上下文管理器
来源：http://hz.ivvv.top/gtzfbtrxzt.html

@contextlib.contextmanager
来源：http://hz.ivvv.top/gtawnmupdv.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtksipgvpi.html

list(zip(*m))
来源：http://hz.wangdashe.top/gtsoemjonj.html

[U23] Py：分块读取大文件
来源：http://hz.hnxiangtu.top/gtpsjnerak.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fengsongda.top/gtllzxfsqe.html

[U24] Py：路径操作
来源：http://hz.nanxinkj.top/gtnepxssbt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhijiandao.cn/gtxuhyydkd.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtuegnlfhd.html

csv.DictReader(f)
来源：http://hz.nanxinkj.top/gtmprztobp.html

[U26] Py：并发下载
来源：http://hz.pengpengdd.cyou/gtfcbbtamy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cucudq.cn/gtjiteyjqy.html

[U27] Py：异步 HTTP
来源：http://hz.tanke756.top/gtxhnpilod.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xylfe.cn/gtnsfapacr.html

[U28] Py：类型别名
来源：http://hz.jinyuanbaomall.cn/gtczaeuacm.html

UserId = int
来源：http://hz.zdqjudy.top/gtpzjsbcoi.html

[U29] Py：属性校验
来源：http://hz.bjfxy.top/gtmvnepbmy.html

@property 与 @x.setter 配合
来源：http://hz.shanyushiyangtech.top/gtnabxgnmx.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtawmdyerd.html

@dataclass(slots=True)
来源：http://hz.mhx1999.top/gtktmjwiij.html

[U31] Py：单测
来源：http://hz.guowangkeji.top/gteebgikaj.html

python -m pytest -q
来源：http://hz.sxryk.cn/gtwbzwwlnk.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangkeji.top/gtvtuqoinw.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtrbvriowb.html

[U33] Py：打包发布
来源：http://hz.iojbl.cn/gtqewjozow.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.aibaodan.cn/gtuknfperb.html

[U34] Py：判断编码
来源：http://hz.dianchejie.cn/gtmykwkpua.html

chardet.detect(raw)
来源：http://hz.hfpthk.cn/gtyomyabbn.html

[U35] Py：发送邮件
来源：http://hz.aibaodan.cn/gtnbxbrawo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinqigfzy.top/gtiyhrpehy.html

[U36] Py：定时任务
来源：http://hz.gogol.net.cn/gtwpfvxbsx.html

schedule.every(10).minutes.do(job)
来源：http://hz.jlsjyb.cn/gtzgakdhan.html

[U37] Py：读写 Excel
来源：http://hz.fengsongda.top/gtvtdnxeai.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtkangolnf.html

[U38] Py：获取脚本所在目录
来源：http://hz.cashguo.top/gtoaawlrdj.html

Path(__file__).resolve().parent
来源：http://hz.gzhubu.top/gtniiwtjon.html

[U39] Py：判断是否在交互环境
来源：http://hz.yuanzhike.top/gtfpyvfjaz.html

sys.stdout.isatty()
来源：http://hz.redwolf501.top/gtkvzvbbih.html

[U40] Py：打印到标准错误
来源：http://hz.pycfn.com/gtpnbgkcak.html

print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtiafnotab.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.andypj.xyz/gtkmjssymb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sxryk.cn/gtkpiitzeh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangtech.top/gtxbbqyhbj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.smart0.xyz/gtemlslegz.html

[U43] PHP：声明命名空间
来源：http://hz.jinqigufen.top/gtyzamkzsg.html

namespace App\Http;
来源：http://hz.0kj1m.cn/gtyqzkjjvq.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtyijagwfy.html

declare(strict_types=1);
来源：http://hz.jianghu66.top/gthoqggopk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ehwqpu.com/gttesvisul.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtifbrkbjy.html

[U46] PHP：可空类型
来源：http://hz.zhengqikj.top/gtlhjvbkuy.html

?string $name = null
来源：http://hz.jinghuilouyu.cn/gtqkkmnrjs.html

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gthfmbytds.html

int|string $id
来源：http://hz.xuanzx.com/gtocsvmbgd.html

[U48] PHP：纯枚举
来源：http://hz.zycfv.cn/gtiuqyzneo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.9152youxi.cn/gtvzlopopd.html

[U49] PHP：只读属性
来源：http://hz.iojbl.cn/gtvcfbalzy.html

public readonly string $name
来源：http://hz.yj20258888.top/gtvujypdfe.html

[U50] PHP：构造器属性提升
来源：http://hz.yangfankeji.com/gtyjjdnqph.html

public function __construct(private int $id) {}
来源：http://hz.yangfankeji.com/gtyfspvcta.html

[U51] PHP：数组解构
来源：http://hz.ybcxt.top/gtkubesage.html

[$a, $b] = $arr;
来源：http://hz.cucudq.cn/gtqftvvlga.html

[U52] PHP：箭头函数
来源：http://hz.c1oappe.top/gttdmvryba.html

$double = fn($x) => $x * 2;
来源：http://hz.redwolf501.top/gtxmywkrky.html

[U53] PHP：空合并运算符
来源：http://hz.andypj.xyz/gteacrwxpi.html

$v = $a ?? $b ?? "default";
来源：http://hz.aibaodan.cn/gtythtgckg.html

[U54] PHP：空安全调用
来源：http://hz.xziqi.cn/gtrgreizds.html

$obj?->method()
来源：http://hz.andypj.xyz/gtwucjnxqc.html

[U55] PHP：match 表达式
来源：http://hz.zhoulong.xyz/gtlnzeufst.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yj20258.top/gtusuzfeqp.html

[U56] PHP：命名参数
来源：http://hz.52xcode.cn/gtwcphzqmo.html

f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtjtjagkkn.html

[U57] PHP：字符串插值
来源：http://hz.hnxiangtu.top/gtcakprzxr.html

"值: {$a}"
来源：http://hz.havefunace.top/gtpbmgjgip.html

[U58] PHP：数组三件套
来源：http://hz.chenjidiqi.icu/gtczrrejod.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinghuilouyu.cn/gtvjmdjsuf.html

[U59] PHP：自定义排序
来源：http://hz.hongshengwenyu.top/gtxlavpvcn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnxiangtu.top/gthhahgnia.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtbcpccieu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yanxiufei.cn/gtuopocbkr.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gtihuopeeh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtocnkiuwh.html

[U62] PHP：日期对象
来源：http://hz.ivvv.top/gtetuwjghx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxinkj.top/gtsugecsvz.html

[U63] PHP：文件读写
来源：http://hz.jinqigufen.top/gtorkrdykf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shzxlz.cn/gtphhwfekk.html

[U64] PHP：目录遍历
来源：http://hz.xuanzx.com/gtektfdudw.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jqgufenzy.top/gtpjehrxkd.html


<!-- 参考信息 -->