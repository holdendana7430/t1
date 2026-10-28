代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtbdzniqhz.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtpfzilhhg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gtsuhydram.html

[S50] C++：格式化数字
来源：http://hz.iojbl.cn/gttuwjgbcu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtcfnqllei.html

[S51] C++：显式类型转换
来源：http://hz.c1oappe.top/gtepyjctcr.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtyrjmihbw.html

[S52] C++：const 与 noexcept
来源：http://hz.hnxiangtu.top/gtbzpdlbss.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtflikrfoi.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtwupgcrep.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtxiuchglp.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtmltivuks.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.snrcjt.cn/gtkteagypq.html

[S55] C++：结构化绑定
来源：http://hz.gotoacloud.top/gtcwbaxiny.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dianchejie.cn/gtmkscuynx.html

[S56] C++：optional
来源：http://hz.ppjwa.cn/gttxrztovc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yanxiufei.cn/gtzocgeglv.html

[S57] C++：编译期常量
来源：http://hz.dianchejie.cn/gtvdrwwzpa.html

constexpr int N = 10;
来源：http://hz.jlsjyb.cn/gtuzmzmsvp.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtknffpovo.html

namespace ns { int f() { return 1; } }
来源：http://hz.mhx1999.top/gtlsnjvjdr.html

[S59] C++：静态断言
来源：http://hz.jyoumei.cn/gtalpouhvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yanxiufei.cn/gtbhlzcfwz.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtkqvmlkyg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yangfankeji.com/gtxmrwrlrx.html

================================================================================
来源：http://hz.mhx1999.top/gtxspmybxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gttfmhpsws.html

================================================================================
来源：http://hz.yj202588.top/gtllgfqrrf.html

[T01] Kotlin：Hello World
来源：http://hz.zhengqikj.top/gtlfnmtags.html

println("Hello")
来源：http://hz.zhixingplan.top/gtkoskfyii.html

[T02] Kotlin：变量
来源：http://hz.jinghuilouyu.cn/gtshdwckqd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtpsjmokey.html

[T03] Kotlin：字符串模板
来源：http://hz.yongpay.top/gtprsdqwzd.html

"值: $b"
来源：http://hz.ivvv.top/gtigxcocrx.html

[T04] Kotlin：空安全
来源：http://hz.xylfe.cn/gtdcalahfx.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtyqpfxquw.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtefwmtsvh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhengqikj.top/gtpxfuxdep.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gttkwktrtb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtidnwrmtg.html

[T07] Kotlin：集合过滤
来源：http://hz.quarkkingdee.top/gtzcvqsgyl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yangfankeji.com/gtmgwtsudf.html

[T08] Kotlin：数据类
来源：http://hz.ydjk.org.cn/gtlldygzts.html

data class User(val name: String, val age: Int)
来源：http://hz.gaohongyu789.top/gtcnxnmaui.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtlzkphsiw.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtjynnyobl.html

[T10] Kotlin：默认参数
来源：http://hz.yuxming.cn/gtajdrqdhv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shuidangran.top/gtqsryavak.html

[T11] Kotlin：协程
来源：http://hz.yj20258888.top/gtbctzgnle.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jqgufenzy.top/gtgcmkrxzj.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtsbyqhmvq.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtrvkaemgi.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gthlgmzgxu.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gtctjqohqs.html

[T14] Kotlin：循环
来源：http://hz.zhixingplan.top/gtnmdigfbi.html

for (i in 1..10) println(i)
来源：http://hz.tanke756.top/gtudpbqtpe.html

[T15] Kotlin：接口
来源：http://hz.havefunace.top/gtmpxhewxg.html

interface Shape { fun area(): Double }
来源：http://hz.pycfn.com/gtbdpznxzb.html

[T16] Swift：Hello World
来源：http://hz.sufxvd.cn/gtrqutjowe.html

print("Hello")
来源：http://hz.xziqi.cn/gtjvpdduai.html

