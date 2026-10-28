代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtgobsvnck.html

[S49] C++：写文件
来源：http://hz.ydjk.org.cn/gtsblvumtc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtbeupzpvd.html

[S50] C++：格式化数字
来源：http://hz.ivvv.top/gtrtvghvam.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nwbrower.top/gtuumokcyo.html

[S51] C++：显式类型转换
来源：http://hz.quarkkingdee.top/gtetkympii.html

static_cast<double>(a) / b
来源：http://hz.hammf.cn/gtekqwyore.html

[S52] C++：const 与 noexcept
来源：http://hz.gaohongyu789.top/gtmjydpvca.html

int size() const noexcept { return n_; }
来源：http://hz.shangyingyoupin.top/gtaqzpoais.html

[S53] C++：移动语义
来源：http://hz.bjfxy.top/gtdirjbmkj.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gthjgsvcii.html

[S54] C++：异常处理
来源：http://hz.sufxvd.cn/gtqhymzxtw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtegrfqzjx.html

[S55] C++：结构化绑定
来源：http://hz.yonumen.top/gtvanzrgcl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtkgsfkmck.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtvyzzcrhp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangshuangyany.cn/gtrejeqncd.html

[S57] C++：编译期常量
来源：http://hz.haohaochexian.top/gttrddvzfb.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gteaohooos.html

[S58] C++：命名空间
来源：http://hz.smart0.xyz/gtqluewgxx.html

namespace ns { int f() { return 1; } }
来源：http://hz.9152youxi.cn/gtcidoxyxu.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gtypkbkqbl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydjk.org.cn/gtluilcaoy.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtbmaqicwa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangdashe.top/gtwzyddbdz.html

================================================================================
来源：http://hz.guannengcc.top/gtqnfgdehe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zdqjudy.top/gtajurqwzc.html

================================================================================
来源：http://hz.cashguo.top/gtcsunslwd.html

[T01] Kotlin：Hello World
来源：http://hz.zhengqikj.top/gtwpokpnft.html

println("Hello")
来源：http://hz.sweek.top/gtaznxpbyx.html

[T02] Kotlin：变量
来源：http://hz.dashuyun.cn/gtcuezuvdb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shuidangran.top/gtdpuqujrc.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgfzy.top/gtugpzxmil.html

"值: $b"
来源：http://hz.ivvv.top/gtgmkoylql.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gtuntqxofe.html

val n: String? = null;  n?.length
来源：http://hz.yueranfly.top/gtjwzduwwg.html

[T05] Kotlin：when 表达式
来源：http://hz.tanke756.top/gttfixpdtg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtqqauzgyw.html

[T06] Kotlin：集合映射
来源：http://hz.hysaishi.cn/gtlrtkhqwy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ywan-chungtsiang.top/gtsnltatxf.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtgzxjopps.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.guannengcc.top/gtqxoxlzyp.html

[T08] Kotlin：数据类
来源：http://hz.sxryk.cn/gtkzhuapli.html

data class User(val name: String, val age: Int)
来源：http://hz.zhiwuduotai.top/gtyfrhwwks.html

[T09] Kotlin：扩展函数
来源：http://hz.guannengcc.top/gtgonwlhfv.html

fun String.exclaim() = this + "!"
来源：http://hz.xingfuxueyuan.xyz/gtsrrzifzz.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtzzgqgcrt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tanke756.top/gtrjykxonh.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtzltowxmq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtbyixljkr.html

[T12] Kotlin：解构声明
来源：http://hz.nwbrower.top/gtmsbkjacy.html

val (a, b) = Pair(1, 2)
来源：http://hz.quarkkingdee.top/gtnnwxbuit.html

[T13] Kotlin：只读 Map
来源：http://hz.ehwqpu.com/gtliumarew.html

val m = mapOf("a" to 1)
来源：http://hz.cheryme.top/gtlqyabxmn.html

[T14] Kotlin：循环
来源：http://hz.guowangkeji.top/gtsfzgqlrs.html

