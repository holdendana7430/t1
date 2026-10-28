代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuxming.cn/gtylxsslzl.html

[S51] C++：显式类型转换
来源：http://hz.andypj.xyz/gtrnwwutdp.html

static_cast<double>(a) / b
来源：http://hz.zhijiandao.cn/gtbvlxrsiq.html

[S52] C++：const 与 noexcept
来源：http://hz.zhijiandao.cn/gtjszhkjdg.html

int size() const noexcept { return n_; }
来源：http://hz.zhaomingkeji.xyz/gtzumfzlsn.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtlmjpybgh.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtrdsdjlzw.html

[S54] C++：异常处理
来源：http://hz.yuxming.cn/gtsowumclz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tian-w.cn/gtrwkqnxcb.html

[S55] C++：结构化绑定
来源：http://hz.shangyingyoupin.top/gtgsmuhpvl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.c1oappe.top/gtekaebssw.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gtgzhphane.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtbncjqzir.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtdhhfoplg.html

constexpr int N = 10;
来源：http://hz.smart0.xyz/gtzxdbehgh.html

[S58] C++：命名空间
来源：http://hz.ywan-chungtsiang.top/gtxrxeuyuz.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtpgvowhfk.html

[S59] C++：静态断言
来源：http://hz.andypj.xyz/gtmbgcmmxw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.vqdsnc.cn/gthcxwzaxm.html

[S60] C++：遍历并删除元素
来源：http://hz.9152youxi.cn/gtfqobngdi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gteartoukh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdtfbdmlq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtgppcdpzj.html

================================================================================
来源：http://hz.gotoacloud.top/gtaugqrkhd.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gtubzkgxjb.html

println("Hello")
来源：http://hz.andypj.xyz/gtguxhgzvn.html

[T02] Kotlin：变量
来源：http://hz.wangshuangyany.cn/gtbvqxdeia.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenjidiqi.icu/gtorabhvzj.html

[T03] Kotlin：字符串模板
来源：http://hz.tanke756.top/gtvuvebfpn.html

"值: $b"
来源：http://hz.yvedp.cn/gtnfqdyvmm.html

[T04] Kotlin：空安全
来源：http://hz.52xcode.cn/gthrtktzdr.html

val n: String? = null;  n?.length
来源：http://hz.pengpengdd.cyou/gtpvvmjtgv.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtfxvxpahx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gzhubu.top/gtjacjzqwx.html

[T06] Kotlin：集合映射
来源：http://hz.jiagoushi.top/gtpuulvxij.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gaohongyu789.top/gtkrpulotp.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtbpegpgrv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.quarkkingdee.top/gtlzkvgixr.html

[T08] Kotlin：数据类
来源：http://hz.aibaodan.cn/gtvxjizrfd.html

data class User(val name: String, val age: Int)
来源：http://hz.jinqigfzy.top/gtkeunucmr.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtlvenosiy.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtibrewreh.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtkxceifig.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtkvopxvvw.html

[T11] Kotlin：协程
来源：http://hz.zhijiandao.cn/gtiwudgfox.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yangfankeji.com/gtaszrmfyl.html

[T12] Kotlin：解构声明
来源：http://hz.xziqi.cn/gtxezskmnd.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtxwpqbakf.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtkiuocgsh.html

val m = mapOf("a" to 1)
来源：http://hz.zhaomingkeji.xyz/gtirxeudgq.html

[T14] Kotlin：循环
来源：http://hz.bjfxy.top/gtzgzdnhdk.html

for (i in 1..10) println(i)
来源：http://hz.ybcxt.top/gtmlvqkesk.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtinjwzraf.html

interface Shape { fun area(): Double }
来源：http://hz.hywenlv.cn/gtqlmpuyce.html

[T16] Swift：Hello World
来源：http://hz.guowangkeji.top/gtklknhfyb.html

print("Hello")
来源：http://hz.zhixingplan.top/gtrepgalny.html

