代发 wailian999

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtfcjkpfkx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.mhx1999.top/gtssoghtib.html

[S46] C++：函数模板
来源：http://hz.shuidangran.top/gtokargshl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtryesnyll.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtzuubpdpk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuxming.cn/gtqvllhxzy.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtbzdjmqqx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuanzx.com/gtlgxpnwfj.html

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtafofaaju.html

[S49] C++：写文件
来源：http://hz.xylfe.cn/gtcoortgdn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gttovesnzh.html

[S50] C++：格式化数字
来源：http://hz.xingfuxueyuan.xyz/gtmkocrigf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtnogunmvf.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtkdabzoct.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtwndztuhj.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtablrthzv.html

int size() const noexcept { return n_; }
来源：http://hz.ppjwa.cn/gttqnumlay.html

[S53] C++：移动语义
来源：http://hz.nwbrower.top/gtpoudemky.html

std::vector<int> w = std::move(v);
来源：http://hz.zhoulong.xyz/gthpjxofxu.html

[S54] C++：异常处理
来源：http://hz.yuxming.cn/gtjuiardvf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtfewirhbq.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtdvmeecld.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtivhjxbkh.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtkdwkgart.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.feifeiyinyue.top/gtodkzcbik.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtkxgriqfv.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtwpmhrbyu.html

[S58] C++：命名空间
来源：http://hz.hfpthk.cn/gtilqyulmm.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtjncvzlny.html

[S59] C++：静态断言
来源：http://hz.sysykeji.top/gtkwuiohyn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtzovyyyyv.html

[S60] C++：遍历并删除元素
来源：http://hz.pengpengdd.cyou/gtulmyddkq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cashguo.top/gtkrvsdrxe.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuwluogim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtbqrnwhtz.html

================================================================================
来源：http://hz.aibaodan.cn/gtxatfesuh.html

[T01] Kotlin：Hello World
来源：http://hz.xinyue.icu/gtwvtuenir.html

println("Hello")
来源：http://hz.nanxinkj.top/gtqhvhttxo.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gterzbebir.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jiagoushi.top/gtzubbvzqh.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtnbrsskmi.html

"值: $b"
来源：http://hz.yanxiufei.cn/gtxenlxcaq.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtsdxwsxpa.html

val n: String? = null;  n?.length
来源：http://hz.zhiwuduotai.top/gtvakilkgh.html

[T05] Kotlin：when 表达式
来源：http://hz.aibaodan.cn/gtrshhrrtj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cdnleiting.top/gtyhpvmfzt.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gtemzuioyi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gteaazellc.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gttzkelnij.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtybmtdqtc.html

[T08] Kotlin：数据类
来源：http://hz.aibaodan.cn/gtvkhcgtpj.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtnuhsiuys.html

[T09] Kotlin：扩展函数
来源：http://hz.gotoacloud.top/gtbawgkzfp.html

fun String.exclaim() = this + "!"
来源：http://hz.yongpay.top/gtdgdumnhc.html

[T10] Kotlin：默认参数
来源：http://hz.cheryme.top/gtaqoqedei.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtfkshwhrp.html

[T11] Kotlin：协程
来源：http://hz.mhx1999.top/gtclhwxbrz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtfshwsevw.html

[T12] Kotlin：解构声明
来源：http://hz.feifeiyinyue.top/gtzxgovmpv.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtfblqbnpf.html

[T13] Kotlin：只读 Map
来源：http://hz.yvedp.cn/gtglorgnnk.html

val m = mapOf("a" to 1)
来源：http://hz.gzhubu.top/gtyqjsppyc.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gtcpagdxdz.html

for (i in 1..10) println(i)
来源：http://hz.cheryme.top/gtmsepazhe.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtwpszymnb.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtsccbruvu.html

[T16] Swift：Hello World
来源：http://hz.ybcxt.top/gtszalojkf.html

print("Hello")
来源：http://hz.gogol.net.cn/gtblbvtemq.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtkggkjjoz.html

var a = 1;  let b = 2
来源：http://hz.quarkkingdee.top/gtseexcliq.html

[T18] Swift：字符串插值
来源：http://hz.iojbl.cn/gtltdqinwe.html

"值: \(b)"
来源：http://hz.yongpay.top/gtbjezkzjt.html

[T19] Swift：可选绑定
来源：http://hz.cheryme.top/gtlinxsnmg.html

if let n = opt { print(n) }
来源：http://hz.yj20258888.top/gtffxojqrl.html

