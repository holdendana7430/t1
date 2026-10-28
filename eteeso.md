代发 wailian999

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtpcifmnii.html

auto p = std::make_unique<int>(5);
来源：http://hz.snrcjt.cn/gtjyicpheo.html

[S44] C++：引用传参
来源：http://hz.zhiwuduotai.top/gtvjnkjnyw.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gtbpgrjhpe.html

[S45] C++：lambda
来源：http://hz.meibo888.top/gttkdlekon.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.vqdsnc.cn/gtlzjovznm.html

[S46] C++：函数模板
来源：http://hz.ivvv.top/gtvcuyfkrk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aizwys.cn/gtqbmhjuvr.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhaomingkeji.xyz/gtgqdulbem.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtndfpggta.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtiplivxcy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yanxiufei.cn/gtmcgtlxmb.html

while (std::getline(in, line)) { }
来源：http://hz.hongshengwenyu.top/gtrpwnfwak.html

[S49] C++：写文件
来源：http://hz.aizwys.cn/gthsbyhaoc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jiagoushi.top/gtedkyplnf.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtjebucnyv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hammf.cn/gtnsklqpve.html

[S51] C++：显式类型转换
来源：http://hz.cashguo.top/gtuijvchho.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtmcbfwbih.html

[S52] C++：const 与 noexcept
来源：http://hz.hysaishi.cn/gtosayfoqi.html

int size() const noexcept { return n_; }
来源：http://hz.ydjk.org.cn/gtyhignfds.html

[S53] C++：移动语义
来源：http://hz.chenzaomai.com/gtiwvrxogm.html

std::vector<int> w = std::move(v);
来源：http://hz.guannengcc.top/gtuoibhlxc.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gtxptsqoql.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gtrofywxft.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtdfbiempf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cashguo.top/gtxnpeaqqo.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtdewybdtg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtjsemmenp.html

[S57] C++：编译期常量
来源：http://hz.gaohongyu789.top/gthagwamkq.html

constexpr int N = 10;
来源：http://hz.cqqwz.cn/gtcklxxezv.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtganlkmad.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuxming.cn/gtastdsybj.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtljvephoi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gteoajzmrz.html

[S60] C++：遍历并删除元素
来源：http://hz.ybcxt.top/gtlmcjmhwi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.iojbl.cn/gtfryeotqv.html

================================================================================
来源：http://hz.jianghu66.top/gtghigoexg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtbkllepeb.html

================================================================================
来源：http://hz.yj20258.top/gtwdbniucr.html

[T01] Kotlin：Hello World
来源：http://hz.yueranfly.top/gtimvhsgmh.html

println("Hello")
来源：http://hz.vqdsnc.cn/gtdxkndfnx.html

[T02] Kotlin：变量
来源：http://hz.haohaochexian.top/gtqibrdgjs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cashguo.top/gtmounxfiv.html

[T03] Kotlin：字符串模板
来源：http://hz.chenjidiqi.icu/gtufvyiecy.html

"值: $b"
来源：http://hz.gogol.net.cn/gthdkzhvzq.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtxjrakrhf.html

val n: String? = null;  n?.length
来源：http://hz.9152youxi.cn/gtumodgyhv.html

[T05] Kotlin：when 表达式
来源：http://hz.kuanghao11.cn/gtpfnwszbj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.tanke756.top/gtmtslrbvp.html

[T06] Kotlin：集合映射
来源：http://hz.xuanzx.com/gtoaocqrcq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtetcohyoj.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtrbwiwcga.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jianghu66.top/gtsozgiebk.html

[T08] Kotlin：数据类
来源：http://hz.jqgufenzy.top/gtfrbxbvop.html

data class User(val name: String, val age: Int)
来源：http://hz.aizwys.cn/gtdupevgid.html

[T09] Kotlin：扩展函数
来源：http://hz.sufxvd.cn/gtkylacmoq.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtbalyiwgr.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtiictdtho.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj202588.top/gtcuuiivdr.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtegjdbtgs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xingfuxueyuan.xyz/gtwvqffohr.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtaahxbptb.html

val (a, b) = Pair(1, 2)
来源：http://hz.tian-w.cn/gttpptmbbd.html

[T13] Kotlin：只读 Map
来源：http://hz.zhiwuduotai.top/gtectqbnsd.html

val m = mapOf("a" to 1)
来源：http://hz.ydjk.org.cn/gtrlrxanev.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtkmqitfsz.html

for (i in 1..10) println(i)
来源：http://hz.sweek.top/gtbmpisdgz.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangkeji.top/gtbqgzxkuc.html

