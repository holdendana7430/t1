代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtmhkuozng.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.wangshuangyany.cn/gtfpthxujh.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtjhtjesmh.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtlfosqfqu.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtooywafey.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gtzxcxqami.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gttlucwrwq.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtdhkhrvfq.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtsuwlftht.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.svipenyu.cn/gtcswuzgix.html

[S46] C++：函数模板
来源：http://hz.fzhhl.top/gtclxhhkbu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtjuzuvdhg.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtbawjemde.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.bjfxy.top/gtmhmrqsta.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gthblyfsun.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtnocfwhzd.html

while (std::getline(in, line)) { }
来源：http://hz.c1oappe.top/gtiwsmcpwc.html

[S49] C++：写文件
来源：http://hz.9152youxi.cn/gtjpptvelt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenzaomai.com/gtaqxwznuq.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtcckptvxw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhengqikj.top/gtcrnmqxez.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtcrxisgqw.html

static_cast<double>(a) / b
来源：http://hz.hnqzz.top/gtdgouocwy.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtoppkvgiw.html

int size() const noexcept { return n_; }
来源：http://hz.ivvv.top/gtpbtzxqwn.html

[S53] C++：移动语义
来源：http://hz.zhiwuduotai.top/gtgaspkeao.html

std::vector<int> w = std::move(v);
来源：http://hz.birdmap.top/gtygibpbge.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtgcyjjsck.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtdzbbqvke.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtcstnebvp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtfwdedypz.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gtfkyvwfkn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cheryme.top/gtvwtdecuj.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtnyvmtmgd.html

constexpr int N = 10;
来源：http://hz.pengpengdd.cyou/gtsifhhefa.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtjwptpejo.html

namespace ns { int f() { return 1; } }
来源：http://hz.tianlin.xyz/gtbelvnnyo.html

[S59] C++：静态断言
来源：http://hz.sufxvd.cn/gttojjzujl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shzxlz.cn/gtkruipcev.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtzxltjsom.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhengqikj.top/gttezsfaut.html

================================================================================
来源：http://hz.dashuyun.cn/gtwtuaqful.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtnvfpgmui.html

================================================================================
来源：http://hz.svipenyu.cn/gtrdvekpgj.html

[T01] Kotlin：Hello World
来源：http://hz.vqdsnc.cn/gtibeazeeu.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtwbthbxrg.html

[T02] Kotlin：变量
来源：http://hz.nanxinkj.top/gttnpupkkk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj202588.top/gtotsgzwkl.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtbrbrjnmy.html

"值: $b"
来源：http://hz.chenzaomai.com/gtlwaozile.html

[T04] Kotlin：空安全
来源：http://hz.gaohongyu789.top/gtpdwhcxlt.html

val n: String? = null;  n?.length
来源：http://hz.snrcjt.cn/gtfmkpuwjk.html

[T05] Kotlin：when 表达式
来源：http://hz.dianchejie.cn/gtugyhbpoi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtctkgalyr.html

[T06] Kotlin：集合映射
来源：http://hz.hysaishi.cn/gtvyszndba.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtrgzxqcvf.html

[T07] Kotlin：集合过滤
来源：http://hz.cdnleiting.top/gtqrtpqexo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258.top/gtckydzpts.html

[T08] Kotlin：数据类
来源：http://hz.snrcjt.cn/gtkclnuvyl.html

data class User(val name: String, val age: Int)
来源：http://hz.birdmap.top/gtvtkkwaox.html

[T09] Kotlin：扩展函数
来源：http://hz.ppjwa.cn/gtdiopbimr.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtldvtgzsf.html

[T10] Kotlin：默认参数
来源：http://hz.cashguo.top/gtoukooomy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtdzpjbyrj.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtdmclgyot.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gtshadsiyl.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangtech.top/gtfrshajmp.html

val (a, b) = Pair(1, 2)
来源：http://hz.svipenyu.cn/gtqsqbyzag.html

[T13] Kotlin：只读 Map
来源：http://hz.xziqi.cn/gtoocawxte.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gtjnfmwxza.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gttxonbjbg.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtiodgfnxw.html

[T15] Kotlin：接口
来源：http://hz.ybcxt.top/gtgvqpsvbs.html

interface Shape { fun area(): Double }
来源：http://hz.pengpengdd.cyou/gtgjaigcco.html

[T16] Swift：Hello World
来源：http://hz.chenjidiqi.icu/gtuikzfyqa.html

print("Hello")
来源：http://hz.bjfxy.top/gtdqdjnsoi.html

