代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.hysaishi.cn/gtpculnjpw.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtwrynmwpf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ivvv.top/gtrkvfmlva.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtlsjbmpqq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jlsjyb.cn/gtcoukdpwf.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtwdglazqt.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gtanwvcxcr.html

[S52] C++：const 与 noexcept
来源：http://hz.yanxiufei.cn/gtdjocgryk.html

int size() const noexcept { return n_; }
来源：http://hz.aibaodan.cn/gtuuhwywlq.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gtvmimmitt.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtbspbzqhk.html

[S54] C++：异常处理
来源：http://hz.yj20258888.top/gtlocaqijx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.quarkkingdee.top/gtaqjextrn.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtktdjanjl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtawmimsif.html

[S56] C++：optional
来源：http://hz.dianchejie.cn/gtznlwiuhn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xuetiantiany.cn/gttaprximg.html

[S57] C++：编译期常量
来源：http://hz.gotoacloud.top/gtlashhgue.html

constexpr int N = 10;
来源：http://hz.gogol.net.cn/gtiovdaosa.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gtaodvftwl.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtoohlioeg.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gtunbwzxwe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gzhubu.top/gtzkyzwaoa.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtasvqfqab.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtwkiwrlxo.html

================================================================================
来源：http://hz.fengsongda.top/gtqpeoakxc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pengpengdd.cyou/gtehintvrf.html

================================================================================
来源：http://hz.iojbl.cn/gtspreajiq.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gtendjvbfy.html

println("Hello")
来源：http://hz.dashuyun.cn/gtfdagfhua.html

[T02] Kotlin：变量
来源：http://hz.yuxming.cn/gtmnqjmfoj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.svipenyu.cn/gtiwuxjerr.html

[T03] Kotlin：字符串模板
来源：http://hz.pengpengdd.cyou/gtxblqwydp.html

"值: $b"
来源：http://hz.andypj.xyz/gtpgheqqeu.html

[T04] Kotlin：空安全
来源：http://hz.kuanghao11.cn/gtcwhlkqgw.html

val n: String? = null;  n?.length
来源：http://hz.birdmap.top/gtaacnwbqf.html

[T05] Kotlin：when 表达式
来源：http://hz.gzhubu.top/gtuhzcptvf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtickuffvr.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtwcgfcplv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinyuanbaomall.cn/gtaqtwcyfv.html

[T07] Kotlin：集合过滤
来源：http://hz.kuanghao11.cn/gtwpyhivko.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtsgnwlfno.html

[T08] Kotlin：数据类
来源：http://hz.bjfxy.top/gtpzpklwmp.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gtwgjnmkjw.html

[T09] Kotlin：扩展函数
来源：http://hz.birdmap.top/gthhaerxdw.html

fun String.exclaim() = this + "!"
来源：http://hz.havefunace.top/gtjayydolo.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gthdbdmyga.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtwaxfbrzg.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangkeji.top/gtwzjmheen.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtqcznxcsz.html

[T12] Kotlin：解构声明
来源：http://hz.iojbl.cn/gtwpnufzbe.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtdpznzuip.html

[T13] Kotlin：只读 Map
来源：http://hz.cashguo.top/gtxggumlyr.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gtfxfhjkrh.html

[T14] Kotlin：循环
来源：http://hz.fzhhl.top/gtugltunec.html

for (i in 1..10) println(i)
来源：http://hz.yvedp.cn/gtanpydozm.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtkfpvshor.html

interface Shape { fun area(): Double }
来源：http://hz.sweek.top/gtinqaixem.html

[T16] Swift：Hello World
来源：http://hz.sweek.top/gtwktnyazc.html

print("Hello")
来源：http://hz.tian-w.cn/gtmifmsxmc.html

[T17] Swift：变量与常量
来源：http://hz.jinghuilouyu.cn/gthhnpkyex.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gtamuqpbho.html

[T18] Swift：字符串插值
来源：http://hz.pycfn.com/gtrtbczfha.html

"值: \(b)"
来源：http://hz.zdqjudy.top/gtyewlcwdz.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtxgyskywp.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtvneegzky.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtiqmmlelp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtiwlbqiaq.html

[T21] Swift：遍历
来源：http://hz.ydzc1.top/gtaiuomgsh.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gtpvfapdft.html

[T22] Swift：字典
来源：http://hz.pengpengdd.cyou/gtbrlamegm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.316326.xyz/gtffktowpz.html

[T23] Swift：函数
来源：http://hz.shangyingyoupin.top/gtuplpfmgv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenjidiqi.icu/gtvjvuxvjr.html