interface Shape { fun area(): Double }
来源：http://hz.zhengqikj.top/gttmyiojjy.html

[T16] Swift：Hello World
来源：http://hz.shangyingyoupin.top/gtenervgwp.html

print("Hello")
来源：http://hz.snrcjt.cn/gtklavsfhq.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtutbmenwc.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtafgtuhwb.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtrzzxczco.html

"值: \(b)"
来源：http://hz.tanke756.top/gtlahmeyjt.html

[T19] Swift：可选绑定
来源：http://hz.birdmap.top/gtpjkliohe.html

if let n = opt { print(n) }
来源：http://hz.hysaishi.cn/gtcdikahxs.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtyevyqzqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtysdzobkj.html

[T21] Swift：遍历
来源：http://hz.nanxuanxn.top/gthlfzkjgc.html

for x in a { print(x) }
来源：http://hz.0kj1m.cn/gtmbyxerjf.html

[T22] Swift：字典
来源：http://hz.iojbl.cn/gtwssfmxpe.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangkeji.top/gtvvprvsqb.html

[T23] Swift：函数
来源：http://hz.shanyushiyangtech.top/gtmqbshqnq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.bjfxy.top/gtbksidtvr.html

[T24] Swift：闭包
来源：http://hz.hfpthk.cn/gtcbjjqfzl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.snrcjt.cn/gtwyryrgxs.html

[T25] Swift：结构体
来源：http://hz.xingfuxueyuan.xyz/gtlmymdbif.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtvyqfzeft.html

[T26] Swift：类与重写
来源：http://hz.yonumen.top/gtnoyjmwns.html

class A: Base { override func f() {} }
来源：http://hz.yonumen.top/gtfxtfospe.html

[T27] Swift：错误处理
来源：http://hz.chenzaomai.com/gtufeezxyf.html

do { try f() } catch { print(error) }
来源：http://hz.bjfxy.top/gttkilgznk.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gttgrizpiz.html

enum Color { case red, green }
来源：http://hz.zycfv.cn/gtyglmnvia.html

[T29] Swift：guard 提前返回
来源：http://hz.daxiang520.top/gtltqupkil.html

guard let x = opt else { return }
来源：http://hz.yuxming.cn/gtwaqfvhcx.html

[T30] Swift：协议
来源：http://hz.sufxvd.cn/gtrlzedqtv.html

protocol Shape { func area() -> Double }
来源：http://hz.sysykeji.top/gtnofynspy.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtqqocuxgn.html

print("Hello")
来源：http://hz.fzhhl.top/gtfqhflhur.html

[T32] Lua：局部变量
来源：http://hz.sweek.top/gtytwunjoc.html

local a = 1
来源：http://hz.sweek.top/gtpvhxkdvz.html

[T33] Lua：表（数组）
来源：http://hz.zhongyouzk.top/gttabdwgtb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hammf.cn/gtoddxhnvs.html

[T34] Lua：遍历表
来源：http://hz.svipenyu.cn/gtkvzdvwtm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tian-w.cn/gtzzvmrfxg.html

[T35] Lua：字典表
来源：http://hz.cashguo.top/gtxgromnut.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jlsjyb.cn/gtyhbyswgm.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtuxhhyfzl.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtscauipld.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtwdxtugzv.html

"a" .. "b"
来源：http://hz.havefunace.top/gtouxjmxvh.html

[T38] Lua：条件
来源：http://hz.jinqigfzy.top/gtzhrlrutp.html

if x > 0 then print("正") end
来源：http://hz.birdmap.top/gtggpscvrf.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtnxnnvdgj.html

string.find(s, "%d+")
来源：http://hz.cheryme.top/gtfrzdqgyw.html

[T40] Lua：元表
来源：http://hz.dianchejie.cn/gtnsptqxvp.html

setmetatable({}, { __index = base })
来源：http://hz.c1oappe.top/gtshuaentc.html

[T41] Perl：Hello World
来源：http://hz.yj20258.top/gteoxmrvcs.html

print "Hello\n";
来源：http://hz.ydjk.org.cn/gtedgrbfam.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtbjvjswlu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtjkogliss.html

[T43] Perl：字符串插值
来源：http://hz.dashuyun.cn/gtoenupaqs.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtmnavwque.html

[T44] Perl：条件
来源：http://hz.mhx1999.top/gtsrvjhqph.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gtgjwcjdzh.html

[T45] Perl：数组遍历
来源：http://hz.ivvv.top/gtapxzgegs.html