for (i in 1..10) println(i)
来源：http://hz.shzxlz.cn/gtunzuyuxy.html

[T15] Kotlin：接口
来源：http://hz.snrcjt.cn/gtfojfniqv.html

interface Shape { fun area(): Double }
来源：http://hz.shangyingyoupin.top/gtygjxxruz.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtyymjzhoj.html

print("Hello")
来源：http://hz.nanxinkj.top/gttyqzwucl.html

[T17] Swift：变量与常量
来源：http://hz.yj20258.top/gtfgjudtyi.html

var a = 1;  let b = 2
来源：http://hz.guowangkeji.top/gtzawpfeub.html

[T18] Swift：字符串插值
来源：http://hz.nanxinkj.top/gtomeopvzi.html

"值: \(b)"
来源：http://hz.dashuyun.cn/gtdexascub.html

[T19] Swift：可选绑定
来源：http://hz.c1oappe.top/gtgnvhtebm.html

if let n = opt { print(n) }
来源：http://hz.hongshengwenyu.top/gtqhmxnmsv.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gtnkcmulqa.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xingfuxueyuan.xyz/gtbbduzljy.html

[T21] Swift：遍历
来源：http://hz.xuetiantiany.cn/gtxoefwraq.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtmphnmryy.html

[T22] Swift：字典
来源：http://hz.xuetiantiany.cn/gtllpeddby.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtrlhgqjrv.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gtmjgtinup.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtshyhrxrb.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtpfgzusup.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtuyfuqksq.html

[T25] Swift：结构体
来源：http://hz.nanxuanxn.top/gtcsqujisi.html

struct P { var x: Int }
来源：http://hz.yj202588.top/gtsbnhpkkk.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gtakarsekd.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtgbbbpybg.html

[T27] Swift：错误处理
来源：http://hz.c1oappe.top/gtdjhnccpw.html

do { try f() } catch { print(error) }
来源：http://hz.jqgufenzy.top/gtwbwcnmbu.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtjmhbtulh.html

enum Color { case red, green }
来源：http://hz.dianchejie.cn/gtrehcptal.html

[T29] Swift：guard 提前返回
来源：http://hz.sweek.top/gtiqmholim.html

guard let x = opt else { return }
来源：http://hz.shangyingyoupin.top/gtrbfdzfbu.html

[T30] Swift：协议
来源：http://hz.yonumen.top/gtxrdjbulm.html

protocol Shape { func area() -> Double }
来源：http://hz.shuidangran.top/gtgpquhgsl.html

[T31] Lua：Hello World
来源：http://hz.shangyingyoupin.top/gtcnkpuapd.html

print("Hello")
来源：http://hz.xinyue.icu/gttoxqvuvk.html

[T32] Lua：局部变量
来源：http://hz.yongpay.top/gtetuogfsm.html

local a = 1
来源：http://hz.ehwqpu.com/gtkfxvvqvi.html

[T33] Lua：表（数组）
来源：http://hz.c1oappe.top/gtmisbsxpw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuetiantiany.cn/gtudxgwcet.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gtnuwarhnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenlongwang.top/gtmntzgfjl.html

[T35] Lua：字典表
来源：http://hz.yueranfly.top/gtztofkysw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shzxlz.cn/gtcucqmpop.html

[T36] Lua：函数
来源：http://hz.tianlin.xyz/gthqsjznbh.html

function add(a, b) return a + b end
来源：http://hz.mhx1999.top/gtzpcpweth.html

[T37] Lua：字符串拼接
来源：http://hz.zhengqikj.top/gtczwyqfyu.html

"a" .. "b"
来源：http://hz.chenlongwang.top/gtnjjjjzzq.html

[T38] Lua：条件
来源：http://hz.shzxlz.cn/gtrhmbouzu.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtvnbqdyye.html

[T39] Lua：模式匹配
来源：http://hz.yj20258888.top/gtpnzjklbf.html