[T17] Swift：变量与常量
来源：http://hz.ivvv.top/gtbytnvjsz.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtwkpnusxm.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtloewoqux.html

"值: \(b)"
来源：http://hz.hysaishi.cn/gtichchbnm.html

[T19] Swift：可选绑定
来源：http://hz.aibaodan.cn/gthtnawvph.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtsxjtrzob.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gtoxezhmyw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guowangkeji.top/gttyzyoyka.html

[T21] Swift：遍历
来源：http://hz.cashguo.top/gtvhokqsxq.html

for x in a { print(x) }
来源：http://hz.pycfn.com/gtdcaflqhi.html

[T22] Swift：字典
来源：http://hz.chenjidiqi.icu/gtllcctwxv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cheryme.top/gtwocirsnn.html

[T23] Swift：函数
来源：http://hz.aizwys.cn/gtzifjhdyu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtcgjxglmr.html

[T24] Swift：闭包
来源：http://hz.shuidangran.top/gtsbetotkj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtbjvruqwv.html

[T25] Swift：结构体
来源：http://hz.ybcxt.top/gtuxvtltbx.html

struct P { var x: Int }
来源：http://hz.hywenlv.cn/gtsxwngvmy.html

[T26] Swift：类与重写
来源：http://hz.sysykeji.top/gtxawnrmln.html

class A: Base { override func f() {} }
来源：http://hz.ppjwa.cn/gtleknrjfh.html

[T27] Swift：错误处理
来源：http://hz.yvedp.cn/gtpsbxendj.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtetltpzcc.html

[T28] Swift：枚举
来源：http://hz.cdnleiting.top/gtcaahgxaf.html

enum Color { case red, green }
来源：http://hz.xinyue.icu/gthiorllfy.html

[T29] Swift：guard 提前返回
来源：http://hz.aibaodan.cn/gtwmjjkfpe.html

guard let x = opt else { return }
来源：http://hz.vqdsnc.cn/gttbelptoz.html

[T30] Swift：协议
来源：http://hz.ywan-chungtsiang.top/gtyxsqcefb.html

protocol Shape { func area() -> Double }
来源：http://hz.ppjwa.cn/gtcjxkmptb.html

[T31] Lua：Hello World
来源：http://hz.fengsongda.top/gtgtnddnlo.html

print("Hello")
来源：http://hz.daxiang520.top/gtxzercsed.html

[T32] Lua：局部变量
来源：http://hz.cdnleiting.top/gtfozuropb.html

local a = 1
来源：http://hz.cqqwz.cn/gtjticrhwj.html

[T33] Lua：表（数组）
来源：http://hz.zhaomingkeji.xyz/gtebpesusx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydzc1.top/gtmsatuqya.html

[T34] Lua：遍历表
来源：http://hz.ybcxt.top/gtmzsxpxrc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtdjvhhydk.html

[T35] Lua：字典表
来源：http://hz.yonumen.top/gthelykwvt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ivvv.top/gtdgisimfb.html

[T36] Lua：函数
来源：http://hz.zycfv.cn/gtacexdbav.html

function add(a, b) return a + b end
来源：http://hz.cucudq.cn/gtuvmgilto.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gtjomlvyjy.html

"a" .. "b"
来源：http://hz.hfpthk.cn/gtgxezvriz.html

[T38] Lua：条件
来源：http://hz.jinghuilouyu.cn/gtynomlvgs.html

if x > 0 then print("正") end
来源：http://hz.sysykeji.top/gtbstbgpzc.html

[T39] Lua：模式匹配
来源：http://hz.316326.xyz/gtrtrsgdlo.html

string.find(s, "%d+")
来源：http://hz.jlsjyb.cn/gtnlbkxzca.html

[T40] Lua：元表
来源：http://hz.cqqwz.cn/gtswmznceo.html

setmetatable({}, { __index = base })
来源：http://hz.hywenlv.cn/gtlpxbvsvk.html