for my $x (@arr) { print $x; }
来源：http://hz.gogol.net.cn/gtycwoucjs.html

[T46] Perl：哈希操作
来源：http://hz.yj20258888.top/gturakasdu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ppjwa.cn/gtmvkvjmji.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtmirmwfri.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.wangshuangyany.cn/gtaqtdhgqv.html

[T48] Perl：正则替换
来源：http://hz.jyoumei.cn/gtzwpiinms.html

$s =~ s/old/new/g;
来源：http://hz.chenzaomai.com/gtssnaxyqm.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtbqrvukai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jinqigufen.top/gtbfpeymap.html

[T50] Perl：逐行读文件
来源：http://hz.aibaodan.cn/gtxmioewlk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gaohongyu789.top/gtogheuado.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinghuilouyu.cn/gtgoeikuov.html

[T51] Scala：Hello World
来源：http://hz.316326.xyz/gtnqcimchx.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtmmkbbqzc.html

[T52] Scala：变量
来源：http://hz.zhengqikj.top/gtaqtearsq.html

val a = 1;  var b = 2
来源：http://hz.yangfankeji.com/gthkumsyue.html

[T53] Scala：字符串插值
来源：http://hz.pycfn.com/gtscogavtj.html

s"值: $b"
来源：http://hz.guannengcc.top/gtajmkkbyc.html

[T54] Scala：集合映射
来源：http://hz.hongshengwenyu.top/gtkqhgczhd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.pycfn.com/gtzsslgnbl.html

[T55] Scala：集合过滤
来源：http://hz.gaohongyu789.top/gtakkvxbzq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cashguo.top/gtmevaqiiy.html

[T56] Scala：样例类
来源：http://hz.aibaodan.cn/gtouhctlgp.html

case class User(name: String, age: Int)
来源：http://hz.jyoumei.cn/gtoknzudem.html

[T57] Scala：模式匹配
来源：http://hz.daxiang520.top/gtvtzbsslr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tanke756.top/gtiveezmrm.html

[T58] Scala：函数定义
来源：http://hz.xuetiantiany.cn/gtdvozfvls.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.52xcode.cn/gtsgrbfzkh.html

[T59] Scala：循环
来源：http://hz.gogol.net.cn/gtsdbejyqn.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtopflwvfb.html

[T60] Scala：折叠
来源：http://hz.chenlongwang.top/gttannveso.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gtjprbsvlh.html

================================================================================
来源：http://hz.hnqzz.top/gtwcwewfsl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.52xcode.cn/gtehuycdsb.html

================================================================================
来源：http://hz.andypj.xyz/gtoxptdrjm.html

[U01] Py：创建虚拟环境
来源：http://hz.gogol.net.cn/gtnvpvshlt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jiagoushi.top/gtwsggixqb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yongpay.top/gtsawhhqpp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yj20258888.top/gtmqhbrsyq.html

[U03] Py：加载 .env 配置
来源：http://hz.chenzaomai.com/gttvyinxqs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.havefunace.top/gtuukuenxc.html

[U04] Py：变量调试打印
来源：http://hz.zhaomingkeji.xyz/gtklefnuif.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgfzy.top/gtvwosxhvg.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtxlektuuh.html

list(dict.fromkeys(arr))
来源：http://hz.jyoumei.cn/gtauctbexb.html

[U06] Py：合并两个字典
来源：http://hz.jyoumei.cn/gtommfalfs.html

{**a, **b}
来源：http://hz.wangdashe.top/gtlgsqoojg.html

[U07] Py：反转字典键值
来源：http://hz.sweek.top/gtjnvwvayh.html

{v: k for k, v in d.items()}
来源：http://hz.quarkkingdee.top/gtfpcyhfrx.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtsdayexxd.html

[y for x in nested for y in x]
来源：http://hz.316326.xyz/gtnuukepvi.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258888.top/gtxmfrjrqt.html

max(d, key=d.get)
来源：http://hz.jianghu66.top/gtgyjklmxt.html

[U10] Py：按值排序字典
来源：http://hz.cdnleiting.top/gtjunejpkf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hammf.cn/gtqvveewyf.html

[U11] Py：生成器表达式
来源：http://hz.jianghu66.top/gtgdxeudgz.html

(x * 2 for x in arr)
来源：http://hz.0kj1m.cn/gtnlabxmtr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sufxvd.cn/gtmjpsstvt.html

Counter(arr).most_common(3)
来源：http://hz.ybcxt.top/gtwexxmgkl.html

[U13] Py：固定长度队列
来源：http://hz.yj202588.top/gthuhevpdx.html