[T17] Swift：变量与常量
来源：http://hz.pycfn.com/gtyijaoywz.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gtxljxwbmd.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtnwjizisp.html

"值: \(b)"
来源：http://hz.ivvv.top/gtaxlqptxo.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtvdshyvfb.html

if let n = opt { print(n) }
来源：http://hz.jlsjyb.cn/gtyubnofsv.html

[T20] Swift：数组操作
来源：http://hz.jqgufenzy.top/gtcwmhfysb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuxming.cn/gtbnccxmtv.html

[T21] Swift：遍历
来源：http://hz.xziqi.cn/gtgjstusqp.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtnwtvqerp.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtihbeiagj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtcrnolqwb.html

[T23] Swift：函数
来源：http://hz.xylfe.cn/gtukbxpyec.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xuanzx.com/gtfbzeguzh.html

[T24] Swift：闭包
来源：http://hz.hfpthk.cn/gtftmthtxw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenzaomai.com/gtqpjhawxr.html

[T25] Swift：结构体
来源：http://hz.svipenyu.cn/gtjiltdrcx.html

struct P { var x: Int }
来源：http://hz.chenjidiqi.icu/gtvxlgtzov.html

[T26] Swift：类与重写
来源：http://hz.yuxming.cn/gtnjdmbpmu.html

class A: Base { override func f() {} }
来源：http://hz.c1oappe.top/gtwfhxabic.html

[T27] Swift：错误处理
来源：http://hz.ydjk.org.cn/gtxlpahyje.html

do { try f() } catch { print(error) }
来源：http://hz.zhoulong.xyz/gtyumemwct.html

[T28] Swift：枚举
来源：http://hz.sysykeji.top/gtgpwbtbjf.html

enum Color { case red, green }
来源：http://hz.nwbrower.top/gtrzuvsoml.html

[T29] Swift：guard 提前返回
来源：http://hz.gzhubu.top/gtmuvbfjbl.html

guard let x = opt else { return }
来源：http://hz.jiagoushi.top/gtvlkcegpa.html

[T30] Swift：协议
来源：http://hz.shanyushiyangtech.top/gtqbrwfefg.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtmquunjjf.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtvwpicgdf.html

print("Hello")
来源：http://hz.9152youxi.cn/gtpxdecbzd.html

[T32] Lua：局部变量
来源：http://hz.sxryk.cn/gtbxtwwoxr.html

local a = 1
来源：http://hz.zhongyouzk.top/gtwhubzura.html

[T33] Lua：表（数组）
来源：http://hz.yj202588.top/gtgulzqtkz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zycfv.cn/gtqtyfdwqn.html

[T34] Lua：遍历表
来源：http://hz.xuanzx.com/gtqnnblloz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ehwqpu.com/gtvxbgrbfp.html

[T35] Lua：字典表
来源：http://hz.hfpthk.cn/gthoxyikzt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.mhx1999.top/gtzeqgqbzl.html

[T36] Lua：函数
来源：http://hz.quarkkingdee.top/gtythpqpcc.html

function add(a, b) return a + b end
来源：http://hz.nwbrower.top/gtgyhswpbc.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtacshyrlc.html

"a" .. "b"
来源：http://hz.dashuyun.cn/gtaseiquom.html

[T38] Lua：条件
来源：http://hz.shangyingyoupin.top/gtvnrqbida.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtckkyebvd.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtgxsnxybi.html

string.find(s, "%d+")
来源：http://hz.pycfn.com/gtwxooijfg.html

[T40] Lua：元表
来源：http://hz.havefunace.top/gtmhbglzch.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtzsxarmya.html

[T41] Perl：Hello World
来源：http://hz.fzhhl.top/gtyemjbptb.html

print "Hello\n";
来源：http://hz.zhijiandao.cn/gtlftcabmm.html

[T42] Perl：变量类型
来源：http://hz.feifeiyinyue.top/gttpbawaem.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtbnxbbuxf.html

[T43] Perl：字符串插值
来源：http://hz.zycfv.cn/gtqcqwkram.html