[T17] Swift：变量与常量
来源：http://hz.xylfe.cn/gtrjwlyxgk.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtuifdjnzp.html

[T18] Swift：字符串插值
来源：http://hz.c1oappe.top/gtwsyulogf.html

"值: \(b)"
来源：http://hz.haohaochexian.top/gtjinzkkip.html

[T19] Swift：可选绑定
来源：http://hz.chenjidiqi.icu/gtzzlmbplv.html

if let n = opt { print(n) }
来源：http://hz.snrcjt.cn/gtypwcwaya.html

[T20] Swift：数组操作
来源：http://hz.jinqigufen.top/gtrsfhhuuw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xuanzx.com/gtknyirgwf.html

[T21] Swift：遍历
来源：http://hz.daxiang520.top/gtajrpadot.html

for x in a { print(x) }
来源：http://hz.meibo888.top/gtlgsypctl.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtdcvwetbv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.bjfxy.top/gtxtjvzvpn.html

[T23] Swift：函数
来源：http://hz.zhaomingkeji.xyz/gttzaaisdj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtmcphzybg.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gtrztbgnrq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tianlin.xyz/gtftqmmwje.html

[T25] Swift：结构体
来源：http://hz.dashuyun.cn/gtkxaboalb.html

struct P { var x: Int }
来源：http://hz.sweek.top/gtxcbojbux.html

[T26] Swift：类与重写
来源：http://hz.xylfe.cn/gtbmmjlrra.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gttqhvocgp.html

[T27] Swift：错误处理
来源：http://hz.tanke756.top/gttpnwnlnk.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gthgycrdbi.html

[T28] Swift：枚举
来源：http://hz.aibaodan.cn/gtyyccnpwa.html

enum Color { case red, green }
来源：http://hz.sxryk.cn/gtemivuxsz.html

[T29] Swift：guard 提前返回
来源：http://hz.dianchejie.cn/gtaqgrtkms.html

guard let x = opt else { return }
来源：http://hz.yj202588.top/gtclugfixs.html

[T30] Swift：协议
来源：http://hz.yangfankeji.com/gtkuvoswfs.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtshgrhujd.html

[T31] Lua：Hello World
来源：http://hz.jianghu66.top/gtvqdwmutf.html

print("Hello")
来源：http://hz.hfpthk.cn/gtruqrxzbg.html

[T32] Lua：局部变量
来源：http://hz.gaohongyu789.top/gtjxpatsgp.html

local a = 1
来源：http://hz.jinqigufen.top/gtpbgxxqmv.html

[T33] Lua：表（数组）
来源：http://hz.guowangkeji.top/gtvpfmowoc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cucudq.cn/gteklmtssx.html

[T34] Lua：遍历表
来源：http://hz.redwolf501.top/gtkzzpqquz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtyzqhkruq.html

[T35] Lua：字典表
来源：http://hz.wangshuangyany.cn/gtcyngrhle.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yongpay.top/gtviwropmc.html

[T36] Lua：函数
来源：http://hz.dashuyun.cn/gtjvpamxgm.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtuqbzfktl.html

[T37] Lua：字符串拼接
来源：http://hz.shangyingyoupin.top/gtprxsaogc.html

"a" .. "b"
来源：http://hz.chenlongwang.top/gtuirypyax.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtrnrqoazs.html

if x > 0 then print("正") end
来源：http://hz.yj202588.top/gtujhgplrf.html

[T39] Lua：模式匹配
来源：http://hz.cdnleiting.top/gtlvmrvkvb.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtgobafxlw.html

[T40] Lua：元表
来源：http://hz.jianghu66.top/gtxluwgecs.html

setmetatable({}, { __index = base })
来源：http://hz.chenjidiqi.icu/gtkeobigte.html

[T41] Perl：Hello World
来源：http://hz.hongshengwenyu.top/gtcxhjgheq.html

print "Hello\n";
来源：http://hz.jyoumei.cn/gtzivzihzd.html

[T42] Perl：变量类型
来源：http://hz.gotoacloud.top/gtotrczlha.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.svipenyu.cn/gtwuzlrpuo.html

[T43] Perl：字符串插值
来源：http://hz.yj20258.top/gtcdkbffwv.html

"值: $a"
来源：http://hz.jinqigufen.top/gtlcsfivaq.html

[T44] Perl：条件
来源：http://hz.sweek.top/gtvhjkhkbv.html

if ($a > 0) { print "正"; }
来源：http://hz.cashguo.top/gtvufiitfb.html

[T45] Perl：数组遍历
来源：http://hz.ywan-chungtsiang.top/gtvvlovbgb.html

