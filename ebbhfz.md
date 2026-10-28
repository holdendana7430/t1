代发 wailian999

[S45] C++：lambda
来源：http://hz.ppjwa.cn/gtdwxgucwz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydzc1.top/gteikeaadg.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gtnadchdvl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinyuanbaomall.cn/gtwxonwtxq.html

[S47] C++：结构化绑定遍历
来源：http://hz.vqdsnc.cn/gtffcgtexb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtbixywxyx.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtdjajdsct.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.vqdsnc.cn/gtpptkaork.html

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gtezlztchp.html

[S49] C++：写文件
来源：http://hz.vqdsnc.cn/gtvzkegisv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtodrfzvou.html

[S50] C++：格式化数字
来源：http://hz.daxiang520.top/gtjasprepo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gtmgyqssbk.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gtfsnmilyf.html

static_cast<double>(a) / b
来源：http://hz.jyoumei.cn/gtrhyeqtrm.html

[S52] C++：const 与 noexcept
来源：http://hz.zycfv.cn/gtfqxnpnnz.html

int size() const noexcept { return n_; }
来源：http://hz.xuanzx.com/gtnhmcxqlt.html

[S53] C++：移动语义
来源：http://hz.nanxuanxn.top/gtgcazfffs.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtiiasgqxg.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtihkysiti.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shangyingyoupin.top/gteqpkkyur.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtpztpclda.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtweqqapvw.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gticjyxzkz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtpzjdxyos.html

[S57] C++：编译期常量
来源：http://hz.quarkkingdee.top/gtkcafqpek.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtpmsmoexn.html

[S58] C++：命名空间
来源：http://hz.bjfxy.top/gtpfncqgrk.html

namespace ns { int f() { return 1; } }
来源：http://hz.ehwqpu.com/gtzkeoiezg.html

[S59] C++：静态断言
来源：http://hz.gaohongyu789.top/gtoxmaddeo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sxryk.cn/gtzylqrccv.html

[S60] C++：遍历并删除元素
来源：http://hz.zhongyouzk.top/gtebfbpbmq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtkczxglhw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtywixbohu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenlongwang.top/gtwiivfsxu.html

================================================================================
来源：http://hz.nwbrower.top/gteswxrjze.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtnenzppnd.html

println("Hello")
来源：http://hz.smart0.xyz/gtyidgdftz.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gthxxobjrz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yonumen.top/gtmbsuihlx.html

[T03] Kotlin：字符串模板
来源：http://hz.nanxuanxn.top/gtswhvxtpj.html

"值: $b"
来源：http://hz.zhixingplan.top/gtyxgceraf.html

[T04] Kotlin：空安全
来源：http://hz.yj202588.top/gtqeopvogd.html

val n: String? = null;  n?.length
来源：http://hz.smart0.xyz/gttrkjyyux.html

[T05] Kotlin：when 表达式
来源：http://hz.tianlin.xyz/gtdfgjiyzu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cqqwz.cn/gtirjoerib.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtgoglpoxe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gteucyuxsl.html

[T07] Kotlin：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtjjgrbuyf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtutnkbcfz.html

[T08] Kotlin：数据类
来源：http://hz.jiagoushi.top/gtymbhsfgb.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtnjkvtjor.html

[T09] Kotlin：扩展函数
来源：http://hz.hysaishi.cn/gtylubqwee.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gtoiwuarmo.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtrnpyruil.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hywenlv.cn/gtrohvrkdc.html

[T11] Kotlin：协程
来源：http://hz.xziqi.cn/gtwhsaathr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ehwqpu.com/gtjuehyanf.html

[T12] Kotlin：解构声明
来源：http://hz.ppjwa.cn/gttuwieqmn.html

val (a, b) = Pair(1, 2)
来源：http://hz.tianlin.xyz/gtdtksqqrw.html

[T13] Kotlin：只读 Map
来源：http://hz.zhongyouzk.top/gtxpvbqnfb.html

val m = mapOf("a" to 1)
来源：http://hz.ivvv.top/gtkjlsbfyh.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtnslnwuzh.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gthbovfyay.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gtwxczivvn.html

interface Shape { fun area(): Double }
来源：http://hz.shzxlz.cn/gtyuvealuc.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtqqyipouk.html

print("Hello")
来源：http://hz.shzxlz.cn/gtepjnspqs.html

[T17] Swift：变量与常量
来源：http://hz.tianlin.xyz/gtrufuityx.html

var a = 1;  let b = 2
来源：http://hz.dashuyun.cn/gtgnihrxxp.html