[T41] Perl：Hello World
来源：http://hz.hongshengwenyu.top/gtxitrwqzt.html

print "Hello\n";
来源：http://hz.jiagoushi.top/gtsrtgzuft.html

[T42] Perl：变量类型
来源：http://hz.sxryk.cn/gtrtqfnogn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guannengcc.top/gtlrgszdhp.html

[T43] Perl：字符串插值
来源：http://hz.yuanzhike.top/gtwzkxivms.html

"值: $a"
来源：http://hz.hfpthk.cn/gtcqofsbjx.html

[T44] Perl：条件
来源：http://hz.hongshengwenyu.top/gtigevthzy.html

if ($a > 0) { print "正"; }
来源：http://hz.nwbrower.top/gtcjmhyfsn.html

[T45] Perl：数组遍历
来源：http://hz.hnqzz.top/gtdcagpwpa.html

for my $x (@arr) { print $x; }
来源：http://hz.zhongyouzk.top/gthzwbreni.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gthglafjqp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hfpthk.cn/gticwfassy.html

[T47] Perl：正则捕获
来源：http://hz.jinyuanbaomall.cn/gtdpwsniaz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yongpay.top/gtctxcetwj.html

[T48] Perl：正则替换
来源：http://hz.xylfe.cn/gtskxrraqq.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtfoidscji.html

[T49] Perl：函数
来源：http://hz.hysaishi.cn/gtzaulytaj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jqgfzy.top/gtjuhkoblg.html

[T50] Perl：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtqlyhabhe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xziqi.cn/gtbezcjerd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hongshengwenyu.top/gtwizioutt.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtzbybomhg.html

println("Hello")
来源：http://hz.hysaishi.cn/gtpholqraz.html

[T52] Scala：变量
来源：http://hz.cdnleiting.top/gtgspdudie.html

val a = 1;  var b = 2
来源：http://hz.meibo888.top/gtyichmrhs.html

[T53] Scala：字符串插值
来源：http://hz.dianchejie.cn/gtkkxbxknw.html

s"值: $b"
来源：http://hz.52xcode.cn/gtqkebdiph.html

[T54] Scala：集合映射
来源：http://hz.aizwys.cn/gtdmagxxsl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhengqikj.top/gtrnjppzbj.html

[T55] Scala：集合过滤
来源：http://hz.meibo888.top/gtizancatm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nanxuanxn.top/gtuzdlempw.html

[T56] Scala：样例类
来源：http://hz.hammf.cn/gtkhplytss.html

case class User(name: String, age: Int)
来源：http://hz.hnqzz.top/gtbbutqgvt.html

[T57] Scala：模式匹配
来源：http://hz.xylfe.cn/gtzhjgdrfx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.52xcode.cn/gtbzyjcdkg.html

[T58] Scala：函数定义
来源：http://hz.snrcjt.cn/gtmtnnnslo.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yonumen.top/gtdflxzczj.html

[T59] Scala：循环
来源：http://hz.fengsongda.top/gtlillqggp.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtwngvlhrm.html

[T60] Scala：折叠
来源：http://hz.chenjidiqi.icu/gtqtapmybc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aizwys.cn/gtlhvnugxm.html

================================================================================
来源：http://hz.yonumen.top/gtufpthjcr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtaltvvmcb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdhnalpxh.html

[U01] Py：创建虚拟环境
来源：http://hz.jinqigfzy.top/gtqlshdzgx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.svipenyu.cn/gtplxobsju.html

[U02] Py：导出 / 安装依赖
来源：http://hz.andypj.xyz/gtamqwkbpw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shangyingyoupin.top/gtowvpnlim.html

[U03] Py：加载 .env 配置
来源：http://hz.yuxming.cn/gthtrpnbbz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhongyouzk.top/gtqtzvgbfv.html

[U04] Py：变量调试打印
来源：http://hz.jqgufenzy.top/gtgvqhokia.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tian-w.cn/gtvnerzqhf.html