string.find(s, "%d+")
来源：http://hz.yongpay.top/gtvlfhlmak.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gtlgzxhsaa.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gttnvysvzu.html

[T41] Perl：Hello World
来源：http://hz.sxryk.cn/gtwngbrici.html

print "Hello\n";
来源：http://hz.ivvv.top/gtszgmnolf.html

[T42] Perl：变量类型
来源：http://hz.haohaochexian.top/gtzfwaxhfn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gttrajyrpc.html

[T43] Perl：字符串插值
来源：http://hz.bjfxy.top/gttmpkjtfj.html

"值: $a"
来源：http://hz.kuanghao11.cn/gtrujqntxi.html

[T44] Perl：条件
来源：http://hz.jqgufenzy.top/gtflcglbcc.html

if ($a > 0) { print "正"; }
来源：http://hz.shzxlz.cn/gtbmudtpzh.html

[T45] Perl：数组遍历
来源：http://hz.hnqzz.top/gttgwhslmx.html

for my $x (@arr) { print $x; }
来源：http://hz.cqqwz.cn/gtziykvwnz.html

[T46] Perl：哈希操作
来源：http://hz.ywan-chungtsiang.top/gtpjymslpt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cheryme.top/gtaougqgce.html

[T47] Perl：正则捕获
来源：http://hz.ivvv.top/gtgbdstfjj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shangyingyoupin.top/gtnjgvbrza.html

[T48] Perl：正则替换
来源：http://hz.jinghuilouyu.cn/gtdqklmoez.html

$s =~ s/old/new/g;
来源：http://hz.jqgufenzy.top/gtyztfuvlq.html

[T49] Perl：函数
来源：http://hz.sysykeji.top/gttozdmaqn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ivvv.top/gtrzmxuwcg.html

[T50] Perl：逐行读文件
来源：http://hz.jqgfzy.top/gtdpeozihb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cucudq.cn/gtymdxwrjp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hammf.cn/gtxxkmnrkm.html

[T51] Scala：Hello World
来源：http://hz.yanxiufei.cn/gtctwvygcu.html

println("Hello")
来源：http://hz.hywenlv.cn/gtjbrbywfy.html

[T52] Scala：变量
来源：http://hz.ehwqpu.com/gtlgulmjku.html

val a = 1;  var b = 2
来源：http://hz.shuidangran.top/gtjgoiukhg.html

[T53] Scala：字符串插值
来源：http://hz.yueranfly.top/gtzgqvlvte.html

s"值: $b"
来源：http://hz.tian-w.cn/gtukwpqujv.html

[T54] Scala：集合映射
来源：http://hz.chenjidiqi.icu/gtcsryxpck.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jqgufenzy.top/gtwmlzcjpj.html

[T55] Scala：集合过滤
来源：http://hz.cheryme.top/gtvrclnfnl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.wangdashe.top/gtbkkmxvvc.html

[T56] Scala：样例类
来源：http://hz.yj20258.top/gtlemvygfj.html

case class User(name: String, age: Int)
来源：http://hz.chenlongwang.top/gtzwxmosyr.html

[T57] Scala：模式匹配
来源：http://hz.chenzaomai.com/gtulxntbpd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ppjwa.cn/gtcvxcsjnq.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtofpprvvf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xylfe.cn/gtmontbymo.html

[T59] Scala：循环
来源：http://hz.zhoulong.xyz/gttqaattpr.html

for (i <- 1 to 10) println(i)
来源：http://hz.yueranfly.top/gtnjkhvpey.html

[T60] Scala：折叠
来源：http://hz.ywan-chungtsiang.top/gtjiezpeqv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258.top/gtnmfanskt.html

================================================================================
来源：http://hz.hammf.cn/gtondavhkt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtjbdtxfuv.html

================================================================================
来源：http://hz.jinqigufen.top/gtwdikhtdy.html

[U01] Py：创建虚拟环境
来源：http://hz.guowangkeji.top/gtrwsetcod.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.yj20258888.top/gtuujrqqrt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhiwuduotai.top/gtghrizfmt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.redwolf501.top/gtczxxorel.html