[T24] Swift：闭包
来源：http://hz.hnxiangtu.top/gtjrddxzwp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daxiang520.top/gtqceqlgju.html

[T25] Swift：结构体
来源：http://hz.smart0.xyz/gtbbqgykyv.html

struct P { var x: Int }
来源：http://hz.yj20258.top/gtihqmlmsg.html

[T26] Swift：类与重写
来源：http://hz.nanxinkj.top/gtjaduxccz.html

class A: Base { override func f() {} }
来源：http://hz.wangshuangyany.cn/gtuhowqwer.html

[T27] Swift：错误处理
来源：http://hz.chenjidiqi.icu/gtdeuctvho.html

do { try f() } catch { print(error) }
来源：http://hz.yj20258888.top/gtoaorwrom.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtkyucyaha.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtmqncnrma.html

[T29] Swift：guard 提前返回
来源：http://hz.zhixingplan.top/gtiqygvfib.html

guard let x = opt else { return }
来源：http://hz.jinqigufen.top/gthqenkkwa.html

[T30] Swift：协议
来源：http://hz.gzhubu.top/gtimojdxbu.html

protocol Shape { func area() -> Double }
来源：http://hz.yj202588.top/gtspktagix.html

[T31] Lua：Hello World
来源：http://hz.xingfuxueyuan.xyz/gthwikfocz.html

print("Hello")
来源：http://hz.haohaochexian.top/gtkwrwmbtg.html

[T32] Lua：局部变量
来源：http://hz.zhixingplan.top/gtmcnfrmjo.html

local a = 1
来源：http://hz.ywan-chungtsiang.top/gtgpdqegyo.html

[T33] Lua：表（数组）
来源：http://hz.ydjk.org.cn/gtzbvymlxk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gogol.net.cn/gtarekgbky.html

[T34] Lua：遍历表
来源：http://hz.ywan-chungtsiang.top/gthoqugoqg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.316326.xyz/gtgwvzotxb.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gtwbllcaty.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hywenlv.cn/gtemdvrdsk.html

[T36] Lua：函数
来源：http://hz.zhongyouzk.top/gtvkrmokwc.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtzvlpxijd.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtqcmsgqzi.html

"a" .. "b"
来源：http://hz.ybcxt.top/gtfdaooqle.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gttdmbyywf.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtgxrjulcj.html

[T39] Lua：模式匹配
来源：http://hz.sxryk.cn/gtaynhphxx.html

string.find(s, "%d+")
来源：http://hz.zycfv.cn/gtmnjlbiop.html

[T40] Lua：元表
来源：http://hz.haohaochexian.top/gtpwlnyirg.html

setmetatable({}, { __index = base })
来源：http://hz.chenzaomai.com/gtfyjztush.html

[T41] Perl：Hello World
来源：http://hz.zhongyouzk.top/gtvuadboms.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gtcrxedmxo.html

[T42] Perl：变量类型
来源：http://hz.zhoulong.xyz/gticwbnsrp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yongpay.top/gtbsvkfbcr.html

[T43] Perl：字符串插值
来源：http://hz.hfpthk.cn/gtyvvsinhs.html

"值: $a"
来源：http://hz.ppjwa.cn/gtjusmqniz.html

[T44] Perl：条件
来源：http://hz.fengsongda.top/gtuukqrlpe.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtevqzdxvt.html

[T45] Perl：数组遍历
来源：http://hz.havefunace.top/gtdkcbaxcy.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigufen.top/gtnpfyzrvq.html

[T46] Perl：哈希操作
来源：http://hz.yj202588.top/gtbjzxwfzw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.pengpengdd.cyou/gtfmzsnczq.html

[T47] Perl：正则捕获
来源：http://hz.zhongyouzk.top/gtygmtwlum.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shzxlz.cn/gtgnwfhour.html

[T48] Perl：正则替换
来源：http://hz.xuanzx.com/gtfnuanrij.html

$s =~ s/old/new/g;
来源：http://hz.zhongyouzk.top/gtcksnmwfe.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gtowmqngkg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sweek.top/gthvmukpxa.html

[T50] Perl：逐行读文件
来源：http://hz.ivvv.top/gtydgavudm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenzaomai.com/gtvuxifimh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sysykeji.top/gtepehcymj.html

[T51] Scala：Hello World
来源：http://hz.zhengqikj.top/gtaeczftcg.html

println("Hello")
来源：http://hz.chenzaomai.com/gtkkzuepow.html

[T52] Scala：变量
来源：http://hz.c1oappe.top/gtvorqzsnm.html