for my $x (@arr) { print $x; }
来源：http://hz.vqdsnc.cn/gtjiuctmfi.html

[T46] Perl：哈希操作
来源：http://hz.iojbl.cn/gtpglsuhgp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigfzy.top/gteltlpzdy.html

[T47] Perl：正则捕获
来源：http://hz.gotoacloud.top/gtxnyewzfx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jinghuilouyu.cn/gtopmeekjt.html

[T48] Perl：正则替换
来源：http://hz.jianghu66.top/gtjctkvsco.html

$s =~ s/old/new/g;
来源：http://hz.wangshuangyany.cn/gtnulumlmb.html

[T49] Perl：函数
来源：http://hz.yonumen.top/gtdwjiwbye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cucudq.cn/gtnbamvfad.html

[T50] Perl：逐行读文件
来源：http://hz.sweek.top/gtfbazvpot.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgfzy.top/gtwswakwcn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhiwuduotai.top/gtazgimpjj.html

[T51] Scala：Hello World
来源：http://hz.shangyingyoupin.top/gtemmxuohc.html

println("Hello")
来源：http://hz.zhongyouzk.top/gtyqexhlxu.html

[T52] Scala：变量
来源：http://hz.hfpthk.cn/gtecmlmldj.html

val a = 1;  var b = 2
来源：http://hz.jqgfzy.top/gtiuiesney.html

[T53] Scala：字符串插值
来源：http://hz.xylfe.cn/gtpcjxhted.html

s"值: $b"
来源：http://hz.9152youxi.cn/gtsinarcag.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtmzsizqcf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cucudq.cn/gtzogdudtx.html

[T55] Scala：集合过滤
来源：http://hz.xziqi.cn/gtolfpxtft.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.c1oappe.top/gtbaeszemo.html

[T56] Scala：样例类
来源：http://hz.jinqigfzy.top/gtkkjkghfd.html

case class User(name: String, age: Int)
来源：http://hz.zycfv.cn/gtfyjxutap.html

[T57] Scala：模式匹配
来源：http://hz.cucudq.cn/gtquqhuyqr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hysaishi.cn/gtjynggqdc.html

[T58] Scala：函数定义
来源：http://hz.hnxiangtu.top/gtbmfdbmsb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ywan-chungtsiang.top/gtpvvyfiin.html

[T59] Scala：循环
来源：http://hz.chenlongwang.top/gtetxdszli.html

for (i <- 1 to 10) println(i)
来源：http://hz.pycfn.com/gtkkbrwmnk.html

[T60] Scala：折叠
来源：http://hz.ydjk.org.cn/gtylgedqcz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gtnnpdcsnw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtreowufcn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtsgfvfhff.html

================================================================================
来源：http://hz.yonumen.top/gtvkidxaoa.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtgzlibjfg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258.top/gtqqcxptsg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhoulong.xyz/gtsiprvejm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.52xcode.cn/gtlwflaeid.html

[U03] Py：加载 .env 配置
来源：http://hz.xingfuxueyuan.xyz/gtjxarzeas.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tian-w.cn/gtkaeqsxxu.html

[U04] Py：变量调试打印
来源：http://hz.hongshengwenyu.top/gtbhdgubvo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hysaishi.cn/gtqigmdvud.html

[U05] Py：列表去重且保序
来源：http://hz.feifeiyinyue.top/gttycnanbh.html

list(dict.fromkeys(arr))
来源：http://hz.ybcxt.top/gthxkgsygi.html

[U06] Py：合并两个字典
来源：http://hz.xinyue.icu/gtevikqlfr.html

{**a, **b}
来源：http://hz.shuidangran.top/gtwnwwcvty.html

[U07] Py：反转字典键值
来源：http://hz.gotoacloud.top/gtrwjxamqm.html

{v: k for k, v in d.items()}
来源：http://hz.yangfankeji.com/gtbajdeujk.html

[U08] Py：展平二维列表
来源：http://hz.52xcode.cn/gtvjpasrzc.html

[y for x in nested for y in x]
来源：http://hz.hysaishi.cn/gtdrzqyddf.html

[U09] Py：字典取最大值的键
来源：http://hz.tanke756.top/gtnjbaiqfm.html

max(d, key=d.get)
来源：http://hz.zhengqikj.top/gtuxmzfngz.html

[U10] Py：按值排序字典
来源：http://hz.hysaishi.cn/gtdsuueulg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtwlfadhhw.html

[U11] Py：生成器表达式
来源：http://hz.nanxuanxn.top/gthedsdxpj.html

