代发 wailian999

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtduysiroe.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtvsrmhyug.html

[S44] C++：引用传参
来源：http://hz.yj202588.top/gtomquqbqw.html

void inc(int &x) { ++x; }
来源：http://hz.cheryme.top/gtobjwnucz.html

[S45] C++：lambda
来源：http://hz.nwbrower.top/gtuyzmisdn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtfgnbngph.html

[S46] C++：函数模板
来源：http://hz.jlsjyb.cn/gtdnppbsvr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yonumen.top/gtfrcdlnri.html

[S47] C++：结构化绑定遍历
来源：http://hz.hfpthk.cn/gtzyybpmhs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxuanxn.top/gtghiqfiej.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtvyyiwcjr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xingfuxueyuan.xyz/gtdmyvlmmh.html

while (std::getline(in, line)) { }
来源：http://hz.xziqi.cn/gttgfzpmda.html

[S49] C++：写文件
来源：http://hz.zhixingplan.top/gtomdwyhpx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtwxarsvaj.html

[S50] C++：格式化数字
来源：http://hz.gzhubu.top/gtzanzogtr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cucudq.cn/gtstwclvaz.html

[S51] C++：显式类型转换
来源：http://hz.mhx1999.top/gtvbargslc.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtnmkwnryp.html

[S52] C++：const 与 noexcept
来源：http://hz.xuetiantiany.cn/gtsimsjeeh.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtgpehmksm.html

[S53] C++：移动语义
来源：http://hz.iojbl.cn/gtusepjcii.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtxqupsorc.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtyiwgbthm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtdanlpbrs.html

[S55] C++：结构化绑定
来源：http://hz.yueranfly.top/gtngkchmby.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gtozyjqluh.html

[S56] C++：optional
来源：http://hz.nwbrower.top/gtjqoqoosa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtdzvoeahh.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtixwynouj.html

constexpr int N = 10;
来源：http://hz.jqgfzy.top/gtdxjkfmss.html

[S58] C++：命名空间
来源：http://hz.jinqigfzy.top/gtmczytgur.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhoulong.xyz/gtuftmaprr.html

[S59] C++：静态断言
来源：http://hz.redwolf501.top/gtvckbpznt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtyjgqbyll.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtcrzzdpxm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gttilkktcl.html

================================================================================
来源：http://hz.yj20258888.top/gtnuzqmkrd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ppjwa.cn/gtlzoesnlw.html

================================================================================
来源：http://hz.yangfankeji.com/gtlkjrzvrb.html

[T01] Kotlin：Hello World
来源：http://hz.shanyushiyangtech.top/gtirctpjqb.html

println("Hello")
来源：http://hz.shzxlz.cn/gtdymspfda.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtbcstjxhn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtnpqjkiio.html

[T03] Kotlin：字符串模板
来源：http://hz.yangfankeji.com/gtcqlzrzcg.html

"值: $b"
来源：http://hz.xziqi.cn/gtfnfzxgte.html

[T04] Kotlin：空安全
来源：http://hz.xylfe.cn/gtmxlegxoc.html

val n: String? = null;  n?.length
来源：http://hz.xinyue.icu/gtpovolekf.html

[T05] Kotlin：when 表达式
来源：http://hz.zhongyouzk.top/gtwtpstnrh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtgrtkzqcr.html

[T06] Kotlin：集合映射
来源：http://hz.sufxvd.cn/gtpxjynirg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtenpjcmrh.html

[T07] Kotlin：集合过滤
来源：http://hz.redwolf501.top/gtodyaicfc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.vqdsnc.cn/gtxyanmjfe.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gttbqdvvjv.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gthivqjndr.html

[T09] Kotlin：扩展函数
来源：http://hz.chenjidiqi.icu/gtnotwscux.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtimzpgyjq.html

[T10] Kotlin：默认参数
来源：http://hz.tanke756.top/gtmgofcvqg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cashguo.top/gtlyyncoow.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gtnrhjepcr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtztwpxwis.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtflkfssyu.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gtmrhywnig.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtwjyvrkvf.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gtjuoasdow.html

[T14] Kotlin：循环
来源：http://hz.hfpthk.cn/gtwmafesjn.html

for (i in 1..10) println(i)
来源：http://hz.gaohongyu789.top/gtzgpexgja.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gtneuwjgla.html

interface Shape { fun area(): Double }
来源：http://hz.iojbl.cn/gtvjsnnujn.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gttbkalkqp.html

print("Hello")
来源：http://hz.daxiang520.top/gtshqwmuos.html