[T18] Swift：字符串插值
来源：http://hz.c1oappe.top/gtnjdniyrl.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtpjsniefi.html

[T19] Swift：可选绑定
来源：http://hz.zdqjudy.top/gtxcqpbgee.html

if let n = opt { print(n) }
来源：http://hz.fzhhl.top/gtyxmrikjl.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtoqhgusqm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtqwyosksx.html

[T21] Swift：遍历
来源：http://hz.xuetiantiany.cn/gtcvspkhvt.html

for x in a { print(x) }
来源：http://hz.jianghu66.top/gtstrqieqr.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtiohregfo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtjjfekisp.html

[T23] Swift：函数
来源：http://hz.sxryk.cn/gthcadjpds.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtfdvaxqro.html

[T24] Swift：闭包
来源：http://hz.iojbl.cn/gtfbcaabtb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nanxinkj.top/gtvyvhrsof.html

[T25] Swift：结构体
来源：http://hz.tian-w.cn/gtptizxtpd.html

struct P { var x: Int }
来源：http://hz.daria6918.cn/gtdcpnjsmi.html

[T26] Swift：类与重写
来源：http://hz.cashguo.top/gttssfnmgp.html

class A: Base { override func f() {} }
来源：http://hz.ppjwa.cn/gtivrbeskw.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtlnaivbpv.html

do { try f() } catch { print(error) }
来源：http://hz.cdnleiting.top/gtogdgawfv.html

[T28] Swift：枚举
来源：http://hz.guannengcc.top/gtkypkasyu.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtsdlzgjbw.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtjqseweqo.html

guard let x = opt else { return }
来源：http://hz.daria6918.cn/gtnlbmnvye.html

[T30] Swift：协议
来源：http://hz.bjfxy.top/gtcwyuaala.html

protocol Shape { func area() -> Double }
来源：http://hz.ywan-chungtsiang.top/gtapbijkrf.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtifnegqwx.html

print("Hello")
来源：http://hz.snrcjt.cn/gtggsgcybb.html

[T32] Lua：局部变量
来源：http://hz.gzhubu.top/gtsexjusgx.html

local a = 1
来源：http://hz.xuetiantiany.cn/gtzxportlz.html

[T33] Lua：表（数组）
来源：http://hz.ppjwa.cn/gtneivbmwd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtpvbxiecj.html

[T34] Lua：遍历表
来源：http://hz.jinyuanbaomall.cn/gttsgubymb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sweek.top/gtephbvjfn.html

[T35] Lua：字典表
来源：http://hz.vqdsnc.cn/gtpgsoeixy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtxbnvnbhd.html

[T36] Lua：函数
来源：http://hz.yj20258888.top/gtyibujozi.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtnuwyhstl.html

[T37] Lua：字符串拼接
来源：http://hz.havefunace.top/gtdednnyyi.html

"a" .. "b"
来源：http://hz.meibo888.top/gtlpjechsn.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtrwpukjgn.html

if x > 0 then print("正") end
来源：http://hz.sweek.top/gtjeoqznqk.html

[T39] Lua：模式匹配
来源：http://hz.yj20258888.top/gtfxganhoe.html

string.find(s, "%d+")
来源：http://hz.jyoumei.cn/gtursvcqwh.html

[T40] Lua：元表
来源：http://hz.jinqigufen.top/gtzlpkwwjl.html

setmetatable({}, { __index = base })
来源：http://hz.hysaishi.cn/gtqprgofof.html

[T41] Perl：Hello World
来源：http://hz.ppjwa.cn/gtqmkfxrea.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gtwbkttjqq.html

[T42] Perl：变量类型
来源：http://hz.zhengqikj.top/gtmiqruyva.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.pengpengdd.cyou/gtkbzqyclm.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtphimrxge.html

"值: $a"
来源：http://hz.svipenyu.cn/gtbhuleplh.html

[T44] Perl：条件
来源：http://hz.sxryk.cn/gticoagbzy.html

if ($a > 0) { print "正"; }
来源：http://hz.c1oappe.top/gtpkjaszle.html

[T45] Perl：数组遍历
来源：http://hz.pengpengdd.cyou/gtwdqdxrtz.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtfiqqvzqe.html

[T46] Perl：哈希操作
来源：http://hz.cashguo.top/gtfixdrpyc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtnveoqhdp.html

[T47] Perl：正则捕获
来源：http://hz.yj202588.top/gthqjyqtnv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cucudq.cn/gtnxgzojhd.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtxlfgshmb.html