"值: $a"
来源：http://hz.ywan-chungtsiang.top/gttouttulg.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gtrnjdjxfr.html

if ($a > 0) { print "正"; }
来源：http://hz.hysaishi.cn/gttqhjspeb.html

[T45] Perl：数组遍历
来源：http://hz.zdqjudy.top/gtaanjxalj.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gtpaiucngf.html

[T46] Perl：哈希操作
来源：http://hz.gotoacloud.top/gtuqifsqnf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.tianlin.xyz/gtrxfwomxz.html

[T47] Perl：正则捕获
来源：http://hz.daria6918.cn/gtawtsvbih.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuetiantiany.cn/gtkskihmcw.html

[T48] Perl：正则替换
来源：http://hz.bjfxy.top/gtnivkvexp.html

$s =~ s/old/new/g;
来源：http://hz.zhengqikj.top/gtyjbfmhkf.html

[T49] Perl：函数
来源：http://hz.ivvv.top/gtjcwcfycs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cqqwz.cn/gtdwnvwhfo.html

[T50] Perl：逐行读文件
来源：http://hz.hongshengwenyu.top/gtksavuvju.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.svipenyu.cn/gtfkifcypy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgfzy.top/gtpqdjvrlq.html

[T51] Scala：Hello World
来源：http://hz.zhongyouzk.top/gttfeliftw.html

println("Hello")
来源：http://hz.cheryme.top/gtausstqqk.html

[T52] Scala：变量
来源：http://hz.jinyuanbaomall.cn/gtzfreeyzs.html

val a = 1;  var b = 2
来源：http://hz.dianchejie.cn/gtzarxlrdg.html

[T53] Scala：字符串插值
来源：http://hz.zhoulong.xyz/gtkjenwlgz.html

s"值: $b"
来源：http://hz.xylfe.cn/gtlgwvqbmw.html

[T54] Scala：集合映射
来源：http://hz.ppjwa.cn/gtapfertee.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ybcxt.top/gtfybyidcm.html

[T55] Scala：集合过滤
来源：http://hz.hfpthk.cn/gtpzibrsit.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhoulong.xyz/gtxydpvwzh.html

[T56] Scala：样例类
来源：http://hz.andypj.xyz/gtvmpczegc.html

case class User(name: String, age: Int)
来源：http://hz.gotoacloud.top/gtsbwgsxmy.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gtavzbtnof.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gtiwitytcq.html

[T58] Scala：函数定义
来源：http://hz.316326.xyz/gtlqubsvjz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.dianchejie.cn/gthwxtgccd.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtrylngicn.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gthngxhjzo.html

[T60] Scala：折叠
来源：http://hz.svipenyu.cn/gtavaqxlbo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.haohaochexian.top/gtopzxayjl.html

================================================================================
来源：http://hz.guowangkeji.top/gtqiqrzrrd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgfzy.top/gtepdqbnxz.html

================================================================================
来源：http://hz.sweek.top/gtielsjflz.html

[U01] Py：创建虚拟环境
来源：http://hz.sufxvd.cn/gtvtkbebqn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sufxvd.cn/gtmazvgcvy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.hnqzz.top/gtqrupbixl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pycfn.com/gtqokmhiuw.html

[U03] Py：加载 .env 配置
来源：http://hz.xylfe.cn/gtwcgdyqnw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ywan-chungtsiang.top/gtrzxjitig.html

[U04] Py：变量调试打印
来源：http://hz.hongshengwenyu.top/gtmhhvwazu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xylfe.cn/gtwlcucecm.html

[U05] Py：列表去重且保序
来源：http://hz.mhx1999.top/gtohoulhzs.html

list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtlcytcifc.html

[U06] Py：合并两个字典
来源：http://hz.xuanzx.com/gtquncylpl.html

{**a, **b}
来源：http://hz.yuxming.cn/gtlhtocmwm.html

[U07] Py：反转字典键值
来源：http://hz.xziqi.cn/gtwrolijtz.html