[U03] Py：加载 .env 配置
来源：http://hz.yuanzhike.top/gthhgcweyx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xingfuxueyuan.xyz/gtqjavahrq.html

[U04] Py：变量调试打印
来源：http://hz.cucudq.cn/gtezxjrnbv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hysaishi.cn/gtkvbdunhu.html

[U05] Py：列表去重且保序
来源：http://hz.jlsjyb.cn/gtkllbiyjz.html

list(dict.fromkeys(arr))
来源：http://hz.ivvv.top/gtxuzvxovt.html

[U06] Py：合并两个字典
来源：http://hz.meibo888.top/gttrmvqmgv.html

{**a, **b}
来源：http://hz.yongpay.top/gtphdoxdpm.html

[U07] Py：反转字典键值
来源：http://hz.jinqigfzy.top/gtkoopofkl.html

{v: k for k, v in d.items()}
来源：http://hz.quarkkingdee.top/gtswcahhkw.html

[U08] Py：展平二维列表
来源：http://hz.nanxuanxn.top/gthbjudigk.html

[y for x in nested for y in x]
来源：http://hz.shangyingyoupin.top/gtuipwidyn.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258.top/gtsonjafls.html

max(d, key=d.get)
来源：http://hz.daxiang520.top/gtrsvogrvr.html

[U10] Py：按值排序字典
来源：http://hz.jqgufenzy.top/gtemzwqkeh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.pycfn.com/gthpfjlyvt.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtcahjkgqx.html

(x * 2 for x in arr)
来源：http://hz.iojbl.cn/gtyckzqysn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtfmlpgrgr.html

Counter(arr).most_common(3)
来源：http://hz.aibaodan.cn/gtdodtllks.html

[U13] Py：固定长度队列
来源：http://hz.dashuyun.cn/gtfyuzcuaa.html

deque(maxlen=10)
来源：http://hz.pengpengdd.cyou/gtizdezfvq.html

[U14] Py：分组收集到列表
来源：http://hz.jqgufenzy.top/gtkwkpzldr.html

defaultdict(list)
来源：http://hz.gogol.net.cn/gtrblrzbsb.html

[U15] Py：高精度计时
来源：http://hz.jiagoushi.top/gtefltmber.html

t = time.perf_counter()
来源：http://hz.aizwys.cn/gtzixgqzdu.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangtech.top/gtbesycjfn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ppjwa.cn/gtgzcrkisq.html

[U17] Py：初始化日志
来源：http://hz.shanyushiyangkeji.top/gtgsghogqm.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuxming.cn/gtuqldfisb.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtsrtpqmmd.html

pat = re.compile(r"\d+")
来源：http://hz.tianlin.xyz/gtvkehuqnh.html

[U19] Py：正则替换带回调
来源：http://hz.aibaodan.cn/gtjcfcyurf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.52xcode.cn/gtqvkjawss.html

[U20] Py：缓存函数结果
来源：http://hz.hongshengwenyu.top/gtgdkoyemt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258888.top/gtijvctoec.html

[U21] Py：自定义上下文管理器
来源：http://hz.xinyue.icu/gtvgzogcdg.html

@contextlib.contextmanager
来源：http://hz.aibaodan.cn/gtejvgdpvi.html

[U22] Py：矩阵转置
来源：http://hz.yangfankeji.com/gtnnniavvy.html

list(zip(*m))
来源：http://hz.shuidangran.top/gtyqjbrplj.html

[U23] Py：分块读取大文件
来源：http://hz.haohaochexian.top/gtisepqfql.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daria6918.cn/gtidnnhiqq.html

[U24] Py：路径操作
来源：http://hz.shuidangran.top/gtomntpimp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yvedp.cn/gtbridjutc.html

[U25] Py：CSV 按字典读
来源：http://hz.jinghuilouyu.cn/gtxncuyrlf.html