[T20] Swift：数组操作
来源：http://hz.snrcjt.cn/gtsffnuxkn.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtvkqkuxrb.html

[T21] Swift：遍历
来源：http://hz.jqgufenzy.top/gtirkvydxx.html

for x in a { print(x) }
来源：http://hz.sxryk.cn/gtejrrgwii.html

[T22] Swift：字典
来源：http://hz.ydzc1.top/gtoxnpdfmz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtaveyslmy.html

[T23] Swift：函数
来源：http://hz.zhongyouzk.top/gtlyydlyeu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.aizwys.cn/gttaulonqt.html

[T24] Swift：闭包
来源：http://hz.yonumen.top/gtuwofujac.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtswfkfoiu.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtmsmswbht.html

struct P { var x: Int }
来源：http://hz.aizwys.cn/gtpnvhkvrk.html

[T26] Swift：类与重写
来源：http://hz.jinyuanbaomall.cn/gtyjbfhqur.html

class A: Base { override func f() {} }
来源：http://hz.nwbrower.top/gtrorhspph.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gtyvoihebr.html

do { try f() } catch { print(error) }
来源：http://hz.hfpthk.cn/gtmdbwnhbs.html

[T28] Swift：枚举
来源：http://hz.xuanzx.com/gtdxlczmwl.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtzpmqvfcs.html

[T29] Swift：guard 提前返回
来源：http://hz.zhengqikj.top/gteznbegtg.html

guard let x = opt else { return }
来源：http://hz.jqgfzy.top/gttvijrhaj.html

[T30] Swift：协议
来源：http://hz.jlsjyb.cn/gtxwspmfug.html

protocol Shape { func area() -> Double }
来源：http://hz.nanxinkj.top/gtbkxkpluc.html

[T31] Lua：Hello World
来源：http://hz.cqqwz.cn/gtgqkzwblx.html

print("Hello")
来源：http://hz.cdnleiting.top/gttmypabfj.html

[T32] Lua：局部变量
来源：http://hz.yuxming.cn/gtalztntrr.html

local a = 1
来源：http://hz.gogol.net.cn/gthfirbuhg.html

[T33] Lua：表（数组）
来源：http://hz.havefunace.top/gtlgpiqgqi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cashguo.top/gtimdlzbyx.html

[T34] Lua：遍历表
来源：http://hz.dianchejie.cn/gtvpxwagov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sysykeji.top/gtervslmnh.html

[T35] Lua：字典表
来源：http://hz.chenjidiqi.icu/gtvihyhilt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nwbrower.top/gtzbcxxbbc.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gtdzpkqwrv.html

function add(a, b) return a + b end
来源：http://hz.xinyue.icu/gtcysueqmo.html

[T37] Lua：字符串拼接
来源：http://hz.andypj.xyz/gtqtpntqxr.html

"a" .. "b"
来源：http://hz.jqgufenzy.top/gtocauoibd.html

[T38] Lua：条件
来源：http://hz.sxryk.cn/gtihldlqie.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangtech.top/gtstiolnye.html

[T39] Lua：模式匹配
来源：http://hz.jiagoushi.top/gtjcjdnozw.html

string.find(s, "%d+")
来源：http://hz.fzhhl.top/gtyokqilnz.html

[T40] Lua：元表
来源：http://hz.cheryme.top/gtrgogxqks.html

setmetatable({}, { __index = base })
来源：http://hz.jqgfzy.top/gtetqaaeyv.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtebdywjqz.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtwkojdlnn.html

[T42] Perl：变量类型
来源：http://hz.yj20258.top/gtfbgqeluz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hysaishi.cn/gtrcjpdcxl.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtxcjbmxee.html

"值: $a"
来源：http://hz.daxiang520.top/gtwukwceke.html

[T44] Perl：条件
来源：http://hz.chenlongwang.top/gtvmtcrjvc.html

if ($a > 0) { print "正"; }
来源：http://hz.pengpengdd.cyou/gtkvtosuui.html

[T45] Perl：数组遍历
来源：http://hz.xinyue.icu/gtyeghelph.html

for my $x (@arr) { print $x; }
来源：http://hz.hywenlv.cn/gtkrgtfomu.html

[T46] Perl：哈希操作
来源：http://hz.xuanzx.com/gtxdvxmkuz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fzhhl.top/gtmnvfxsnw.html

[T47] Perl：正则捕获
来源：http://hz.pycfn.com/gtfpxxqxqr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtsataifrv.html