[U05] Py：列表去重且保序
来源：http://hz.ybcxt.top/gtbzfojcis.html

list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtzayjmcgp.html

[U06] Py：合并两个字典
来源：http://hz.xinyue.icu/gtujiwbean.html

{**a, **b}
来源：http://hz.pycfn.com/gtpwycjqsx.html

[U07] Py：反转字典键值
来源：http://hz.iojbl.cn/gtcwkfuxsx.html

{v: k for k, v in d.items()}
来源：http://hz.yonumen.top/gtfegoxsbc.html

[U08] Py：展平二维列表
来源：http://hz.zhongyouzk.top/gtnksitylw.html

[y for x in nested for y in x]
来源：http://hz.ybcxt.top/gtxnsvjjxh.html

[U09] Py：字典取最大值的键
来源：http://hz.dianchejie.cn/gtetdfjqhc.html

max(d, key=d.get)
来源：http://hz.guowangkeji.top/gtmwppvmyn.html

[U10] Py：按值排序字典
来源：http://hz.gaohongyu789.top/gteaiblmes.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhixingplan.top/gtitgdeojy.html

[U11] Py：生成器表达式
来源：http://hz.yuanzhike.top/gtkzujnepq.html

(x * 2 for x in arr)
来源：http://hz.fzhhl.top/gtnxbixymf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxinkj.top/gtsbymorfz.html

Counter(arr).most_common(3)
来源：http://hz.ydjk.org.cn/gtadywvzva.html

[U13] Py：固定长度队列
来源：http://hz.birdmap.top/gtfrlmzwxb.html

deque(maxlen=10)
来源：http://hz.shanyushiyangtech.top/gteixfotyz.html

[U14] Py：分组收集到列表
来源：http://hz.jinyuanbaomall.cn/gtikarmbue.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtrcfibutk.html

[U15] Py：高精度计时
来源：http://hz.chenlongwang.top/gtjdrjyszf.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtaowdwkct.html

[U16] Py：命令行参数解析
来源：http://hz.dianchejie.cn/gtrimixsbd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigufen.top/gtjvzlblcd.html

[U17] Py：初始化日志
来源：http://hz.shangyingyoupin.top/gtdzrtbcvv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.bjfxy.top/gttsstfdtl.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtehrebskh.html

pat = re.compile(r"\d+")
来源：http://hz.nanxuanxn.top/gtdcehpwdc.html

[U19] Py：正则替换带回调
来源：http://hz.mhx1999.top/gtsvckcxkp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.havefunace.top/gtyiruoxxk.html

[U20] Py：缓存函数结果
来源：http://hz.zycfv.cn/gtoluwjunc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.cashguo.top/gttvskghce.html

[U21] Py：自定义上下文管理器
来源：http://hz.52xcode.cn/gtpbztskfq.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtpjmoxgwg.html

[U22] Py：矩阵转置
来源：http://hz.dianchejie.cn/gtsvsgikar.html

list(zip(*m))
来源：http://hz.cdnleiting.top/gtyhnjzihl.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gttbcwdjzv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.kuanghao11.cn/gtqgbnjism.html

[U24] Py：路径操作
来源：http://hz.zhiwuduotai.top/gtzpzljkwn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ydzc1.top/gtgtrkhrzk.html

[U25] Py：CSV 按字典读
来源：http://hz.316326.xyz/gtzodnleqb.html

csv.DictReader(f)
来源：http://hz.fengsongda.top/gtrgnswnup.html

[U26] Py：并发下载
来源：http://hz.xziqi.cn/gtsbsrhoci.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ywan-chungtsiang.top/gtxunprbon.html

[U27] Py：异步 HTTP
来源：http://hz.ydzc1.top/gtecsozmwv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.havefunace.top/gtcfibhevw.html

[U28] Py：类型别名
来源：http://hz.zhaomingkeji.xyz/gtoxmbaetl.html