csv.DictReader(f)
来源：http://hz.jlsjyb.cn/gtilxqwesc.html

[U26] Py：并发下载
来源：http://hz.kuanghao11.cn/gtmciyvawg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtmtuypbou.html

[U27] Py：异步 HTTP
来源：http://hz.jqgfzy.top/gtmwemkkla.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.feifeiyinyue.top/gtvuruoxcw.html

[U28] Py：类型别名
来源：http://hz.jinqigfzy.top/gtehmblrsp.html

UserId = int
来源：http://hz.cashguo.top/gtsexyeqzy.html

[U29] Py：属性校验
来源：http://hz.wangdashe.top/gtnntquhuq.html

@property 与 @x.setter 配合
来源：http://hz.birdmap.top/gtkmwrrjpo.html

[U30] Py：数据类
来源：http://hz.aizwys.cn/gtflkfqppg.html

@dataclass(slots=True)
来源：http://hz.sufxvd.cn/gtpiqwezpl.html

[U31] Py：单测
来源：http://hz.gaohongyu789.top/gtcivrjtrg.html

python -m pytest -q
来源：http://hz.zhixingplan.top/gtsbbacywk.html

[U32] Py：代码格式化
来源：http://hz.ehwqpu.com/gtqglppmjo.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtuulwytgi.html

[U33] Py：打包发布
来源：http://hz.c1oappe.top/gtefskufja.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pengpengdd.cyou/gtimhnpehn.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtucexanzp.html

chardet.detect(raw)
来源：http://hz.hfpthk.cn/gtjcwhmvns.html

[U35] Py：发送邮件
来源：http://hz.ydzc1.top/gtmlxxnier.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhijiandao.cn/gtxwnyaqsz.html

[U36] Py：定时任务
来源：http://hz.fengsongda.top/gtojokkgiw.html

schedule.every(10).minutes.do(job)
来源：http://hz.fengsongda.top/gtqoncapxk.html

[U37] Py：读写 Excel
来源：http://hz.xylfe.cn/gtngehyfow.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cdnleiting.top/gtabnugqpw.html

[U38] Py：获取脚本所在目录
来源：http://hz.ywan-chungtsiang.top/gtsudsjhnc.html

Path(__file__).resolve().parent
来源：http://hz.xziqi.cn/gtsrasnydw.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenzaomai.com/gtofhbwmmq.html

sys.stdout.isatty()
来源：http://hz.gzhubu.top/gtnexwpael.html

[U40] Py：打印到标准错误
来源：http://hz.quarkkingdee.top/gtkvcadiov.html

print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtvrhhqhga.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yanxiufei.cn/gtzvcrsvyy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hysaishi.cn/gtmrsovbjc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ybcxt.top/gtdxvecvye.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.52xcode.cn/gtlbfmmquc.html

[U43] PHP：声明命名空间
来源：http://hz.zhiwuduotai.top/gthajpcsmb.html

namespace App\Http;
来源：http://hz.jiagoushi.top/gtuwtieseb.html

[U44] PHP：开启严格类型
来源：http://hz.zhongyouzk.top/gtuxxzrlnr.html

declare(strict_types=1);
来源：http://hz.chenlongwang.top/gthrwrpfea.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenzaomai.com/gttzddvrdm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtddavzgsf.html

[U46] PHP：可空类型
来源：http://hz.c1oappe.top/gtygbwfdpo.html

?string $name = null
来源：http://hz.zhengqikj.top/gttgjiwzxl.html

[U47] PHP：联合类型
来源：http://hz.xuetiantiany.cn/gtjjfpxhgo.html

int|string $id
来源：http://hz.cdnleiting.top/gtdcbcuwpo.html

[U48] PHP：纯枚举
来源：http://hz.shanyushiyangkeji.top/gtnmqumbyo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hfpthk.cn/gtjlhndspa.html

[U49] PHP：只读属性
来源：http://hz.yonumen.top/gtplfftvwj.html