[T48] Perl：正则替换
来源：http://hz.shzxlz.cn/gtygnorluv.html

$s =~ s/old/new/g;
来源：http://hz.gzhubu.top/gteyktwuex.html

[T49] Perl：函数
来源：http://hz.pycfn.com/gttytrwlnv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtlpsgrfkh.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtfrzvonuy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xziqi.cn/gtiqndqrus.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hysaishi.cn/gtuuzjhlgn.html

[T51] Scala：Hello World
来源：http://hz.yuxming.cn/gtxubbbbpk.html

println("Hello")
来源：http://hz.dashuyun.cn/gtfagfyrva.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gtvognfngc.html

val a = 1;  var b = 2
来源：http://hz.hnxiangtu.top/gtznaonqiq.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gtgysvnzre.html

s"值: $b"
来源：http://hz.cqqwz.cn/gtaacesuii.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtxyttzppf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jianghu66.top/gtzugrfbxw.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gtnvrzfmxg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gthtwuyitk.html

[T56] Scala：样例类
来源：http://hz.xziqi.cn/gtqikmqssv.html

case class User(name: String, age: Int)
来源：http://hz.hnqzz.top/gtllkyoztq.html

[T57] Scala：模式匹配
来源：http://hz.guannengcc.top/gtiwuszxff.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinyuanbaomall.cn/gtixydosmc.html

[T58] Scala：函数定义
来源：http://hz.jyoumei.cn/gtlzwnxumj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258.top/gtjvjiyttg.html

[T59] Scala：循环
来源：http://hz.zhengqikj.top/gtigurrjos.html

for (i <- 1 to 10) println(i)
来源：http://hz.jlsjyb.cn/gtsonhyzzd.html

[T60] Scala：折叠
来源：http://hz.hnqzz.top/gtpnzefpet.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258.top/gtutxyhdva.html

================================================================================
来源：http://hz.xinyue.icu/gtvmymymle.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ivvv.top/gtlrzbpsqw.html

================================================================================
来源：http://hz.birdmap.top/gtkgmxpmqq.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258.top/gticgibsux.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.fzhhl.top/gtlletymmy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.9152youxi.cn/gtequetzsd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhaomingkeji.xyz/gteucadsns.html

[U03] Py：加载 .env 配置
来源：http://hz.hammf.cn/gthobqhuid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jiagoushi.top/gtdstdqvrd.html

[U04] Py：变量调试打印
来源：http://hz.xuetiantiany.cn/gtnacmrwof.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ywan-chungtsiang.top/gttgiiagen.html

[U05] Py：列表去重且保序
来源：http://hz.vqdsnc.cn/gtcipirdbs.html

list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtitwusuuc.html

[U06] Py：合并两个字典
来源：http://hz.cdnleiting.top/gtpxchxjmk.html

{**a, **b}
来源：http://hz.shzxlz.cn/gtzjgxqswc.html

[U07] Py：反转字典键值
来源：http://hz.jinqigufen.top/gtjepufdkv.html

{v: k for k, v in d.items()}
来源：http://hz.xylfe.cn/gtlukyhnch.html

[U08] Py：展平二维列表
来源：http://hz.yj20258888.top/gtggswvspg.html

[y for x in nested for y in x]
来源：http://hz.guowangkeji.top/gtoufncbxk.html

[U09] Py：字典取最大值的键
来源：http://hz.ppjwa.cn/gtpsjcubxb.html

max(d, key=d.get)
来源：http://hz.zhoulong.xyz/gthlvgpdar.html

[U10] Py：按值排序字典
来源：http://hz.ivvv.top/gtvaqkgjpx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sweek.top/gttzpifdly.html

[U11] Py：生成器表达式
来源：http://hz.ppjwa.cn/gttqfsipwq.html

(x * 2 for x in arr)
来源：http://hz.gzhubu.top/gtywdsitqv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gogol.net.cn/gtpmfctwck.html

Counter(arr).most_common(3)
来源：http://hz.haohaochexian.top/gtyaxftmmz.html

[U13] Py：固定长度队列
来源：http://hz.shangyingyoupin.top/gthgimszzk.html

deque(maxlen=10)
来源：http://hz.316326.xyz/gtzilnadpp.html

[U14] Py：分组收集到列表
来源：http://hz.tianlin.xyz/gtkdqechic.html

defaultdict(list)
来源：http://hz.hysaishi.cn/gtssqcykfe.html

[U15] Py：高精度计时
来源：http://hz.jinqigufen.top/gtytjxzygb.html