UserId = int
来源：http://hz.zhoulong.xyz/gttqsalrtx.html

[U29] Py：属性校验
来源：http://hz.0kj1m.cn/gtrparrkxi.html

@property 与 @x.setter 配合
来源：http://hz.chenzaomai.com/gtimzbvmdb.html

[U30] Py：数据类
来源：http://hz.gaohongyu789.top/gtufprrxws.html

@dataclass(slots=True)
来源：http://hz.yj20258.top/gtwslgetbp.html

[U31] Py：单测
来源：http://hz.316326.xyz/gtkqyhkjaa.html

python -m pytest -q
来源：http://hz.zycfv.cn/gtawpjbvto.html

[U32] Py：代码格式化
来源：http://hz.yangfankeji.com/gtwefhfszw.html

ruff format . && ruff check --fix .
来源：http://hz.ivvv.top/gtsaiftvfq.html

[U33] Py：打包发布
来源：http://hz.52xcode.cn/gtiwpargcx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj20258.top/gtqxqdjslz.html

[U34] Py：判断编码
来源：http://hz.yonumen.top/gtpxmbofbs.html

chardet.detect(raw)
来源：http://hz.feifeiyinyue.top/gtvqomjtnx.html

[U35] Py：发送邮件
来源：http://hz.c1oappe.top/gtaqfcyviq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.haohaochexian.top/gtsoiblypi.html

[U36] Py：定时任务
来源：http://hz.zdqjudy.top/gteiyggopq.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuxming.cn/gtbtopgwcd.html

[U37] Py：读写 Excel
来源：http://hz.hnqzz.top/gtjghrjukl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yuanzhike.top/gtahukijau.html

[U38] Py：获取脚本所在目录
来源：http://hz.yueranfly.top/gtahcdpttp.html

Path(__file__).resolve().parent
来源：http://hz.feifeiyinyue.top/gtmjjtysvz.html

[U39] Py：判断是否在交互环境
来源：http://hz.nwbrower.top/gtaeluwecp.html

sys.stdout.isatty()
来源：http://hz.dianchejie.cn/gtdczrtqes.html

[U40] Py：打印到标准错误
来源：http://hz.zhengqikj.top/gtbvlujauj.html

print("err", file=sys.stderr)
来源：http://hz.shzxlz.cn/gtonuiqklx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zdqjudy.top/gtlaijrbzy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hongshengwenyu.top/gtesgzkxdc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenlongwang.top/gtxbeobvyu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.mhx1999.top/gtqwygneyv.html

[U43] PHP：声明命名空间
来源：http://hz.mhx1999.top/gthhfplfue.html

namespace App\Http;
来源：http://hz.hysaishi.cn/gtrmsfacav.html

[U44] PHP：开启严格类型
来源：http://hz.xylfe.cn/gthjxcplko.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtpcrnpsax.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hfpthk.cn/gtgtxnxaag.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtgnjvybva.html

[U46] PHP：可空类型
来源：http://hz.zhoulong.xyz/gtalolyurr.html

?string $name = null
来源：http://hz.yj20258888.top/gtpcxeudzd.html

[U47] PHP：联合类型
来源：http://hz.nanxinkj.top/gtkhmypmwm.html

int|string $id
来源：http://hz.pengpengdd.cyou/gttdewoyfc.html

[U48] PHP：纯枚举
来源：http://hz.aizwys.cn/gtooghbuwr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aizwys.cn/gtsqfzvtol.html

[U49] PHP：只读属性
来源：http://hz.yueranfly.top/gtioyjzztb.html

public readonly string $name
来源：http://hz.zhongyouzk.top/gtdhcdegmm.html

[U50] PHP：构造器属性提升
来源：http://hz.fengsongda.top/gtznqsdght.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gtygfznotk.html

[U51] PHP：数组解构
来源：http://hz.wangdashe.top/gtymqfpjbi.html

[$a, $b] = $arr;
来源：http://hz.yj20258.top/gtdjthrbpg.html