deque(maxlen=10)
来源：http://hz.zhongyouzk.top/gtadocavfc.html

[U14] Py：分组收集到列表
来源：http://hz.birdmap.top/gtehvrspgs.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gthmgkjbjl.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtmpwdbzvf.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtyexgszlz.html

[U16] Py：命令行参数解析
来源：http://hz.jinqigfzy.top/gtrqvhdjrm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tian-w.cn/gtftnikogx.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangkeji.top/gteohorsxi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hywenlv.cn/gtrjfwsqiu.html

[U18] Py：预编译正则
来源：http://hz.zdqjudy.top/gthsmmkjtp.html

pat = re.compile(r"\d+")
来源：http://hz.shangyingyoupin.top/gtkmfapmym.html

[U19] Py：正则替换带回调
来源：http://hz.zhengqikj.top/gtshwptwpv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shanyushiyangkeji.top/gtlrompbvs.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangkeji.top/gtusfwnfqi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gthhdtkzzg.html

[U21] Py：自定义上下文管理器
来源：http://hz.yongpay.top/gtgzujteqd.html

@contextlib.contextmanager
来源：http://hz.ydzc1.top/gtjfumtcex.html

[U22] Py：矩阵转置
来源：http://hz.nanxinkj.top/gtgqtwqcrf.html

list(zip(*m))
来源：http://hz.chenzaomai.com/gtristscfk.html

[U23] Py：分块读取大文件
来源：http://hz.tanke756.top/gthenvexqv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xylfe.cn/gtzsdnbmlh.html

[U24] Py：路径操作
来源：http://hz.yuxming.cn/gthcyfiuix.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.bjfxy.top/gtltxeliey.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258.top/gtdgpwaupl.html

csv.DictReader(f)
来源：http://hz.jqgufenzy.top/gtfouhsraw.html

[U26] Py：并发下载
来源：http://hz.havefunace.top/gtrstqrdmc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.tanke756.top/gtoyjadebt.html

[U27] Py：异步 HTTP
来源：http://hz.hfpthk.cn/gtgdzqcxwi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tianlin.xyz/gtsavoiryt.html

[U28] Py：类型别名
来源：http://hz.cheryme.top/gtwbdntqqb.html

UserId = int
来源：http://hz.vqdsnc.cn/gtoaduqekh.html

[U29] Py：属性校验
来源：http://hz.tianlin.xyz/gtzwgmfhyk.html

@property 与 @x.setter 配合
来源：http://hz.zhijiandao.cn/gtinzrhcdm.html

[U30] Py：数据类
来源：http://hz.ydjk.org.cn/gtywhfdkxq.html

@dataclass(slots=True)
来源：http://hz.mhx1999.top/gtzuzdhzgx.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtszsmohgr.html

python -m pytest -q
来源：http://hz.shanyushiyangtech.top/gtksfzulpn.html

[U32] Py：代码格式化
来源：http://hz.hnxiangtu.top/gtwwcblmja.html

ruff format . && ruff check --fix .
来源：http://hz.sufxvd.cn/gtcupbtulq.html

[U33] Py：打包发布
来源：http://hz.nwbrower.top/gtjntddqwp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.quarkkingdee.top/gtvnmdhxfw.html

[U34] Py：判断编码
来源：http://hz.yuanzhike.top/gtwrozfjiu.html

chardet.detect(raw)
来源：http://hz.andypj.xyz/gtubjhorqq.html

[U35] Py：发送邮件
来源：http://hz.yuxming.cn/gtpwayokbr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuanzhike.top/gtikymelgv.html

[U36] Py：定时任务
来源：http://hz.gogol.net.cn/gtzlmjfwrg.html

schedule.every(10).minutes.do(job)
来源：http://hz.shanyushiyangtech.top/gtwppkqbur.html

[U37] Py：读写 Excel
来源：http://hz.chenzaomai.com/gtabroctgb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258888.top/gtghfwjpdh.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenlongwang.top/gtccswttzh.html

Path(__file__).resolve().parent
来源：http://hz.aibaodan.cn/gtlovjcqea.html

[U39] Py：判断是否在交互环境
来源：http://hz.havefunace.top/gtlqfmkqox.html

sys.stdout.isatty()
来源：http://hz.hnxiangtu.top/gtzvyndcli.html

[U40] Py：打印到标准错误
来源：http://hz.c1oappe.top/gtaystiyjp.html

print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtqhecbuor.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yvedp.cn/gtabuegfza.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sufxvd.cn/gtbnjyqtkk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hywenlv.cn/gtfadumvmg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhiwuduotai.top/gtxdulbbox.html