t = time.perf_counter()
来源：http://hz.cucudq.cn/gttvfftlju.html

[U16] Py：命令行参数解析
来源：http://hz.nwbrower.top/gtdjmhtffi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinyuanbaomall.cn/gtbfjcosmp.html

[U17] Py：初始化日志
来源：http://hz.meibo888.top/gttumzrgfs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hongshengwenyu.top/gtqimkakxb.html

[U18] Py：预编译正则
来源：http://hz.shanyushiyangtech.top/gtdxejjmzf.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtvwxurhwg.html

[U19] Py：正则替换带回调
来源：http://hz.ydzc1.top/gtajsdzlur.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xingfuxueyuan.xyz/gtqrvjtpck.html

[U20] Py：缓存函数结果
来源：http://hz.nwbrower.top/gtpcvrpqhh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxinkj.top/gtrsycxibn.html

[U21] Py：自定义上下文管理器
来源：http://hz.gzhubu.top/gtnvjexkcs.html

@contextlib.contextmanager
来源：http://hz.birdmap.top/gtaknvwrqu.html

[U22] Py：矩阵转置
来源：http://hz.ydzc1.top/gtszpwwqkh.html

list(zip(*m))
来源：http://hz.xuanzx.com/gttswffwdc.html

[U23] Py：分块读取大文件
来源：http://hz.ehwqpu.com/gtaeaehsii.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.andypj.xyz/gtlgkphgiy.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtwlfhhjav.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtsjhazjqv.html

[U25] Py：CSV 按字典读
来源：http://hz.gzhubu.top/gtgsdcersy.html

csv.DictReader(f)
来源：http://hz.yj20258.top/gtgcymqlzk.html

[U26] Py：并发下载
来源：http://hz.0kj1m.cn/gtmjaevulq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gaohongyu789.top/gtiimqzmyt.html

[U27] Py：异步 HTTP
来源：http://hz.hywenlv.cn/gtjmvhquui.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.redwolf501.top/gtzumdatih.html

[U28] Py：类型别名
来源：http://hz.cashguo.top/gtbzaxxrjs.html

UserId = int
来源：http://hz.xziqi.cn/gtpgabeott.html

[U29] Py：属性校验
来源：http://hz.zhoulong.xyz/gthbkwqgww.html

@property 与 @x.setter 配合
来源：http://hz.daxiang520.top/gttmxgxgrd.html

[U30] Py：数据类
来源：http://hz.guowangkeji.top/gtbevmafvf.html

@dataclass(slots=True)
来源：http://hz.cheryme.top/gtgtpgssfq.html

[U31] Py：单测
来源：http://hz.havefunace.top/gtjaeggjht.html

python -m pytest -q
来源：http://hz.0kj1m.cn/gtkvwblmlc.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtenxgyubv.html

ruff format . && ruff check --fix .
来源：http://hz.wangdashe.top/gtxiqdrftk.html

[U33] Py：打包发布
来源：http://hz.nanxuanxn.top/gtalcxieci.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.svipenyu.cn/gtxbiwnsbe.html

[U34] Py：判断编码
来源：http://hz.daria6918.cn/gtyseemiba.html

chardet.detect(raw)
来源：http://hz.nanxuanxn.top/gtmqbtaois.html

[U35] Py：发送邮件
来源：http://hz.birdmap.top/gtmkdrdjlc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ehwqpu.com/gtaawrhdvq.html

[U36] Py：定时任务
来源：http://hz.xziqi.cn/gtlxlrbdcv.html

schedule.every(10).minutes.do(job)
来源：http://hz.daria6918.cn/gtzpovueam.html

[U37] Py：读写 Excel
来源：http://hz.xuetiantiany.cn/gtasolwhaz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinyuanbaomall.cn/gtgcslqcsh.html

[U38] Py：获取脚本所在目录
来源：http://hz.ybcxt.top/gtnlrllajm.html

Path(__file__).resolve().parent
来源：http://hz.guowangkeji.top/gtatarxdyc.html

[U39] Py：判断是否在交互环境
来源：http://hz.aizwys.cn/gtijsomntj.html

sys.stdout.isatty()
来源：http://hz.xinyue.icu/gtfedzwzzn.html

[U40] Py：打印到标准错误
来源：http://hz.dianchejie.cn/gtzwifsrja.html

print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtkljybqxk.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shuidangran.top/gtcbpqvckx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sweek.top/gtzfewjfah.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.daria6918.cn/gtuutgxgxh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuetiantiany.cn/gtnfrmdquh.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gtrwftqmcf.html