{v: k for k, v in d.items()}
来源：http://hz.birdmap.top/gtjhhvbhrz.html

[U08] Py：展平二维列表
来源：http://hz.snrcjt.cn/gtnniqzggz.html

[y for x in nested for y in x]
来源：http://hz.redwolf501.top/gtlfvyykvl.html

[U09] Py：字典取最大值的键
来源：http://hz.ppjwa.cn/gtlyeawwhx.html

max(d, key=d.get)
来源：http://hz.pengpengdd.cyou/gtorttlyxq.html

[U10] Py：按值排序字典
来源：http://hz.smart0.xyz/gtmroluzsh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xziqi.cn/gtdzxazaoz.html

[U11] Py：生成器表达式
来源：http://hz.kuanghao11.cn/gtjurzxvkg.html

(x * 2 for x in arr)
来源：http://hz.zhijiandao.cn/gtfqujynby.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnxiangtu.top/gtwcebrbct.html

Counter(arr).most_common(3)
来源：http://hz.yanxiufei.cn/gtrcesiesv.html

[U13] Py：固定长度队列
来源：http://hz.hongshengwenyu.top/gtnytjaper.html

deque(maxlen=10)
来源：http://hz.hnxiangtu.top/gtbfkyczon.html

[U14] Py：分组收集到列表
来源：http://hz.zycfv.cn/gtstcjvpis.html

defaultdict(list)
来源：http://hz.quarkkingdee.top/gtloexwope.html

[U15] Py：高精度计时
来源：http://hz.chenjidiqi.icu/gtwwjjebqk.html

t = time.perf_counter()
来源：http://hz.hnxiangtu.top/gtowtmooxi.html

[U16] Py：命令行参数解析
来源：http://hz.tanke756.top/gtrldpedbb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.chenzaomai.com/gtuonrjtay.html

[U17] Py：初始化日志
来源：http://hz.nanxinkj.top/gtfnyierzi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.smart0.xyz/gtbyollojd.html

[U18] Py：预编译正则
来源：http://hz.nanxinkj.top/gteixbznpp.html

pat = re.compile(r"\d+")
来源：http://hz.zhijiandao.cn/gtvaxgrjdh.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigufen.top/gtqpujmmbs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ydzc1.top/gtbnrmpege.html

[U20] Py：缓存函数结果
来源：http://hz.fengsongda.top/gtomfvbsjj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ivvv.top/gtmgbeynfz.html

[U21] Py：自定义上下文管理器
来源：http://hz.shuidangran.top/gtvycwrbou.html

@contextlib.contextmanager
来源：http://hz.hysaishi.cn/gtfmsvubzv.html

[U22] Py：矩阵转置
来源：http://hz.ybcxt.top/gtdokkmnzh.html

list(zip(*m))
来源：http://hz.nwbrower.top/gttjvnmnud.html

[U23] Py：分块读取大文件
来源：http://hz.hnxiangtu.top/gtwjzgruhf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ydzc1.top/gtepuvfxzb.html

[U24] Py：路径操作
来源：http://hz.cheryme.top/gtgetvmkez.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtevrzkppz.html

[U25] Py：CSV 按字典读
来源：http://hz.daria6918.cn/gtxpmxpmty.html

csv.DictReader(f)
来源：http://hz.wangdashe.top/gtonvgtxyg.html

[U26] Py：并发下载
来源：http://hz.shanyushiyangkeji.top/gtzakymbqc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gaohongyu789.top/gtkghsyzul.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gtytrteozv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yj20258.top/gtnbqekzcg.html

[U28] Py：类型别名
来源：http://hz.yj20258888.top/gtlyzvyshg.html

UserId = int
来源：http://hz.birdmap.top/gtieieixzt.html

[U29] Py：属性校验
来源：http://hz.chenlongwang.top/gtzxnddghr.html

@property 与 @x.setter 配合
来源：http://hz.hnqzz.top/gtrxyozziz.html