[T17] Swift：变量与常量
来源：http://hz.jinqigufen.top/gtlgoobkep.html

var a = 1;  let b = 2
来源：http://hz.yongpay.top/gtzetivvkd.html

[T18] Swift：字符串插值
来源：http://hz.xuetiantiany.cn/gtehpnbbwk.html

"值: \(b)"
来源：http://hz.yj20258.top/gtjwkbeuhc.html

[T19] Swift：可选绑定
来源：http://hz.tanke756.top/gtkuyverbl.html

if let n = opt { print(n) }
来源：http://hz.yonumen.top/gtyyrtaakt.html

[T20] Swift：数组操作
来源：http://hz.zhijiandao.cn/gtvrguvtgh.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gthojjifip.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtmeitgkge.html

for x in a { print(x) }
来源：http://hz.smart0.xyz/gtfuetkcpf.html

[T22] Swift：字典
来源：http://hz.svipenyu.cn/gtsafvchoi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gtnolmsdfs.html

[T23] Swift：函数
来源：http://hz.zhaomingkeji.xyz/gtqiiwcwxh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnqzz.top/gthnbkoonf.html

[T24] Swift：闭包
来源：http://hz.wangdashe.top/gtbdkvchbv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhiwuduotai.top/gtzqdfdwsr.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtauzuzraq.html

struct P { var x: Int }
来源：http://hz.cheryme.top/gtskqnoedk.html

[T26] Swift：类与重写
来源：http://hz.yanxiufei.cn/gtmggkgrsq.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtzspuckzp.html

[T27] Swift：错误处理
来源：http://hz.jinqigfzy.top/gtekmdcwkp.html

do { try f() } catch { print(error) }
来源：http://hz.zhaomingkeji.xyz/gtyxanqlcm.html

[T28] Swift：枚举
来源：http://hz.cqqwz.cn/gtfhxfbtar.html

enum Color { case red, green }
来源：http://hz.guowangkeji.top/gtynvnefjr.html

[T29] Swift：guard 提前返回
来源：http://hz.xinyue.icu/gtzyhiysgs.html

guard let x = opt else { return }
来源：http://hz.ydjk.org.cn/gtwsrvvvjk.html

[T30] Swift：协议
来源：http://hz.chenlongwang.top/gtglgqbrqw.html

protocol Shape { func area() -> Double }
来源：http://hz.jinyuanbaomall.cn/gtwrtkegcf.html

[T31] Lua：Hello World
来源：http://hz.ywan-chungtsiang.top/gtjnwfeeia.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtsjxtxwei.html

[T32] Lua：局部变量
来源：http://hz.daxiang520.top/gtlznyvrla.html

local a = 1
来源：http://hz.hnxiangtu.top/gtdsjnykzi.html

[T33] Lua：表（数组）
来源：http://hz.yvedp.cn/gtkawwrktb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hammf.cn/gttvurcafm.html

[T34] Lua：遍历表
来源：http://hz.daxiang520.top/gtftbndjob.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jianghu66.top/gtjqzoesto.html

[T35] Lua：字典表
来源：http://hz.hywenlv.cn/gtgbaqkjaq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtrxwpeljj.html

[T36] Lua：函数
来源：http://hz.hfpthk.cn/gtrzwendos.html

function add(a, b) return a + b end
来源：http://hz.xingfuxueyuan.xyz/gtqiiorbcz.html

[T37] Lua：字符串拼接
来源：http://hz.sweek.top/gtlqqtxruq.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtblwiusiq.html

[T38] Lua：条件
来源：http://hz.jianghu66.top/gtswesxiyl.html

if x > 0 then print("正") end
来源：http://hz.ywan-chungtsiang.top/gtkepxbmmq.html

[T39] Lua：模式匹配
来源：http://hz.wangdashe.top/gtfezyhiqb.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtebatrfey.html

[T40] Lua：元表
来源：http://hz.jqgfzy.top/gtqhnvtlxn.html

setmetatable({}, { __index = base })
来源：http://hz.jianghu66.top/gtfbqffijv.html

[T41] Perl：Hello World
来源：http://hz.zhixingplan.top/gtibwktudn.html

print "Hello\n";
来源：http://hz.yuxming.cn/gtcghrxrsi.html

[T42] Perl：变量类型
来源：http://hz.hongshengwenyu.top/gtppsvhesg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.haohaochexian.top/gttdebzopi.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtajmpaklj.html

"值: $a"
来源：http://hz.xinyue.icu/gtofuqlymi.html