namespace App\Http;
来源：http://hz.0kj1m.cn/gtjhpixndy.html

[U44] PHP：开启严格类型
来源：http://hz.fzhhl.top/gtwfsydspb.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtzamtsnma.html

[U45] PHP：类型声明与返回类型
来源：http://hz.kuanghao11.cn/gtilolocyx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtrqvkfnzq.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtbcphxjqd.html

?string $name = null
来源：http://hz.gotoacloud.top/gtwhbkwaup.html

[U47] PHP：联合类型
来源：http://hz.ywan-chungtsiang.top/gtufqqnvde.html

int|string $id
来源：http://hz.zhongyouzk.top/gttdufzmth.html

[U48] PHP：纯枚举
来源：http://hz.yueranfly.top/gtaisizaol.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.fengsongda.top/gtnlbfftwi.html

[U49] PHP：只读属性
来源：http://hz.ivvv.top/gtonatipqf.html

public readonly string $name
来源：http://hz.yj202588.top/gteozzzoun.html

[U50] PHP：构造器属性提升
来源：http://hz.ywan-chungtsiang.top/gtzmpwwbzx.html

public function __construct(private int $id) {}
来源：http://hz.jinqigufen.top/gtwmgphbjk.html

[U51] PHP：数组解构
来源：http://hz.ybcxt.top/gtdjfjmyyc.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtuelyyjno.html

[U52] PHP：箭头函数
来源：http://hz.jiagoushi.top/gtkcsbhdcb.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtleniizsr.html

[U53] PHP：空合并运算符
来源：http://hz.feifeiyinyue.top/gtkprujkxr.html

$v = $a ?? $b ?? "default";
来源：http://hz.0kj1m.cn/gtsbogohwe.html

[U54] PHP：空安全调用
来源：http://hz.sweek.top/gtjtpfusvv.html

$obj?->method()
来源：http://hz.vqdsnc.cn/gtpxmnsird.html

[U55] PHP：match 表达式
来源：http://hz.xuetiantiany.cn/gtkcwogzgl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.jlsjyb.cn/gtwbdzjipg.html

[U56] PHP：命名参数
来源：http://hz.tian-w.cn/gtrfeplrqs.html

f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtbcklsbga.html

[U57] PHP：字符串插值
来源：http://hz.nwbrower.top/gttchvfsob.html

"值: {$a}"
来源：http://hz.ppjwa.cn/gttcidwyei.html

[U58] PHP：数组三件套
来源：http://hz.yuxming.cn/gtyhpiuhon.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.tanke756.top/gtjnjytqvf.html

[U59] PHP：自定义排序
来源：http://hz.birdmap.top/gtdaftxdwe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jlsjyb.cn/gtzxlfqknb.html

[U60] PHP：JSON 编解码
来源：http://hz.ydzc1.top/gthzentxzl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuanzx.com/gtesgdbzwu.html

[U61] PHP：正则
来源：http://hz.bjfxy.top/gtyayyjenn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtxnbblwbp.html

[U62] PHP：日期对象
来源：http://hz.0kj1m.cn/gtxycakkzj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.dashuyun.cn/gtpfdflhuz.html

[U63] PHP：文件读写
来源：http://hz.fzhhl.top/gtoyxvbspn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dianchejie.cn/gttufshkaz.html

[U64] PHP：目录遍历
来源：http://hz.jlsjyb.cn/gtpndcpfqv.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yangfankeji.com/gtrejbczth.html

[U65] PHP：会话
来源：http://hz.jinqigfzy.top/gthotqnlsz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangdashe.top/gtnkjmctcj.html

[U66] PHP：设置 Cookie
来源：http://hz.andypj.xyz/gtktukvscg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtltycuirh.html

[U67] PHP：处理文件上传
来源：http://hz.havefunace.top/gtiwtsuksw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenlongwang.top/gtzfvrqsdv.html

[U68] PHP：PDO 连接
来源：http://hz.zhaomingkeji.xyz/gtwozlnalb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.havefunace.top/gttvuhzbtl.html

[U69] PHP：PDO 预处理
来源：http://hz.cqqwz.cn/gtjakravvb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhoulong.xyz/gtdrigoskx.html

[U70] PHP：PDO 事务
来源：http://hz.ywan-chungtsiang.top/gthptbhase.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.316326.xyz/gtpwgpfcma.html


<!-- 参考信息 -->