$s =~ s/old/new/g;
来源：http://hz.sxryk.cn/gtpobylpai.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtfjrjwxmh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jlsjyb.cn/gthmtvoieu.html

[T50] Perl：逐行读文件
来源：http://hz.cashguo.top/gtbsjjbqzg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tanke756.top/gtgkwlvkdt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.wangshuangyany.cn/gtgehvvkax.html

[T51] Scala：Hello World
来源：http://hz.yvedp.cn/gteqeepinp.html

println("Hello")
来源：http://hz.yvedp.cn/gtdeyjivwd.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtvazmubcz.html

val a = 1;  var b = 2
来源：http://hz.fengsongda.top/gtvsmejfjb.html

[T53] Scala：字符串插值
来源：http://hz.cashguo.top/gtotlnsxtu.html

s"值: $b"
来源：http://hz.fzhhl.top/gtlytmjhda.html

[T54] Scala：集合映射
来源：http://hz.yongpay.top/gtxdhfqjph.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.haohaochexian.top/gtuavfrnzl.html

[T55] Scala：集合过滤
来源：http://hz.316326.xyz/gtsvxkfdmq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yvedp.cn/gtbedynkiv.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtzabuusov.html

case class User(name: String, age: Int)
来源：http://hz.mhx1999.top/gtntdkmrng.html

[T57] Scala：模式匹配
来源：http://hz.nanxinkj.top/gtruuqmqmh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.quarkkingdee.top/gtdywiaqqc.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gtbrzsvnkv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zycfv.cn/gtnnrdjdcm.html

[T59] Scala：循环
来源：http://hz.jinyuanbaomall.cn/gtivohcave.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtifrznymf.html

[T60] Scala：折叠
来源：http://hz.cheryme.top/gttuediywu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtzurlwjlt.html

================================================================================
来源：http://hz.pycfn.com/gtdbedgwda.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dashuyun.cn/gtwerprevm.html

================================================================================
来源：http://hz.sufxvd.cn/gtfeoxnrtk.html

[U01] Py：创建虚拟环境
来源：http://hz.gaohongyu789.top/gtqwdkkqnn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jlsjyb.cn/gtfweigymw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.0kj1m.cn/gthflbxrcl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.smart0.xyz/gtsartwxzu.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtunxplrji.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.gotoacloud.top/gtgnxtbsfo.html

[U04] Py：变量调试打印
来源：http://hz.yonumen.top/gtdcgcbkpq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtdrbyfztz.html

[U05] Py：列表去重且保序
来源：http://hz.hongshengwenyu.top/gtxratjqkp.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gttibbsttm.html

[U06] Py：合并两个字典
来源：http://hz.shzxlz.cn/gttxjqyzst.html

{**a, **b}
来源：http://hz.jinghuilouyu.cn/gttgkvofqs.html

[U07] Py：反转字典键值
来源：http://hz.jinqigfzy.top/gtyjingugb.html

{v: k for k, v in d.items()}
来源：http://hz.hfpthk.cn/gtyzolozzx.html

[U08] Py：展平二维列表
来源：http://hz.kuanghao11.cn/gtqrrlsbrt.html

[y for x in nested for y in x]
来源：http://hz.sufxvd.cn/gtnnpszyqk.html

[U09] Py：字典取最大值的键
来源：http://hz.xziqi.cn/gtommrfkaf.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtqoyudbbd.html

[U10] Py：按值排序字典
来源：http://hz.shuidangran.top/gtztagqnop.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ybcxt.top/gttkziiiui.html

[U11] Py：生成器表达式
来源：http://hz.hnqzz.top/gtzxjvsmzh.html

(x * 2 for x in arr)
来源：http://hz.hnqzz.top/gtfdhwftyc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daria6918.cn/gtncjqxthv.html

Counter(arr).most_common(3)
来源：http://hz.iojbl.cn/gtdsniqtew.html

[U13] Py：固定长度队列
来源：http://hz.sxryk.cn/gtgcemvddg.html

deque(maxlen=10)
来源：http://hz.kuanghao11.cn/gtbvqqnvlg.html

[U14] Py：分组收集到列表
来源：http://hz.cheryme.top/gtdvwvfwfl.html

defaultdict(list)
来源：http://hz.xingfuxueyuan.xyz/gtmnsztcke.html

[U15] Py：高精度计时
来源：http://hz.zhiwuduotai.top/gtrkfeqbmi.html

t = time.perf_counter()
来源：http://hz.guowangkeji.top/gtxbfevtdb.html

[U16] Py：命令行参数解析
来源：http://hz.cdnleiting.top/gtbqdqxjyi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gaohongyu789.top/gtxlsqbxxq.html