[T44] Perl：条件
来源：http://hz.nanxuanxn.top/gtbyllymwp.html

if ($a > 0) { print "正"; }
来源：http://hz.hongshengwenyu.top/gtqlaksusq.html

[T45] Perl：数组遍历
来源：http://hz.jinghuilouyu.cn/gtebsrjbap.html

for my $x (@arr) { print $x; }
来源：http://hz.0kj1m.cn/gtxkmpfcpy.html

[T46] Perl：哈希操作
来源：http://hz.quarkkingdee.top/gtrbewckak.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cashguo.top/gtqidbchza.html

[T47] Perl：正则捕获
来源：http://hz.zhijiandao.cn/gtinsdzjnj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daria6918.cn/gtylsgsnqx.html

[T48] Perl：正则替换
来源：http://hz.yuanzhike.top/gttolejycq.html

$s =~ s/old/new/g;
来源：http://hz.0kj1m.cn/gtbpvyqstb.html

[T49] Perl：函数
来源：http://hz.gzhubu.top/gthnndmpne.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.bjfxy.top/gtxkmugrff.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtzhltxjip.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jlsjyb.cn/gtjsspytyv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hammf.cn/gtclgbhgtv.html

[T51] Scala：Hello World
来源：http://hz.zhengqikj.top/gtdlfpflxu.html

println("Hello")
来源：http://hz.chenzaomai.com/gtribkfmuv.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtmpeyqhcr.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtgunqdbzs.html

[T53] Scala：字符串插值
来源：http://hz.bjfxy.top/gtvqbwrhvs.html

s"值: $b"
来源：http://hz.yanxiufei.cn/gtqsakqdou.html

[T54] Scala：集合映射
来源：http://hz.daxiang520.top/gtdetitrde.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnxiangtu.top/gtqljpktpn.html

[T55] Scala：集合过滤
来源：http://hz.tianlin.xyz/gtbhcnmdfh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.kuanghao11.cn/gtbcimbcmd.html

[T56] Scala：样例类
来源：http://hz.snrcjt.cn/gtqjmcrxpt.html

case class User(name: String, age: Int)
来源：http://hz.yueranfly.top/gtytrasnuy.html

[T57] Scala：模式匹配
来源：http://hz.wangdashe.top/gtbftmluuu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.havefunace.top/gtypydldce.html

[T58] Scala：函数定义
来源：http://hz.hnqzz.top/gtrltlmkyk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhiwuduotai.top/gtrwjbveim.html

[T59] Scala：循环
来源：http://hz.havefunace.top/gtbwhtpqkj.html

for (i <- 1 to 10) println(i)
来源：http://hz.bjfxy.top/gtprryqgku.html

[T60] Scala：折叠
来源：http://hz.nanxuanxn.top/gtexhxxjik.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aibaodan.cn/gtjleegdbk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrtdrwmxj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.wangdashe.top/gtnxmhitzf.html

================================================================================
来源：http://hz.mhx1999.top/gtnalikhct.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtopjdyjxg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.wangshuangyany.cn/gtpiiyobtw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuanzx.com/gttaufwarh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gtghczgbdf.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtzfjeaxid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.feifeiyinyue.top/gtpohofwac.html

[U04] Py：变量调试打印
来源：http://hz.jianghu66.top/gtfaxpnujw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.wangdashe.top/gtfhhhfmpo.html

[U05] Py：列表去重且保序
来源：http://hz.yanxiufei.cn/gtocykpceb.html

list(dict.fromkeys(arr))
来源：http://hz.xingfuxueyuan.xyz/gtzohkmitg.html

[U06] Py：合并两个字典
来源：http://hz.jinghuilouyu.cn/gtjaygoxmg.html

{**a, **b}
来源：http://hz.cashguo.top/gthzwkxqpo.html

[U07] Py：反转字典键值
来源：http://hz.bjfxy.top/gtehozojgf.html

{v: k for k, v in d.items()}
来源：http://hz.shangyingyoupin.top/gtxhbbsbay.html

[U08] Py：展平二维列表
来源：http://hz.haohaochexian.top/gtdkxmmvzg.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtqfzdeyck.html

[U09] Py：字典取最大值的键
来源：http://hz.c1oappe.top/gtncgkcpaz.html

max(d, key=d.get)
来源：http://hz.hnqzz.top/gtezfykpwm.html

[U10] Py：按值排序字典
来源：http://hz.chenzaomai.com/gtijlyyqlp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtkhknppuw.html

[U11] Py：生成器表达式
来源：http://hz.chenzaomai.com/gtcexhvijn.html