val a = 1;  var b = 2
来源：http://hz.redwolf501.top/gtclebctrd.html

[T53] Scala：字符串插值
来源：http://hz.daria6918.cn/gtrjejkadw.html

s"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtqvxhovok.html

[T54] Scala：集合映射
来源：http://hz.haohaochexian.top/gtsmbunwow.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtzdtpfxnk.html

[T55] Scala：集合过滤
来源：http://hz.sufxvd.cn/gtowokbpaz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.guowangkeji.top/gtwskadonh.html

[T56] Scala：样例类
来源：http://hz.jinghuilouyu.cn/gtanokaise.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gtjkowmkvf.html

[T57] Scala：模式匹配
来源：http://hz.yueranfly.top/gtpllthesu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yvedp.cn/gtwcxqqacr.html

[T58] Scala：函数定义
来源：http://hz.gaohongyu789.top/gtocofmdgz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtjgphskab.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gtmmtmloxs.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtfjuqzrmz.html

[T60] Scala：折叠
来源：http://hz.ehwqpu.com/gtytpyqtah.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hammf.cn/gtlnfyfeho.html

================================================================================
来源：http://hz.ppjwa.cn/gtuwsznoke.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtfxtpoiqx.html

================================================================================
来源：http://hz.9152youxi.cn/gtltvclszq.html

[U01] Py：创建虚拟环境
来源：http://hz.zycfv.cn/gtyqjlrxpy.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ydzc1.top/gtpkhbdtih.html

[U02] Py：导出 / 安装依赖
来源：http://hz.meibo888.top/gtaddaxwvs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yanxiufei.cn/gtulfbbbpq.html

[U03] Py：加载 .env 配置
来源：http://hz.chenlongwang.top/gtkfpgfiks.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tanke756.top/gtmqhpdkyb.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtdbxojwsh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guowangkeji.top/gtvaqsyqui.html

[U05] Py：列表去重且保序
来源：http://hz.hnxiangtu.top/gtzxtcnrml.html

list(dict.fromkeys(arr))
来源：http://hz.jinyuanbaomall.cn/gtegfpbcwx.html

[U06] Py：合并两个字典
来源：http://hz.yj20258888.top/gtddijsjzr.html

{**a, **b}
来源：http://hz.jqgfzy.top/gteydwcnke.html

[U07] Py：反转字典键值
来源：http://hz.gaohongyu789.top/gtmwpcrwxn.html

{v: k for k, v in d.items()}
来源：http://hz.ybcxt.top/gtdphwjrub.html

[U08] Py：展平二维列表
来源：http://hz.0kj1m.cn/gtqkurbhzr.html

[y for x in nested for y in x]
来源：http://hz.gzhubu.top/gtshkpxgfk.html

[U09] Py：字典取最大值的键
来源：http://hz.jyoumei.cn/gtvmfwlusf.html

max(d, key=d.get)
来源：http://hz.cdnleiting.top/gtasfhhkcv.html

[U10] Py：按值排序字典
来源：http://hz.jyoumei.cn/gtxwrjkzzl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cheryme.top/gtnfhnhrxm.html

[U11] Py：生成器表达式
来源：http://hz.xingfuxueyuan.xyz/gtvczdfuwa.html

(x * 2 for x in arr)
来源：http://hz.hywenlv.cn/gthnjhysnp.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.redwolf501.top/gtjbbxynmj.html

Counter(arr).most_common(3)
来源：http://hz.9152youxi.cn/gtbrwlcuue.html

[U13] Py：固定长度队列
来源：http://hz.yj20258888.top/gtwknxtues.html

deque(maxlen=10)
来源：http://hz.52xcode.cn/gtolettdvf.html

[U14] Py：分组收集到列表
来源：http://hz.nanxuanxn.top/gtnhjrfudp.html

defaultdict(list)
来源：http://hz.cucudq.cn/gthexchyev.html

[U15] Py：高精度计时
来源：http://hz.shanyushiyangkeji.top/gtzlvqtnnq.html

t = time.perf_counter()
来源：http://hz.0kj1m.cn/gtmmnwkqxl.html

[U16] Py：命令行参数解析
来源：http://hz.9152youxi.cn/gtmbutfzom.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj202588.top/gtikbvvbjf.html

[U17] Py：初始化日志
来源：http://hz.gzhubu.top/gtjllzycpf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guannengcc.top/gtuycgereb.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtiwxjdtes.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gthhdakhpx.html

[U19] Py：正则替换带回调
来源：http://hz.mhx1999.top/gthhmktvew.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinghuilouyu.cn/gtplahwrse.html