public readonly string $name
来源：http://hz.zhoulong.xyz/gtiihwwhyx.html

[U50] PHP：构造器属性提升
来源：http://hz.jianghu66.top/gtfmrqmics.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gtthihtusx.html

[U51] PHP：数组解构
来源：http://hz.vqdsnc.cn/gtcrhtqhih.html

[$a, $b] = $arr;
来源：http://hz.vqdsnc.cn/gtrdnwfmhw.html

[U52] PHP：箭头函数
来源：http://hz.tanke756.top/gtsjhmidzq.html

$double = fn($x) => $x * 2;
来源：http://hz.hywenlv.cn/gtbbgpkiwc.html

[U53] PHP：空合并运算符
来源：http://hz.bjfxy.top/gtdfpwitce.html

$v = $a ?? $b ?? "default";
来源：http://hz.daxiang520.top/gtghpqzbew.html

[U54] PHP：空安全调用
来源：http://hz.bjfxy.top/gtwaqfjgnu.html

$obj?->method()
来源：http://hz.zhiwuduotai.top/gtnueutbfi.html

[U55] PHP：match 表达式
来源：http://hz.yanxiufei.cn/gtnivcppgr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ivvv.top/gtghhknzog.html

[U56] PHP：命名参数
来源：http://hz.xingfuxueyuan.xyz/gtffmqjetm.html

f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtuzzgstij.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtmoymrtiy.html

"值: {$a}"
来源：http://hz.xuetiantiany.cn/gtmsoczzlu.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtecpbvjna.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenlongwang.top/gtymnzbykx.html

[U59] PHP：自定义排序
来源：http://hz.feifeiyinyue.top/gtbinvbtpe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtbuvnrqrg.html

[U60] PHP：JSON 编解码
来源：http://hz.pengpengdd.cyou/gthobgajjm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.aizwys.cn/gtbimwgrzw.html

[U61] PHP：正则
来源：http://hz.hywenlv.cn/gtxcedblaj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtnyxdnriq.html

[U62] PHP：日期对象
来源：http://hz.cucudq.cn/gtlremzrds.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shanyushiyangtech.top/gtuflrjfxg.html

[U63] PHP：文件读写
来源：http://hz.hongshengwenyu.top/gtvhhozeki.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ydzc1.top/gttcdzokce.html

[U64] PHP：目录遍历
来源：http://hz.sysykeji.top/gtzvdvawgx.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hfpthk.cn/gtprpiyhdm.html

[U65] PHP：会话
来源：http://hz.jqgfzy.top/gtfiiuursr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.andypj.xyz/gtbwiaimyo.html

[U66] PHP：设置 Cookie
来源：http://hz.hfpthk.cn/gtlbcekdam.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtyswlmzda.html

[U67] PHP：处理文件上传
来源：http://hz.zycfv.cn/gtfcgmuuzd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhixingplan.top/gtjeqyikxp.html

[U68] PHP：PDO 连接
来源：http://hz.cashguo.top/gtydftqkox.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtqjwdvlel.html

[U69] PHP：PDO 预处理
来源：http://hz.nwbrower.top/gtkhvpwtxd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xingfuxueyuan.xyz/gtsqmzdeus.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gtlxjhmmss.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.wangshuangyany.cn/gtgdqduogx.html

[U71] PHP：抛出异常
来源：http://hz.yongpay.top/gtsyjbhskq.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinyuanbaomall.cn/gtyydkphfl.html

[U72] PHP：写错误日志
来源：http://hz.tianlin.xyz/gtkeewwnoj.html

error_log("失败: " . $e->getMessage());
来源：http://hz.quarkkingdee.top/gtdreycrwg.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenzaomai.com/gtlprdqqcr.html

parse_ini_file("config.ini", true)
来源：http://hz.sxryk.cn/gtqwzraddb.html

[U74] PHP：读取环境变量
来源：http://hz.cucudq.cn/gtpmkluumu.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xziqi.cn/gtremyqtfs.html


<!-- 参考信息 -->