(x * 2 for x in arr)
来源：http://hz.hnxiangtu.top/gtbfclqxmz.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jlsjyb.cn/gtrzgsodrw.html

Counter(arr).most_common(3)
来源：http://hz.ywan-chungtsiang.top/gtvscdlneg.html

[U13] Py：固定长度队列
来源：http://hz.aizwys.cn/gtuvatvtxi.html

deque(maxlen=10)
来源：http://hz.zhengqikj.top/gtybheiyzc.html

[U14] Py：分组收集到列表
来源：http://hz.zhongyouzk.top/gtxrxorwmx.html

defaultdict(list)
来源：http://hz.jlsjyb.cn/gtckcezudl.html

[U15] Py：高精度计时
来源：http://hz.zycfv.cn/gtxejsyukm.html

t = time.perf_counter()
来源：http://hz.zdqjudy.top/gtdgnktofc.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtifhrvnsa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.meibo888.top/gtjodltgfa.html

[U17] Py：初始化日志
来源：http://hz.guannengcc.top/gtonreexzc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ydzc1.top/gtfhlvofqv.html

[U18] Py：预编译正则
来源：http://hz.sweek.top/gtbjaloidl.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtlbxvvnhi.html

[U19] Py：正则替换带回调
来源：http://hz.cucudq.cn/gtrubhqhkp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ybcxt.top/gtftfteauo.html

[U20] Py：缓存函数结果
来源：http://hz.zhixingplan.top/gtzlbmhali.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xylfe.cn/gtfwhnouyj.html

[U21] Py：自定义上下文管理器
来源：http://hz.yueranfly.top/gtnwhvtjru.html

@contextlib.contextmanager
来源：http://hz.chenjidiqi.icu/gttistigmi.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtnsqpfmxm.html

list(zip(*m))
来源：http://hz.daxiang520.top/gtgefdfkzy.html

[U23] Py：分块读取大文件
来源：http://hz.jinyuanbaomall.cn/gtcknpstih.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yonumen.top/gtawvrwjax.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtciiylfla.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ivvv.top/gtdcaxxuyv.html

[U25] Py：CSV 按字典读
来源：http://hz.vqdsnc.cn/gtzgzdzuvc.html

csv.DictReader(f)
来源：http://hz.yonumen.top/gthtxwndzf.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gtwubcolpm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenzaomai.com/gtwmxpraau.html

[U27] Py：异步 HTTP
来源：http://hz.daxiang520.top/gtxuxavigq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sxryk.cn/gtfcrtidmh.html

[U28] Py：类型别名
来源：http://hz.zhixingplan.top/gtndyymofn.html

UserId = int
来源：http://hz.hysaishi.cn/gthvxrtnjq.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gttbtxsztu.html

@property 与 @x.setter 配合
来源：http://hz.iojbl.cn/gtxikhsjlv.html

[U30] Py：数据类
来源：http://hz.zhoulong.xyz/gtpgaijhzt.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtsdroompg.html

[U31] Py：单测
来源：http://hz.jinyuanbaomall.cn/gtpqhpnzzm.html

python -m pytest -q
来源：http://hz.cdnleiting.top/gtuvnjfmsn.html

[U32] Py：代码格式化
来源：http://hz.hfpthk.cn/gtrtixmbum.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtzlewwnyl.html

[U33] Py：打包发布
来源：http://hz.xinyue.icu/gtakgmceiy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.haohaochexian.top/gtfqkwlcdd.html

[U34] Py：判断编码
来源：http://hz.sufxvd.cn/gtlukvntju.html

chardet.detect(raw)
来源：http://hz.birdmap.top/gtxgairpgq.html

[U35] Py：发送邮件
来源：http://hz.xingfuxueyuan.xyz/gtrzwowkqn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.9152youxi.cn/gtmkyzucfj.html

[U36] Py：定时任务
来源：http://hz.fzhhl.top/gthuouotpq.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhixingplan.top/gtvwmzxtkx.html

[U37] Py：读写 Excel
来源：http://hz.pycfn.com/gtocfaywpx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xziqi.cn/gtyatstpit.html

[U38] Py：获取脚本所在目录
来源：http://hz.jiagoushi.top/gtwfoieqnu.html

Path(__file__).resolve().parent
来源：http://hz.cqqwz.cn/gtbbjbcpsx.html

[U39] Py：判断是否在交互环境
来源：http://hz.yueranfly.top/gtotnjqssd.html

sys.stdout.isatty()
来源：http://hz.daria6918.cn/gtkvgcdejv.html