[U20] Py：缓存函数结果
来源：http://hz.vqdsnc.cn/gtdxlyhptb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.9152youxi.cn/gtfyfzuhhs.html

[U21] Py：自定义上下文管理器
来源：http://hz.snrcjt.cn/gtuziudfqk.html

@contextlib.contextmanager
来源：http://hz.aibaodan.cn/gtgyjbqisy.html

[U22] Py：矩阵转置
来源：http://hz.xuetiantiany.cn/gtksuhzqrt.html

list(zip(*m))
来源：http://hz.wangshuangyany.cn/gtpxnuoybl.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtxnuqsooc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yangfankeji.com/gtuonsjeqm.html

[U24] Py：路径操作
来源：http://hz.hfpthk.cn/gtrxiuwtqx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.0kj1m.cn/gtoimlnxjw.html

[U25] Py：CSV 按字典读
来源：http://hz.quarkkingdee.top/gtewnivsjg.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtfyggqiup.html

[U26] Py：并发下载
来源：http://hz.dashuyun.cn/gtzrrsjebt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daxiang520.top/gttzgovapz.html

[U27] Py：异步 HTTP
来源：http://hz.c1oappe.top/gtwdjfvxng.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shuidangran.top/gtegkamagb.html

[U28] Py：类型别名
来源：http://hz.birdmap.top/gtjtfmusym.html

UserId = int
来源：http://hz.xinyue.icu/gtsqyflbvy.html

[U29] Py：属性校验
来源：http://hz.jyoumei.cn/gtgnacdunu.html

@property 与 @x.setter 配合
来源：http://hz.yanxiufei.cn/gteaalmmpg.html

[U30] Py：数据类
来源：http://hz.zhiwuduotai.top/gtduzsfpli.html

@dataclass(slots=True)
来源：http://hz.jyoumei.cn/gtxasofwqg.html

[U31] Py：单测
来源：http://hz.fzhhl.top/gthipwsodw.html

python -m pytest -q
来源：http://hz.yvedp.cn/gtunvqztsk.html

[U32] Py：代码格式化
来源：http://hz.nanxinkj.top/gthehdtfwk.html

ruff format . && ruff check --fix .
来源：http://hz.jyoumei.cn/gtajahvagt.html

[U33] Py：打包发布
来源：http://hz.feifeiyinyue.top/gtmpzixttx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.aibaodan.cn/gtkdsgpnmg.html

[U34] Py：判断编码
来源：http://hz.birdmap.top/gtwpuachym.html

chardet.detect(raw)
来源：http://hz.hfpthk.cn/gtznzyfabr.html

[U35] Py：发送邮件
来源：http://hz.hfpthk.cn/gtgcarkjjp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cqqwz.cn/gtbvmbsipa.html

[U36] Py：定时任务
来源：http://hz.wangdashe.top/gtotkzgkop.html

schedule.every(10).minutes.do(job)
来源：http://hz.kuanghao11.cn/gtfbgqrnnz.html

[U37] Py：读写 Excel
来源：http://hz.sweek.top/gtbtdsreuv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nwbrower.top/gtnnijplkd.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhijiandao.cn/gtjqotqsyy.html

Path(__file__).resolve().parent
来源：http://hz.sxryk.cn/gtzdhsxexq.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhaomingkeji.xyz/gthdauazxb.html

sys.stdout.isatty()
来源：http://hz.ydzc1.top/gtnhujpngc.html

[U40] Py：打印到标准错误
来源：http://hz.yj20258888.top/gtenmiduwq.html

print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtjutpwnbf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hywenlv.cn/gtprobfquh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.feifeiyinyue.top/gtdhjlwjhs.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.316326.xyz/gtajycklev.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shangyingyoupin.top/gtffbbkrjj.html

[U43] PHP：声明命名空间
来源：http://hz.shzxlz.cn/gtrudxtmui.html

namespace App\Http;
来源：http://hz.pengpengdd.cyou/gtbksvmibi.html

[U44] PHP：开启严格类型
来源：http://hz.shzxlz.cn/gtznuzwush.html

declare(strict_types=1);
来源：http://hz.ydjk.org.cn/gtvusekvxk.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tianlin.xyz/gtgmdwmoar.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtorhqeccx.html

[U46] PHP：可空类型
来源：http://hz.zycfv.cn/gtowgyijue.html

?string $name = null
来源：http://hz.kuanghao11.cn/gthcmpblir.html

[U47] PHP：联合类型
来源：http://hz.wangdashe.top/gtbvppbchw.html