[U17] Py：初始化日志
来源：http://hz.jinyuanbaomall.cn/gtvafljafz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenlongwang.top/gtvjgqgzdb.html

[U18] Py：预编译正则
来源：http://hz.cucudq.cn/gtvksyyvpa.html

pat = re.compile(r"\d+")
来源：http://hz.sysykeji.top/gtjqusabrx.html

[U19] Py：正则替换带回调
来源：http://hz.jqgufenzy.top/gtymjxrlfj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtypvbcuuc.html

[U20] Py：缓存函数结果
来源：http://hz.bjfxy.top/gtokiyyjvd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sysykeji.top/gtmuqbvhjh.html

[U21] Py：自定义上下文管理器
来源：http://hz.gogol.net.cn/gtptnjslid.html

@contextlib.contextmanager
来源：http://hz.pengpengdd.cyou/gtftlwuujb.html

[U22] Py：矩阵转置
来源：http://hz.cashguo.top/gtyatbqrwp.html

list(zip(*m))
来源：http://hz.cqqwz.cn/gtyntjlhuk.html

[U23] Py：分块读取大文件
来源：http://hz.nwbrower.top/gtvwvkpkpv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtkniaqdpf.html

[U24] Py：路径操作
来源：http://hz.guannengcc.top/gtgcmfrinr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtlhqryfew.html

[U25] Py：CSV 按字典读
来源：http://hz.yuanzhike.top/gtuutnmhsi.html

csv.DictReader(f)
来源：http://hz.jinqigufen.top/gtbokjkdru.html

[U26] Py：并发下载
来源：http://hz.xziqi.cn/gtohqwmwqb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hammf.cn/gtkdqpijxy.html

[U27] Py：异步 HTTP
来源：http://hz.chenlongwang.top/gtjtwhzxdt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtvyjyjpvn.html

[U28] Py：类型别名
来源：http://hz.nanxinkj.top/gtcssmryvz.html

UserId = int
来源：http://hz.yonumen.top/gtbsjkudgt.html

[U29] Py：属性校验
来源：http://hz.ywan-chungtsiang.top/gtanqcjhre.html

@property 与 @x.setter 配合
来源：http://hz.chenzaomai.com/gtgdxbgigc.html

[U30] Py：数据类
来源：http://hz.jinqigfzy.top/gtshopwfjm.html

@dataclass(slots=True)
来源：http://hz.quarkkingdee.top/gtfuoyedqc.html

[U31] Py：单测
来源：http://hz.vqdsnc.cn/gtgmwpwkzl.html

python -m pytest -q
来源：http://hz.chenzaomai.com/gtuxkvmuyo.html

[U32] Py：代码格式化
来源：http://hz.kuanghao11.cn/gtqpkytssy.html

ruff format . && ruff check --fix .
来源：http://hz.havefunace.top/gtgjreruva.html

[U33] Py：打包发布
来源：http://hz.zhiwuduotai.top/gtcdrjnkwr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhengqikj.top/gtoclxneiq.html

[U34] Py：判断编码
来源：http://hz.ppjwa.cn/gtqeedkwip.html

chardet.detect(raw)
来源：http://hz.jinghuilouyu.cn/gtknzeygdm.html

[U35] Py：发送邮件
来源：http://hz.zhoulong.xyz/gtlzefmkza.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.havefunace.top/gtsajjhufm.html

[U36] Py：定时任务
来源：http://hz.hysaishi.cn/gtskzxocdg.html

schedule.every(10).minutes.do(job)
来源：http://hz.316326.xyz/gtvguedxbd.html

[U37] Py：读写 Excel
来源：http://hz.mhx1999.top/gtmrvmewnb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.kuanghao11.cn/gttqibtipe.html

[U38] Py：获取脚本所在目录
来源：http://hz.zdqjudy.top/gtpjjvrqle.html

Path(__file__).resolve().parent
来源：http://hz.zhaomingkeji.xyz/gtzjaypdxg.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhaomingkeji.xyz/gtfiwgrbmm.html

sys.stdout.isatty()
来源：http://hz.gogol.net.cn/gthoqcntfq.html

[U40] Py：打印到标准错误
来源：http://hz.9152youxi.cn/gtubveaybt.html

print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtyagovrcq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cqqwz.cn/gthqoftvix.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hammf.cn/gtaagtcydo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.52xcode.cn/gtsacovjoc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinghuilouyu.cn/gthwedeojc.html

[U43] PHP：声明命名空间
来源：http://hz.cashguo.top/gtjxulhndz.html