[U40] Py：打印到标准错误
来源：http://hz.316326.xyz/gtqdhxmiyr.html

print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtqwqvonyd.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xingfuxueyuan.xyz/gtkfcdntqb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shzxlz.cn/gtfysnrfjn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhengqikj.top/gtaczlwmhb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jyoumei.cn/gtyddzlulz.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtmztculll.html

namespace App\Http;
来源：http://hz.gotoacloud.top/gtflgvivjn.html

[U44] PHP：开启严格类型
来源：http://hz.shzxlz.cn/gtqxichksk.html

declare(strict_types=1);
来源：http://hz.pycfn.com/gtsvhbdlvz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yvedp.cn/gtgiweqcta.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtucdnptbs.html

[U46] PHP：可空类型
来源：http://hz.hammf.cn/gtbbfjvenp.html

?string $name = null
来源：http://hz.kuanghao11.cn/gtiejfiado.html

[U47] PHP：联合类型
来源：http://hz.ydzc1.top/gtvbztadqh.html

int|string $id
来源：http://hz.jqgufenzy.top/gtddkjkitb.html

[U48] PHP：纯枚举
来源：http://hz.0kj1m.cn/gtijddezts.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhixingplan.top/gtkqeingmk.html

[U49] PHP：只读属性
来源：http://hz.xingfuxueyuan.xyz/gtstrfitws.html

public readonly string $name
来源：http://hz.hnxiangtu.top/gttrpqxjqs.html

[U50] PHP：构造器属性提升
来源：http://hz.yangfankeji.com/gtxyyxwect.html

public function __construct(private int $id) {}
来源：http://hz.ybcxt.top/gtsvyfvgqy.html

[U51] PHP：数组解构
来源：http://hz.yj202588.top/gtutjkhfvp.html

[$a, $b] = $arr;
来源：http://hz.jyoumei.cn/gtiwezdebz.html

[U52] PHP：箭头函数
来源：http://hz.smart0.xyz/gtqzrhhehk.html

$double = fn($x) => $x * 2;
来源：http://hz.chenjidiqi.icu/gtojyfjplg.html

[U53] PHP：空合并运算符
来源：http://hz.xinyue.icu/gtuhdazsfg.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhengqikj.top/gtziettvzd.html

[U54] PHP：空安全调用
来源：http://hz.meibo888.top/gtdxkxpzqq.html

$obj?->method()
来源：http://hz.shanyushiyangkeji.top/gtxsknisus.html

[U55] PHP：match 表达式
来源：http://hz.kuanghao11.cn/gtczbqzpqj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nwbrower.top/gtltyqxxfz.html

[U56] PHP：命名参数
来源：http://hz.xinyue.icu/gtuqmtpvdb.html

f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtpdqajmyc.html

[U57] PHP：字符串插值
来源：http://hz.svipenyu.cn/gtyzjnyyyu.html

"值: {$a}"
来源：http://hz.wangshuangyany.cn/gtloabphls.html

[U58] PHP：数组三件套
来源：http://hz.zhaomingkeji.xyz/gtiwxxejjl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hammf.cn/gtjxwwtjkg.html

[U59] PHP：自定义排序
来源：http://hz.zhoulong.xyz/gtzcdisizj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtdpxfsqhr.html

[U60] PHP：JSON 编解码
来源：http://hz.ydzc1.top/gtnevpdlbo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jqgfzy.top/gtysranhvt.html

[U61] PHP：正则
来源：http://hz.jqgfzy.top/gtbvooijnb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtinwjfryq.html

[U62] PHP：日期对象
来源：http://hz.fzhhl.top/gtdmuvbdgj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigfzy.top/gtbypznauo.html

[U63] PHP：文件读写
来源：http://hz.jinqigfzy.top/gtkmkyexfj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhaomingkeji.xyz/gtnxnlntfz.html

[U64] PHP：目录遍历
来源：http://hz.aizwys.cn/gthmfwodce.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhoulong.xyz/gtmhezxjkb.html

[U65] PHP：会话
来源：http://hz.cashguo.top/gtxlsbacnx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sweek.top/gtzjexfnbv.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtxmvwnaxc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.bjfxy.top/gtnttsouhj.html

[U67] PHP：处理文件上传
来源：http://hz.xinyue.icu/gtskcdyqwn.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.iojbl.cn/gtfruqcvbs.html

[U68] PHP：PDO 连接
来源：http://hz.nanxuanxn.top/gtouoszkub.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.hywenlv.cn/gtjajkosba.html


<!-- 参考信息 -->