[U30] Py：数据类
来源：http://hz.redwolf501.top/gtogcxpwqz.html

@dataclass(slots=True)
来源：http://hz.daria6918.cn/gtakwubglm.html

[U31] Py：单测
来源：http://hz.jqgufenzy.top/gtivjaxhok.html

python -m pytest -q
来源：http://hz.pengpengdd.cyou/gtohwprcgn.html

[U32] Py：代码格式化
来源：http://hz.cashguo.top/gtchmizfkn.html

ruff format . && ruff check --fix .
来源：http://hz.gzhubu.top/gtexsbofid.html

[U33] Py：打包发布
来源：http://hz.redwolf501.top/gtkeuqcvvq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xinyue.icu/gtbvpkxmgh.html

[U34] Py：判断编码
来源：http://hz.jinqigfzy.top/gtzcjjwfnh.html

chardet.detect(raw)
来源：http://hz.ppjwa.cn/gtycydumhj.html

[U35] Py：发送邮件
来源：http://hz.316326.xyz/gtavtwurza.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhongyouzk.top/gtkbrjatlj.html

[U36] Py：定时任务
来源：http://hz.nwbrower.top/gtlvuqjqjl.html

schedule.every(10).minutes.do(job)
来源：http://hz.ivvv.top/gtdfjezgef.html

[U37] Py：读写 Excel
来源：http://hz.yvedp.cn/gtyredvzdz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nanxuanxn.top/gtorehazqg.html

[U38] Py：获取脚本所在目录
来源：http://hz.yueranfly.top/gtxaoirtgm.html

Path(__file__).resolve().parent
来源：http://hz.yongpay.top/gtgbieuovr.html

[U39] Py：判断是否在交互环境
来源：http://hz.ivvv.top/gtafiltmwt.html

sys.stdout.isatty()
来源：http://hz.chenjidiqi.icu/gtepnquumf.html

[U40] Py：打印到标准错误
来源：http://hz.quarkkingdee.top/gtumkkxbom.html

print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtxdszzqzf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhaomingkeji.xyz/gtqxryiorl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yuxming.cn/gtrexarynq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hnqzz.top/gtpgfnuxws.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dianchejie.cn/gthyejmidt.html

[U43] PHP：声明命名空间
来源：http://hz.yvedp.cn/gtxsvhnugm.html

namespace App\Http;
来源：http://hz.xingfuxueyuan.xyz/gtafkzztst.html

[U44] PHP：开启严格类型
来源：http://hz.cucudq.cn/gtugjvectq.html

declare(strict_types=1);
来源：http://hz.zhaomingkeji.xyz/gtqgmwupbz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.tian-w.cn/gtzmefohdt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gthggkdbqm.html

[U46] PHP：可空类型
来源：http://hz.aibaodan.cn/gtwifxhxks.html

?string $name = null
来源：http://hz.316326.xyz/gtxetkojhn.html

[U47] PHP：联合类型
来源：http://hz.yj202588.top/gtwqjsaxcn.html

int|string $id
来源：http://hz.wangdashe.top/gtruihzato.html

[U48] PHP：纯枚举
来源：http://hz.jlsjyb.cn/gtyplwhrei.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenlongwang.top/gtsxdyobzs.html

[U49] PHP：只读属性
来源：http://hz.haohaochexian.top/gtexizjxns.html

public readonly string $name
来源：http://hz.sxryk.cn/gtxorrrxml.html

[U50] PHP：构造器属性提升
来源：http://hz.ybcxt.top/gtofajvpty.html

public function __construct(private int $id) {}
来源：http://hz.guowangkeji.top/gtqvqnrolq.html

[U51] PHP：数组解构
来源：http://hz.nwbrower.top/gtroanougb.html

[$a, $b] = $arr;
来源：http://hz.yuanzhike.top/gtcotegmkr.html

[U52] PHP：箭头函数
来源：http://hz.sweek.top/gtsyabbsae.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtiofsrhdy.html