(x * 2 for x in arr)
来源：http://hz.ehwqpu.com/gtasuohbxe.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhengqikj.top/gteqzjzsio.html

Counter(arr).most_common(3)
来源：http://hz.yongpay.top/gtdmfqqxkh.html

[U13] Py：固定长度队列
来源：http://hz.hnqzz.top/gtzzridens.html

deque(maxlen=10)
来源：http://hz.nanxinkj.top/gtewrljfvw.html

[U14] Py：分组收集到列表
来源：http://hz.ybcxt.top/gtiyyutpax.html

defaultdict(list)
来源：http://hz.jianghu66.top/gthihahsic.html

[U15] Py：高精度计时
来源：http://hz.jinyuanbaomall.cn/gtkryqutfe.html

t = time.perf_counter()
来源：http://hz.bjfxy.top/gtyihwjfbq.html

[U16] Py：命令行参数解析
来源：http://hz.chenjidiqi.icu/gtoqjhqyql.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cucudq.cn/gtjdlhnkze.html

[U17] Py：初始化日志
来源：http://hz.zhixingplan.top/gtuqickbfq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ywan-chungtsiang.top/gtmutikwyk.html

[U18] Py：预编译正则
来源：http://hz.0kj1m.cn/gtvcclaxqq.html

pat = re.compile(r"\d+")
来源：http://hz.zhiwuduotai.top/gtsnmoflae.html

[U19] Py：正则替换带回调
来源：http://hz.gogol.net.cn/gtspgsgdxk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtwtzppjdm.html

[U20] Py：缓存函数结果
来源：http://hz.cqqwz.cn/gtzgearvvu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gtpjypvcbs.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gtizmoucqt.html

@contextlib.contextmanager
来源：http://hz.zycfv.cn/gtvmxugyqw.html

[U22] Py：矩阵转置
来源：http://hz.yuanzhike.top/gtwenqfpii.html

list(zip(*m))
来源：http://hz.snrcjt.cn/gtvwgtfafn.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gteboiijjs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xylfe.cn/gttqeqmlxm.html

[U24] Py：路径操作
来源：http://hz.xylfe.cn/gtalxdhdfj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gotoacloud.top/gtneicquqg.html

[U25] Py：CSV 按字典读
来源：http://hz.shuidangran.top/gtqymxmisi.html

csv.DictReader(f)
来源：http://hz.hywenlv.cn/gtrbtbhatl.html

[U26] Py：并发下载
来源：http://hz.tanke756.top/gtizwnaajw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cucudq.cn/gtkoqhxwgo.html

[U27] Py：异步 HTTP
来源：http://hz.cashguo.top/gtcaerghxf.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yongpay.top/gthexlgcnn.html

[U28] Py：类型别名
来源：http://hz.zhijiandao.cn/gtvnsjtyyd.html

UserId = int
来源：http://hz.tianlin.xyz/gtajnjfquj.html

[U29] Py：属性校验
来源：http://hz.mhx1999.top/gtsuwqfawz.html

@property 与 @x.setter 配合
来源：http://hz.nanxuanxn.top/gtjnfqapcc.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtupvbcoep.html

@dataclass(slots=True)
来源：http://hz.yj20258888.top/gtxmspcvwd.html

[U31] Py：单测
来源：http://hz.ydjk.org.cn/gtscwqzawt.html

python -m pytest -q
来源：http://hz.zhengqikj.top/gtgndpnonj.html

[U32] Py：代码格式化
来源：http://hz.fzhhl.top/gtyxxpnicd.html

ruff format . && ruff check --fix .
来源：http://hz.havefunace.top/gtftzegiqm.html

[U33] Py：打包发布
来源：http://hz.jqgfzy.top/gtuwctvkqh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtoszsfssp.html

[U34] Py：判断编码
来源：http://hz.yvedp.cn/gtrxrrpaqu.html

chardet.detect(raw)
来源：http://hz.316326.xyz/gtnwtqgqvx.html

[U35] Py：发送邮件
来源：http://hz.hnqzz.top/gtpizqwiid.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jianghu66.top/gthroqvvsa.html

[U36] Py：定时任务
来源：http://hz.xylfe.cn/gtehknyovo.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtcazdjnsl.html

[U37] Py：读写 Excel
来源：http://hz.sxryk.cn/gtqfsuoyyu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aizwys.cn/gtiqpkhrvv.html

[U38] Py：获取脚本所在目录
来源：http://hz.ywan-chungtsiang.top/gtyfaxapxn.html

Path(__file__).resolve().parent
来源：http://hz.bjfxy.top/gtbbovfitu.html