int|string $id
来源：http://hz.meibo888.top/gtikovgbdz.html

[U48] PHP：纯枚举
来源：http://hz.cucudq.cn/gtmnjdbved.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xylfe.cn/gtrrtzodjw.html

[U49] PHP：只读属性
来源：http://hz.quarkkingdee.top/gtokyydnct.html

public readonly string $name
来源：http://hz.xuetiantiany.cn/gtvwdkxfbr.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtvyjrdrpf.html

public function __construct(private int $id) {}
来源：http://hz.bjfxy.top/gtehytrbma.html

[U51] PHP：数组解构
来源：http://hz.xylfe.cn/gtkmdtftem.html

[$a, $b] = $arr;
来源：http://hz.snrcjt.cn/gtwfslzyfi.html

[U52] PHP：箭头函数
来源：http://hz.fzhhl.top/gttyazqzar.html

$double = fn($x) => $x * 2;
来源：http://hz.yj20258888.top/gtfsqmacfc.html

[U53] PHP：空合并运算符
来源：http://hz.yangfankeji.com/gtzwaqmxvv.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangdashe.top/gtpxibahab.html

[U54] PHP：空安全调用
来源：http://hz.ydjk.org.cn/gtiixvgkyi.html

$obj?->method()
来源：http://hz.9152youxi.cn/gtidzxlesr.html

[U55] PHP：match 表达式
来源：http://hz.jyoumei.cn/gtixqalybu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhongyouzk.top/gtjdfkcsch.html

[U56] PHP：命名参数
来源：http://hz.ywan-chungtsiang.top/gtqfwdkwnv.html

f(a: 1, b: 2)
来源：http://hz.dianchejie.cn/gtgzvxhnlg.html

[U57] PHP：字符串插值
来源：http://hz.chenzaomai.com/gtgtonyquu.html

"值: {$a}"
来源：http://hz.yuxming.cn/gtuwuieifc.html

[U58] PHP：数组三件套
来源：http://hz.gogol.net.cn/gtchevsast.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.meibo888.top/gtaitmbbua.html

[U59] PHP：自定义排序
来源：http://hz.ehwqpu.com/gtjbojfcxq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtqqwxhuzw.html

[U60] PHP：JSON 编解码
来源：http://hz.wangshuangyany.cn/gtavuzmjso.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinqigfzy.top/gtubpbfldw.html

[U61] PHP：正则
来源：http://hz.cheryme.top/gtpuicqlzt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtsbinrgdr.html

[U62] PHP：日期对象
来源：http://hz.gzhubu.top/gtpmipneai.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ehwqpu.com/gtxlyxgxob.html

[U63] PHP：文件读写
来源：http://hz.shangyingyoupin.top/gtqzhpujlp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hysaishi.cn/gthyekvclc.html

[U64] PHP：目录遍历
来源：http://hz.chenjidiqi.icu/gtnqthevfl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.bjfxy.top/gtyvepubyk.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtcpblwhzt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.zdqjudy.top/gtxhayhyzw.html

[U66] PHP：设置 Cookie
来源：http://hz.zhixingplan.top/gtnoitftrp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.dashuyun.cn/gtceljibdx.html

[U67] PHP：处理文件上传
来源：http://hz.zhengqikj.top/gtrjtjzxqe.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yuxming.cn/gtduzenpib.html

[U68] PHP：PDO 连接
来源：http://hz.nwbrower.top/gtzjlaicbp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shanyushiyangtech.top/gtvgahzkyf.html

[U69] PHP：PDO 预处理
来源：http://hz.ybcxt.top/gtwokitwps.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gaohongyu789.top/gtvwtqsabp.html

[U70] PHP：PDO 事务
来源：http://hz.ivvv.top/gtilghfqxk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.smart0.xyz/gtrqhfinhk.html

[U71] PHP：抛出异常
来源：http://hz.aizwys.cn/gtabwlweyx.html

throw new RuntimeException("失败", 500);
来源：http://hz.yj20258888.top/gtwofchbng.html

[U72] PHP：写错误日志
来源：http://hz.cdnleiting.top/gtjkfzyoui.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hongshengwenyu.top/gtynvsxtpm.html

[U73] PHP：读取 ini 配置
来源：http://hz.cashguo.top/gtjiutfwqu.html

parse_ini_file("config.ini", true)
来源：http://hz.birdmap.top/gtbzubrhsw.html

[U74] PHP：读取环境变量
来源：http://hz.tian-w.cn/gtecdewzqd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.gzhubu.top/gtlnrvrdwz.html


<!-- 参考信息 -->