namespace App\Http;
来源：http://hz.zdqjudy.top/gtaspihnay.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258888.top/gturkzjpwe.html

declare(strict_types=1);
来源：http://hz.xinyue.icu/gtpgfuobnd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.aizwys.cn/gtsqakxiyi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtnwsmufau.html

[U46] PHP：可空类型
来源：http://hz.sysykeji.top/gtnojcvjiu.html

?string $name = null
来源：http://hz.nanxuanxn.top/gtbylnkgzj.html

[U47] PHP：联合类型
来源：http://hz.havefunace.top/gtkpfulyju.html

int|string $id
来源：http://hz.jinyuanbaomall.cn/gtqwthvzjz.html

[U48] PHP：纯枚举
来源：http://hz.yuxming.cn/gtksbinhvy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtyapwrata.html

[U49] PHP：只读属性
来源：http://hz.birdmap.top/gtgrjaahtc.html

public readonly string $name
来源：http://hz.yuanzhike.top/gtzpsrqqjw.html

[U50] PHP：构造器属性提升
来源：http://hz.yuanzhike.top/gtircstnqt.html

public function __construct(private int $id) {}
来源：http://hz.chenjidiqi.icu/gtykjwplle.html

[U51] PHP：数组解构
来源：http://hz.aizwys.cn/gtruvqalcc.html

[$a, $b] = $arr;
来源：http://hz.gzhubu.top/gthkvfmgzi.html

[U52] PHP：箭头函数
来源：http://hz.yj20258888.top/gtawipvxxs.html

$double = fn($x) => $x * 2;
来源：http://hz.fzhhl.top/gtnawjtvmg.html

[U53] PHP：空合并运算符
来源：http://hz.nanxuanxn.top/gtiuvslwra.html

$v = $a ?? $b ?? "default";
来源：http://hz.haohaochexian.top/gtjhdqavkh.html

[U54] PHP：空安全调用
来源：http://hz.sufxvd.cn/gtzdeuedyw.html

$obj?->method()
来源：http://hz.daria6918.cn/gtiijhcvnj.html

[U55] PHP：match 表达式
来源：http://hz.xingfuxueyuan.xyz/gtbhmezlyf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.feifeiyinyue.top/gtgkaivtei.html

[U56] PHP：命名参数
来源：http://hz.bjfxy.top/gtzqhoeegu.html

f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtnerjqnjq.html

[U57] PHP：字符串插值
来源：http://hz.yueranfly.top/gttaoibkby.html

"值: {$a}"
来源：http://hz.aibaodan.cn/gtwvuxwjvv.html

[U58] PHP：数组三件套
来源：http://hz.yvedp.cn/gtzhzmfulb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yj202588.top/gthekzlwft.html

[U59] PHP：自定义排序
来源：http://hz.yongpay.top/gtzpkisxgk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhijiandao.cn/gthustjnsd.html

[U60] PHP：JSON 编解码
来源：http://hz.yj202588.top/gtujjxgori.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.birdmap.top/gtyyupzbfk.html

[U61] PHP：正则
来源：http://hz.gogol.net.cn/gttesvvodo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtkgdvxfgd.html

[U62] PHP：日期对象
来源：http://hz.tanke756.top/gtowmuyjwc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.wangshuangyany.cn/gtbpnnuciv.html

[U63] PHP：文件读写
来源：http://hz.zhongyouzk.top/gtwhosogco.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hnqzz.top/gtaeyzsyfh.html

[U64] PHP：目录遍历
来源：http://hz.hnqzz.top/gteacgqfsx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.nwbrower.top/gtogjidmed.html

[U65] PHP：会话
来源：http://hz.gogol.net.cn/gtgxjksygh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenzaomai.com/gtarjlpgwh.html

[U66] PHP：设置 Cookie
来源：http://hz.sweek.top/gtsyuxiukl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ivvv.top/gtsjltjife.html

[U67] PHP：处理文件上传
来源：http://hz.mhx1999.top/gthqsopnbo.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.aizwys.cn/gtciwbgfpd.html

[U68] PHP：PDO 连接
来源：http://hz.nanxinkj.top/gtvknmbzjv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jianghu66.top/gtdtedueqj.html

[U69] PHP：PDO 预处理
来源：http://hz.pycfn.com/gtnbgzphuu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.haohaochexian.top/gtpynglurq.html

[U70] PHP：PDO 事务
来源：http://hz.jianghu66.top/gtbicycyoo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.guannengcc.top/gtlgoqvvsx.html


<!-- 参考信息 -->