[U52] PHP：箭头函数
来源：http://hz.xinyue.icu/gtuzdrfcmu.html

$double = fn($x) => $x * 2;
来源：http://hz.ppjwa.cn/gtsfqrttsx.html

[U53] PHP：空合并运算符
来源：http://hz.haohaochexian.top/gtbhvsxkim.html

$v = $a ?? $b ?? "default";
来源：http://hz.jiagoushi.top/gtwiosrkjh.html

[U54] PHP：空安全调用
来源：http://hz.feifeiyinyue.top/gtjpnvxeyl.html

$obj?->method()
来源：http://hz.zycfv.cn/gtvvnzfead.html

[U55] PHP：match 表达式
来源：http://hz.iojbl.cn/gtfqmhauab.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gaohongyu789.top/gtbrvhpkws.html

[U56] PHP：命名参数
来源：http://hz.sweek.top/gtuioxslum.html

f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtuuaginlu.html

[U57] PHP：字符串插值
来源：http://hz.hongshengwenyu.top/gtxjqgeees.html

"值: {$a}"
来源：http://hz.yonumen.top/gtihfwkpvd.html

[U58] PHP：数组三件套
来源：http://hz.jlsjyb.cn/gtsvfoupql.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yanxiufei.cn/gtbfvnqsls.html

[U59] PHP：自定义排序
来源：http://hz.snrcjt.cn/gtldmbapcz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtdfyzvbdi.html

[U60] PHP：JSON 编解码
来源：http://hz.tian-w.cn/gtfsbebucm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tianlin.xyz/gttgdsdqzv.html

[U61] PHP：正则
来源：http://hz.mhx1999.top/gteovsllkv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtkxchbedu.html

[U62] PHP：日期对象
来源：http://hz.shanyushiyangkeji.top/gthpmuxtad.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ybcxt.top/gtdgdlgpgw.html

[U63] PHP：文件读写
来源：http://hz.nanxuanxn.top/gttxxvrnfv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.0kj1m.cn/gtbvygrpaw.html

[U64] PHP：目录遍历
来源：http://hz.gotoacloud.top/gtwtekvkob.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daxiang520.top/gtwbbhxana.html

[U65] PHP：会话
来源：http://hz.iojbl.cn/gtlbcsatsz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zdqjudy.top/gttlygdxua.html

[U66] PHP：设置 Cookie
来源：http://hz.feifeiyinyue.top/gtvwpybucb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.bjfxy.top/gtfoeaxbhn.html

[U67] PHP：处理文件上传
来源：http://hz.aibaodan.cn/gtaytmgtbl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ppjwa.cn/gtjzbibuiu.html

[U68] PHP：PDO 连接
来源：http://hz.zhoulong.xyz/gtvudhuxkm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigufen.top/gttkjjjxxc.html

[U69] PHP：PDO 预处理
来源：http://hz.pycfn.com/gtlelfytvq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xziqi.cn/gtwphdkpmx.html

[U70] PHP：PDO 事务
来源：http://hz.ehwqpu.com/gtcmltfbgx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cheryme.top/gtmgdvkrwr.html

[U71] PHP：抛出异常
来源：http://hz.ehwqpu.com/gtnommjjfl.html

throw new RuntimeException("失败", 500);
来源：http://hz.cucudq.cn/gtpmfzmshk.html

[U72] PHP：写错误日志
来源：http://hz.daxiang520.top/gtwlkehciz.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhaomingkeji.xyz/gtoowaptqr.html

[U73] PHP：读取 ini 配置
来源：http://hz.dianchejie.cn/gtemorybck.html

parse_ini_file("config.ini", true)
来源：http://hz.aibaodan.cn/gtcmwqxslf.html

[U74] PHP：读取环境变量
来源：http://hz.hammf.cn/gtgtmnlyac.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yueranfly.top/gtnstrqomo.html


<!-- 参考信息 -->