[U43] PHP：声明命名空间
来源：http://hz.birdmap.top/gttwgjcrqf.html

namespace App\Http;
来源：http://hz.fengsongda.top/gtinvrpljd.html

[U44] PHP：开启严格类型
来源：http://hz.gzhubu.top/gtuacrrzvm.html

declare(strict_types=1);
来源：http://hz.jiagoushi.top/gtsovfyoeh.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtgancaisq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gthpjvmzlk.html

[U46] PHP：可空类型
来源：http://hz.vqdsnc.cn/gtiipticvb.html

?string $name = null
来源：http://hz.xuanzx.com/gtvwgmhwzr.html

[U47] PHP：联合类型
来源：http://hz.zhijiandao.cn/gtwjaostwx.html

int|string $id
来源：http://hz.kuanghao11.cn/gtkhkuobgi.html

[U48] PHP：纯枚举
来源：http://hz.nanxuanxn.top/gtxdxhfhtx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hnxiangtu.top/gtjarzpdue.html

[U49] PHP：只读属性
来源：http://hz.pengpengdd.cyou/gtpkuqiqps.html

public readonly string $name
来源：http://hz.xylfe.cn/gtuiarszyn.html

[U50] PHP：构造器属性提升
来源：http://hz.cqqwz.cn/gtgpjwoyoc.html

public function __construct(private int $id) {}
来源：http://hz.guannengcc.top/gtnalrfesy.html

[U51] PHP：数组解构
来源：http://hz.svipenyu.cn/gtupmjvxfz.html

[$a, $b] = $arr;
来源：http://hz.gotoacloud.top/gttomlrhbj.html

[U52] PHP：箭头函数
来源：http://hz.wangshuangyany.cn/gtsxxktjyj.html

$double = fn($x) => $x * 2;
来源：http://hz.yuanzhike.top/gtienucnwj.html

[U53] PHP：空合并运算符
来源：http://hz.ydjk.org.cn/gtwocdtzyf.html

$v = $a ?? $b ?? "default";
来源：http://hz.9152youxi.cn/gtslaprihl.html

[U54] PHP：空安全调用
来源：http://hz.316326.xyz/gtpsmjhslg.html

$obj?->method()
来源：http://hz.xuetiantiany.cn/gtzomrlnze.html

[U55] PHP：match 表达式
来源：http://hz.c1oappe.top/gtzwqpxsqq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aizwys.cn/gthnxdcibp.html

[U56] PHP：命名参数
来源：http://hz.shuidangran.top/gthoqlmeqq.html

f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gttcxqvfsv.html

[U57] PHP：字符串插值
来源：http://hz.feifeiyinyue.top/gtzaxqkolh.html

"值: {$a}"
来源：http://hz.sxryk.cn/gtnkyxelxx.html

[U58] PHP：数组三件套
来源：http://hz.birdmap.top/gtpegqzjiw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinghuilouyu.cn/gtbxwlezsl.html

[U59] PHP：自定义排序
来源：http://hz.zhongyouzk.top/gtidjnrbry.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtuzkhryqu.html

[U60] PHP：JSON 编解码
来源：http://hz.hnqzz.top/gtqstskzga.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.wangshuangyany.cn/gtdikfzyhp.html

[U61] PHP：正则
来源：http://hz.yueranfly.top/gtyllrhtlg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtwwazjetu.html

[U62] PHP：日期对象
来源：http://hz.yangfankeji.com/gtprazzopy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ydzc1.top/gtdcvawgmp.html

[U63] PHP：文件读写
来源：http://hz.zycfv.cn/gtvijnaiag.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gzhubu.top/gtrxayejul.html

[U64] PHP：目录遍历
来源：http://hz.xingfuxueyuan.xyz/gtoadwxfjq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tian-w.cn/gthlujnfjz.html

[U65] PHP：会话
来源：http://hz.redwolf501.top/gtgwryyaxw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jlsjyb.cn/gtryhsfqfo.html

[U66] PHP：设置 Cookie
来源：http://hz.sxryk.cn/gtoavdbowp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jinqigufen.top/gttrklahnu.html

[U67] PHP：处理文件上传
来源：http://hz.jyoumei.cn/gtilmvcrlo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhongyouzk.top/gtceavthil.html

[U68] PHP：PDO 连接
来源：http://hz.hnxiangtu.top/gtbhmygqjh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nanxuanxn.top/gtvaalcodg.html


<!-- 参考信息 -->