[U53] PHP：空合并运算符
来源：http://hz.ydjk.org.cn/gtbftkiumx.html

$v = $a ?? $b ?? "default";
来源：http://hz.iojbl.cn/gtowcjhqhj.html

[U54] PHP：空安全调用
来源：http://hz.guowangkeji.top/gtlnjpjqyw.html

$obj?->method()
来源：http://hz.yj20258.top/gtskwnvxih.html

[U55] PHP：match 表达式
来源：http://hz.sweek.top/gtggbyoomu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shangyingyoupin.top/gtcbnefsps.html

[U56] PHP：命名参数
来源：http://hz.sysykeji.top/gtijbxiwzr.html

f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtphksrpfy.html

[U57] PHP：字符串插值
来源：http://hz.52xcode.cn/gtowpkemnj.html

"值: {$a}"
来源：http://hz.guowangkeji.top/gtqzodyxnt.html

[U58] PHP：数组三件套
来源：http://hz.0kj1m.cn/gtappmhpxf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zdqjudy.top/gtyaomdata.html

[U59] PHP：自定义排序
来源：http://hz.chenzaomai.com/gtofjmjugp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtqmcbxphu.html

[U60] PHP：JSON 编解码
来源：http://hz.yonumen.top/gtkrexjgki.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuetiantiany.cn/gtrrtbzebe.html

[U61] PHP：正则
来源：http://hz.ppjwa.cn/gtrozcvahj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtspstacvh.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtvswmtsbs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.sxryk.cn/gtjhfqvlfe.html

[U63] PHP：文件读写
来源：http://hz.ppjwa.cn/gtpaufpkrx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.wangdashe.top/gtwjxnznue.html

[U64] PHP：目录遍历
来源：http://hz.zycfv.cn/gtreqvawvy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ydzc1.top/gtzpyjyhbv.html

[U65] PHP：会话
来源：http://hz.zhoulong.xyz/gtayqosaak.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cucudq.cn/gtwpzvnsiq.html

[U66] PHP：设置 Cookie
来源：http://hz.nanxinkj.top/gthqcbtyxk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gaohongyu789.top/gtwrqivldv.html

[U67] PHP：处理文件上传
来源：http://hz.c1oappe.top/gtvsilrnzz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.0kj1m.cn/gtozdiznvu.html

[U68] PHP：PDO 连接
来源：http://hz.jinqigfzy.top/gtdacigrdi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.quarkkingdee.top/gtdeoxggin.html

[U69] PHP：PDO 预处理
来源：http://hz.jiagoushi.top/gtnvmauxsq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.havefunace.top/gttrximjtg.html

[U70] PHP：PDO 事务
来源：http://hz.0kj1m.cn/gtrnyqrmru.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ydjk.org.cn/gtacdqchsh.html

[U71] PHP：抛出异常
来源：http://hz.jinqigfzy.top/gtvfjoiire.html

throw new RuntimeException("失败", 500);
来源：http://hz.hfpthk.cn/gtjcztpung.html

[U72] PHP：写错误日志
来源：http://hz.aibaodan.cn/gtyehwgxwk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.hongshengwenyu.top/gtvowjbdkw.html

[U73] PHP：读取 ini 配置
来源：http://hz.yuanzhike.top/gtveqojzgx.html

parse_ini_file("config.ini", true)
来源：http://hz.aibaodan.cn/gtnpktnfoz.html

[U74] PHP：读取环境变量
来源：http://hz.zycfv.cn/gtsjnhyvst.html

getenv("APP_ENV") ?: "production"
来源：http://hz.tianlin.xyz/gthabgmyza.html

[U75] PHP：依赖注入
来源：http://hz.hywenlv.cn/gtppiaoloo.html

composer require psr/container
来源：http://hz.yj20258888.top/gtzlhypmgh.html

[U76] PHP：简单路由
来源：http://hz.tianlin.xyz/gtpszeewjv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jlsjyb.cn/gtqozehogx.html


<!-- 参考信息 -->