[U39] Py：判断是否在交互环境
来源：http://hz.316326.xyz/gtzeguhqid.html

sys.stdout.isatty()
来源：http://hz.cucudq.cn/gtbsmbmhwc.html

[U40] Py：打印到标准错误
来源：http://hz.gaohongyu789.top/gtjnfgxbjo.html

print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtwfmayqde.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nanxuanxn.top/gtnqyfdtve.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.smart0.xyz/gtsjbivdaj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnxiangtu.top/gtgllablwq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xinyue.icu/gtzmnoxjrf.html

[U43] PHP：声明命名空间
来源：http://hz.ydjk.org.cn/gtxtismcgl.html

namespace App\Http;
来源：http://hz.ppjwa.cn/gtbcdhvwwj.html

[U44] PHP：开启严格类型
来源：http://hz.jiagoushi.top/gtkpefmsqq.html

declare(strict_types=1);
来源：http://hz.hnxiangtu.top/gtnmcrhiom.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hfpthk.cn/gtigkgxnzj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtkyzfmtbu.html

[U46] PHP：可空类型
来源：http://hz.yongpay.top/gtjazwlnje.html

?string $name = null
来源：http://hz.ydzc1.top/gtwaxsomgk.html

[U47] PHP：联合类型
来源：http://hz.gotoacloud.top/gtsoqvzwwi.html

int|string $id
来源：http://hz.tianlin.xyz/gtdonqakuo.html

[U48] PHP：纯枚举
来源：http://hz.vqdsnc.cn/gtmijzhahd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhoulong.xyz/gtgkxzwwwn.html

[U49] PHP：只读属性
来源：http://hz.xylfe.cn/gtlfmymgyj.html

public readonly string $name
来源：http://hz.c1oappe.top/gtyrpjhbpm.html

[U50] PHP：构造器属性提升
来源：http://hz.meibo888.top/gtrensbdau.html

public function __construct(private int $id) {}
来源：http://hz.bjfxy.top/gtkovgbzfs.html

[U51] PHP：数组解构
来源：http://hz.yonumen.top/gtyglqwpfa.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtxukeyaer.html

[U52] PHP：箭头函数
来源：http://hz.hfpthk.cn/gtgxosrhmt.html

$double = fn($x) => $x * 2;
来源：http://hz.ivvv.top/gtygvrhmjm.html

[U53] PHP：空合并运算符
来源：http://hz.yonumen.top/gtbbmaysgw.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydjk.org.cn/gtbgeyhmbk.html

[U54] PHP：空安全调用
来源：http://hz.cdnleiting.top/gttcgidulj.html

$obj?->method()
来源：http://hz.gotoacloud.top/gtgezlclno.html

[U55] PHP：match 表达式
来源：http://hz.fzhhl.top/gtcjnjuwwn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sysykeji.top/gtileaqfix.html

[U56] PHP：命名参数
来源：http://hz.zhixingplan.top/gthkfflcml.html

f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gteddhnlse.html

[U57] PHP：字符串插值
来源：http://hz.yvedp.cn/gtmpavjtlp.html

"值: {$a}"
来源：http://hz.jinqigufen.top/gtgaajywou.html

[U58] PHP：数组三件套
来源：http://hz.shanyushiyangkeji.top/gtnmqcroii.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shangyingyoupin.top/gtvgitomoo.html

[U59] PHP：自定义排序
来源：http://hz.gogol.net.cn/gtggqxpbjj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnqzz.top/gtgbebfbck.html

[U60] PHP：JSON 编解码
来源：http://hz.cqqwz.cn/gtkokxkyjd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yueranfly.top/gteesrmocg.html

[U61] PHP：正则
来源：http://hz.shuidangran.top/gtlhhzoutw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtuuuvsgwi.html

[U62] PHP：日期对象
来源：http://hz.sweek.top/gtraufjgrc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jiagoushi.top/gtqjcjalhe.html

[U63] PHP：文件读写
来源：http://hz.redwolf501.top/gtyvbqrgzt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangkeji.top/gtssmngayq.html

[U64] PHP：目录遍历
来源：http://hz.daxiang520.top/gtfnifznet.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.snrcjt.cn/gtmcmggudb.html

[U65] PHP：会话
来源：http://hz.shzxlz.cn/gtjteobugu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dianchejie.cn/gthmmeqeri.html

[U66] PHP：设置 Cookie
来源：http://hz.dianchejie.cn/gtxkzlegxy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.haohaochexian.top/gtmivmruyc.html


<!-- 参考信息 -->