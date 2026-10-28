代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangkeji.top/gtjbacpmxt.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gttsvavkkx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtqmbrymmn.html

[S50] C++：格式化数字
来源：http://hz.xinyue.icu/gtbzshmnup.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtihhzqdwk.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtrqjkiury.html

static_cast<double>(a) / b
来源：http://hz.316326.xyz/gttlmbbsfa.html

[S52] C++：const 与 noexcept
来源：http://hz.ybcxt.top/gtydduqeea.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtpurwnffq.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtkkjovqhz.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtnwmzsgqw.html

[S54] C++：异常处理
来源：http://hz.quarkkingdee.top/gtesucnmjk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtmxopqowo.html

[S55] C++：结构化绑定
来源：http://hz.ivvv.top/gtqojqjhlm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xylfe.cn/gtfgemfpsf.html

[S56] C++：optional
来源：http://hz.c1oappe.top/gtytecetpx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yvedp.cn/gthzogozvq.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtcvrgizvo.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtffuaenad.html

[S58] C++：命名空间
来源：http://hz.daxiang520.top/gttamdmwst.html

namespace ns { int f() { return 1; } }
来源：http://hz.sweek.top/gtksguutsa.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtjqekspra.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.andypj.xyz/gtadtwallm.html

[S60] C++：遍历并删除元素
来源：http://hz.birdmap.top/gtjwttgeiu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xuetiantiany.cn/gtzpxrdpsx.html

================================================================================
来源：http://hz.ppjwa.cn/gtdarxzewc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtyfgzlmjq.html

================================================================================
来源：http://hz.52xcode.cn/gtuwuiahii.html

[T01] Kotlin：Hello World
来源：http://hz.ehwqpu.com/gtfvbmvawd.html

println("Hello")
来源：http://hz.yj20258888.top/gtlwiurgdj.html

[T02] Kotlin：变量
来源：http://hz.yueranfly.top/gtgtolpylj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cdnleiting.top/gtlbaxufwr.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtwxcyuqaw.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtncfsxdnj.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtqiotzdhh.html

val n: String? = null;  n?.length
来源：http://hz.jiagoushi.top/gtydabryjj.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gtukpjfpjc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtcoxtimrx.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gtaggygncx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ivvv.top/gtozrmirxd.html

[T07] Kotlin：集合过滤
来源：http://hz.iojbl.cn/gtarawmuzb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hywenlv.cn/gtcnegixtp.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtpnmkpjvu.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtdnmucmaz.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gtyudsrhjs.html

fun String.exclaim() = this + "!"
来源：http://hz.pengpengdd.cyou/gttfykkxey.html

[T10] Kotlin：默认参数
来源：http://hz.hywenlv.cn/gtjwvwxjkr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gthdkyhjqg.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtgkdypvrs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtxdttcirg.html

[T12] Kotlin：解构声明
来源：http://hz.hongshengwenyu.top/gtfekyyhzy.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtcgbbvrxr.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtpjbiblcm.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gteyblupoh.html

[T14] Kotlin：循环
来源：http://hz.ehwqpu.com/gtirarvdtj.html

for (i in 1..10) println(i)
来源：http://hz.sxryk.cn/gtjmjybmpj.html

[T15] Kotlin：接口
来源：http://hz.jinghuilouyu.cn/gtertpiobl.html

interface Shape { fun area(): Double }
来源：http://hz.xylfe.cn/gtxfmghbtv.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gtiwuuojej.html

print("Hello")
来源：http://hz.yuxming.cn/gtimikwrxl.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtguqtzypl.html

var a = 1;  let b = 2
来源：http://hz.0kj1m.cn/gtsznikkuc.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtzcaxrccm.html

"值: \(b)"
来源：http://hz.hnqzz.top/gtjsjdrziu.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtacypaizd.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtyyxpnnmx.html

[T20] Swift：数组操作
来源：http://hz.chenzaomai.com/gttyyvbgop.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuanzhike.top/gtusikahif.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gthituttcg.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtielfqnbs.html

[T22] Swift：字典
来源：http://hz.tianlin.xyz/gtciyeregn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.316326.xyz/gtssvrckgv.html

[T23] Swift：函数
来源：http://hz.gaohongyu789.top/gtcpoosrjb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtrcawackr.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtrktbrhni.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtifurdpxq.html

[T25] Swift：结构体
来源：http://hz.cdnleiting.top/gtperazity.html

struct P { var x: Int }
来源：http://hz.hfpthk.cn/gtugaaehsx.html

[T26] Swift：类与重写
来源：http://hz.tanke756.top/gtlyitxezw.html

class A: Base { override func f() {} }
来源：http://hz.sysykeji.top/gtxublvtme.html

[T27] Swift：错误处理
来源：http://hz.dianchejie.cn/gtazzdjzhn.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtegihmglk.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtofkizfhr.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtnfosiomz.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigfzy.top/gtsggscrfy.html

guard let x = opt else { return }
来源：http://hz.jyoumei.cn/gtrpypoqhk.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gtxfnxftpm.html

protocol Shape { func area() -> Double }
来源：http://hz.hysaishi.cn/gtwpqacelt.html

[T31] Lua：Hello World
来源：http://hz.xziqi.cn/gthzxanckv.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtliauachs.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gtuhbervho.html

local a = 1
来源：http://hz.jlsjyb.cn/gtynmvwhyp.html

[T33] Lua：表（数组）
来源：http://hz.xinyue.icu/gtqtdvvrpf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.quarkkingdee.top/gtpugyorbq.html

[T34] Lua：遍历表
来源：http://hz.haohaochexian.top/gteexhekax.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gtegiuctjf.html

[T35] Lua：字典表
来源：http://hz.nanxinkj.top/gtagnprzow.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhiwuduotai.top/gttagjergn.html

[T36] Lua：函数
来源：http://hz.jiagoushi.top/gticfclqpt.html

function add(a, b) return a + b end
来源：http://hz.zhengqikj.top/gtwamvcqel.html

[T37] Lua：字符串拼接
来源：http://hz.hammf.cn/gtfcjmwmoe.html

"a" .. "b"
来源：http://hz.ydjk.org.cn/gtsxglblkf.html

[T38] Lua：条件
来源：http://hz.zycfv.cn/gtihonucoj.html

if x > 0 then print("正") end
来源：http://hz.ydzc1.top/gtdkuebgnu.html

[T39] Lua：模式匹配
来源：http://hz.jlsjyb.cn/gtmiscatpd.html

string.find(s, "%d+")
来源：http://hz.chenzaomai.com/gtwcdbzvzl.html

[T40] Lua：元表
来源：http://hz.jinqigufen.top/gttjznrfen.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtzoyhqalk.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtnlpxikfj.html

print "Hello\n";
来源：http://hz.gzhubu.top/gtecaymlxx.html

[T42] Perl：变量类型
来源：http://hz.ppjwa.cn/gtjofovfxn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhengqikj.top/gtuvdekgrk.html

[T43] Perl：字符串插值
来源：http://hz.jiagoushi.top/gtvezvguzm.html

"值: $a"
来源：http://hz.yonumen.top/gtsuzkgrmf.html

[T44] Perl：条件
来源：http://hz.meibo888.top/gtizhhorbp.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtzqadrhbx.html

[T45] Perl：数组遍历
来源：http://hz.iojbl.cn/gtogztbqiw.html

for my $x (@arr) { print $x; }
来源：http://hz.sufxvd.cn/gtrnvpgslc.html

[T46] Perl：哈希操作
来源：http://hz.ydjk.org.cn/gtljoxfdpu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.316326.xyz/gttwvcleeu.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtblowprst.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.iojbl.cn/gttcwgjzqp.html

[T48] Perl：正则替换
来源：http://hz.yj20258888.top/gteshhexgc.html

$s =~ s/old/new/g;
来源：http://hz.9152youxi.cn/gtdebhgltq.html

[T49] Perl：函数
来源：http://hz.zhengqikj.top/gtforrcigz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtkphvxmhy.html

[T50] Perl：逐行读文件
来源：http://hz.tianlin.xyz/gtpggltswm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.gzhubu.top/gtqbuakrvh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.dianchejie.cn/gtkqdlmbtk.html

[T51] Scala：Hello World
来源：http://hz.quarkkingdee.top/gtmubuugja.html

println("Hello")
来源：http://hz.mhx1999.top/gtqtebmqiq.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtsrrbippq.html

val a = 1;  var b = 2
来源：http://hz.zhengqikj.top/gtlnhiuvlb.html

[T53] Scala：字符串插值
来源：http://hz.hysaishi.cn/gtxgqckykn.html

s"值: $b"
来源：http://hz.cheryme.top/gtrslvrlgu.html

[T54] Scala：集合映射
来源：http://hz.svipenyu.cn/gtlxiadgez.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ywan-chungtsiang.top/gtjlzcvzqb.html

[T55] Scala：集合过滤
来源：http://hz.sweek.top/gtbvbarbek.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtbfalbjiv.html

[T56] Scala：样例类
来源：http://hz.gaohongyu789.top/gtmichmyvs.html

case class User(name: String, age: Int)
来源：http://hz.jqgfzy.top/gtxvsxadcj.html

[T57] Scala：模式匹配
来源：http://hz.shzxlz.cn/gtyddsphle.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuanzx.com/gtztrbssxm.html

[T58] Scala：函数定义
来源：http://hz.sysykeji.top/gtitnabsla.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhongyouzk.top/gtlskjmfyu.html

[T59] Scala：循环
来源：http://hz.shangyingyoupin.top/gtogjyasyt.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtwvezkvdj.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gteeebtbeu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xingfuxueyuan.xyz/gtrnfthgmd.html

================================================================================
来源：http://hz.tanke756.top/gtujxyivgk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtmknoaxzo.html

================================================================================
来源：http://hz.iojbl.cn/gtubnqkegi.html

[U01] Py：创建虚拟环境
来源：http://hz.zhiwuduotai.top/gtodytgbdz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xinyue.icu/gtuovgfyug.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtrxemsfpq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ppjwa.cn/gttcthjqtk.html

[U03] Py：加载 .env 配置
来源：http://hz.nwbrower.top/gtdsnvmdfr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtyhlyjbez.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gtwzblcsma.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gttjjsswco.html

[U05] Py：列表去重且保序
来源：http://hz.zhiwuduotai.top/gtzgvkvmbs.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtpudsafnr.html

[U06] Py：合并两个字典
来源：http://hz.andypj.xyz/gtnmvygcho.html

{**a, **b}
来源：http://hz.nanxuanxn.top/gtllvqwytw.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtskpckqqe.html

{v: k for k, v in d.items()}
来源：http://hz.hysaishi.cn/gtwcujqgbf.html

[U08] Py：展平二维列表
来源：http://hz.hongshengwenyu.top/gtyjoymspm.html

[y for x in nested for y in x]
来源：http://hz.yj20258.top/gtcvblopjo.html

[U09] Py：字典取最大值的键
来源：http://hz.shuidangran.top/gtcyiiobak.html

max(d, key=d.get)
来源：http://hz.zhaomingkeji.xyz/gtxwynnvlq.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtndezmxef.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gogol.net.cn/gtetizguzx.html

[U11] Py：生成器表达式
来源：http://hz.jiagoushi.top/gtbzjfygmn.html

(x * 2 for x in arr)
来源：http://hz.xuetiantiany.cn/gthszwbluy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.aizwys.cn/gtyigftwkj.html

Counter(arr).most_common(3)
来源：http://hz.yuxming.cn/gtijccqnqz.html

[U13] Py：固定长度队列
来源：http://hz.wangdashe.top/gtsydqkrsl.html

deque(maxlen=10)
来源：http://hz.jiagoushi.top/gtlsaeneqy.html

[U14] Py：分组收集到列表
来源：http://hz.zhaomingkeji.xyz/gtgwehjerq.html

defaultdict(list)
来源：http://hz.kuanghao11.cn/gtqqtwcgxo.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtvstjwdvp.html

t = time.perf_counter()
来源：http://hz.pengpengdd.cyou/gtsmnigxsu.html

[U16] Py：命令行参数解析
来源：http://hz.xuetiantiany.cn/gtqfxiimha.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.birdmap.top/gtuwdzbpgi.html

[U17] Py：初始化日志
来源：http://hz.dashuyun.cn/gtubotxboj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.mhx1999.top/gtdytirqdh.html

[U18] Py：预编译正则
来源：http://hz.dianchejie.cn/gtfgdzlyzy.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtrpikcxil.html

[U19] Py：正则替换带回调
来源：http://hz.chenzaomai.com/gtepuegbuq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtclqgirtx.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtgfrzddpp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ydzc1.top/gtmaxneecb.html

[U21] Py：自定义上下文管理器
来源：http://hz.sufxvd.cn/gtpseabccu.html

@contextlib.contextmanager
来源：http://hz.jinqigufen.top/gtjqfdjedr.html

[U22] Py：矩阵转置
来源：http://hz.pengpengdd.cyou/gtssbfyrrv.html

list(zip(*m))
来源：http://hz.wangshuangyany.cn/gtadccdrhh.html

[U23] Py：分块读取大文件
来源：http://hz.sweek.top/gtoylahtig.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.snrcjt.cn/gtynhhnlbh.html

[U24] Py：路径操作
来源：http://hz.sysykeji.top/gtgljvllnx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxinkj.top/gtvacrruxl.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtmggzqbtz.html

csv.DictReader(f)
来源：http://hz.yj20258888.top/gtsemhxmuo.html

[U26] Py：并发下载
来源：http://hz.ywan-chungtsiang.top/gtlibpwiak.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yj20258888.top/gturfcxeal.html

[U27] Py：异步 HTTP
来源：http://hz.nanxinkj.top/gtgjqswmel.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nanxinkj.top/gtdwykrvuu.html

[U28] Py：类型别名
来源：http://hz.jyoumei.cn/gtorpidtna.html

UserId = int
来源：http://hz.hongshengwenyu.top/gtohgayjup.html

[U29] Py：属性校验
来源：http://hz.ppjwa.cn/gtbotqgtdx.html

@property 与 @x.setter 配合
来源：http://hz.pycfn.com/gtbraxfylt.html

[U30] Py：数据类
来源：http://hz.jinqigfzy.top/gtkqypmquq.html

@dataclass(slots=True)
来源：http://hz.chenzaomai.com/gtwpzgxmag.html

[U31] Py：单测
来源：http://hz.hfpthk.cn/gtfttyvfuj.html

python -m pytest -q
来源：http://hz.zhijiandao.cn/gtryjhqhgf.html

[U32] Py：代码格式化
来源：http://hz.0kj1m.cn/gtrzcivvjq.html

ruff format . && ruff check --fix .
来源：http://hz.guannengcc.top/gttgvjbhfg.html

[U33] Py：打包发布
来源：http://hz.xuanzx.com/gtfvnzkpsp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhongyouzk.top/gtvihwbhzj.html

[U34] Py：判断编码
来源：http://hz.jinyuanbaomall.cn/gtxojxcnjg.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gthpuregwi.html

[U35] Py：发送邮件
来源：http://hz.jyoumei.cn/gtqhlckeyg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shzxlz.cn/gtpcptgeyh.html

[U36] Py：定时任务
来源：http://hz.hfpthk.cn/gtixrtkfhk.html

schedule.every(10).minutes.do(job)
来源：http://hz.wangshuangyany.cn/gtcwttskvh.html

[U37] Py：读写 Excel
来源：http://hz.snrcjt.cn/gtjcdsjowt.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.aibaodan.cn/gtibwdyvkk.html

[U38] Py：获取脚本所在目录
来源：http://hz.hammf.cn/gtqvmclvym.html

Path(__file__).resolve().parent
来源：http://hz.cqqwz.cn/gtvefoezon.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuetiantiany.cn/gtfuksrxns.html

sys.stdout.isatty()
来源：http://hz.hfpthk.cn/gtusomhpzu.html

[U40] Py：打印到标准错误
来源：http://hz.yanxiufei.cn/gtktfupjyf.html

print("err", file=sys.stderr)
来源：http://hz.yj202588.top/gtxsherosq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ppjwa.cn/gtxjhcoxtj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenlongwang.top/gteeodsryw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj20258.top/gthhgbdlvk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cashguo.top/gtjeemefqu.html

[U43] PHP：声明命名空间
来源：http://hz.guowangkeji.top/gtnitezknl.html

namespace App\Http;
来源：http://hz.yangfankeji.com/gtlvcsmkre.html

[U44] PHP：开启严格类型
来源：http://hz.chenlongwang.top/gtxisdtfbl.html

declare(strict_types=1);
来源：http://hz.cashguo.top/gtvcuwyipl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hywenlv.cn/gtqnmwzagr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtperxrasd.html

[U46] PHP：可空类型
来源：http://hz.chenjidiqi.icu/gtyxcrvhnn.html

?string $name = null
来源：http://hz.ivvv.top/gtbopzsimn.html

[U47] PHP：联合类型
来源：http://hz.zycfv.cn/gtuuewithj.html

int|string $id
来源：http://hz.xuetiantiany.cn/gthcapygwz.html

[U48] PHP：纯枚举
来源：http://hz.ywan-chungtsiang.top/gtuytifdgu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hnqzz.top/gtpvxzzznl.html

[U49] PHP：只读属性
来源：http://hz.jinqigfzy.top/gtzanauers.html

public readonly string $name
来源：http://hz.zhijiandao.cn/gtiwwubhhr.html

[U50] PHP：构造器属性提升
来源：http://hz.316326.xyz/gtrliafgfp.html

public function __construct(private int $id) {}
来源：http://hz.jyoumei.cn/gttulomuvq.html

[U51] PHP：数组解构
来源：http://hz.birdmap.top/gtiyionyth.html

[$a, $b] = $arr;
来源：http://hz.ybcxt.top/gtsjjmyaqt.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtdtqbwtfq.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxuanxn.top/gtfkmprcgq.html

[U53] PHP：空合并运算符
来源：http://hz.sufxvd.cn/gtrbwtwjoh.html

$v = $a ?? $b ?? "default";
来源：http://hz.tian-w.cn/gtmhnzggxf.html

[U54] PHP：空安全调用
来源：http://hz.mhx1999.top/gtgqbwofjw.html

$obj?->method()
来源：http://hz.chenjidiqi.icu/gtgxoxsrnk.html

[U55] PHP：match 表达式
来源：http://hz.hnqzz.top/gtrjqblqlh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.redwolf501.top/gtevvwjwph.html

[U56] PHP：命名参数
来源：http://hz.shangyingyoupin.top/gtnlqgxefw.html

f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtsdbtomfw.html

[U57] PHP：字符串插值
来源：http://hz.bjfxy.top/gtyqqbztgu.html

"值: {$a}"
来源：http://hz.chenzaomai.com/gtflighzbi.html

[U58] PHP：数组三件套
来源：http://hz.zycfv.cn/gtbzsawzxn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.xylfe.cn/gtipntwlde.html

[U59] PHP：自定义排序
来源：http://hz.yj20258.top/gtpjaswhby.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.feifeiyinyue.top/gttpforpfp.html

[U60] PHP：JSON 编解码
来源：http://hz.316326.xyz/gtjqcendcr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.guannengcc.top/gtbsqqnfem.html

[U61] PHP：正则
来源：http://hz.guannengcc.top/gtyliyvqsg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtendorplj.html

[U62] PHP：日期对象
来源：http://hz.chenzaomai.com/gtrunweoqr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.dianchejie.cn/gtrjazqazj.html

[U63] PHP：文件读写
来源：http://hz.ywan-chungtsiang.top/gtpjwwihuu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zhiwuduotai.top/gtqvmfjwzz.html

[U64] PHP：目录遍历
来源：http://hz.gzhubu.top/gtnuusxzsc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hammf.cn/gtopdjrohx.html

[U65] PHP：会话
来源：http://hz.cashguo.top/gtmscmrjuq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.quarkkingdee.top/gttecsikaq.html

[U66] PHP：设置 Cookie
来源：http://hz.yj20258.top/gtmexazvcg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jqgfzy.top/gtixekivss.html

[U67] PHP：处理文件上传
来源：http://hz.hysaishi.cn/gtfzzjkfiw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.snrcjt.cn/gtgbmvaxco.html

[U68] PHP：PDO 连接
来源：http://hz.shuidangran.top/gtfwtstnjd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.redwolf501.top/gtucwavewm.html

[U69] PHP：PDO 预处理
来源：http://hz.nanxinkj.top/gtkvnyxiac.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhixingplan.top/gttdtuazpd.html

[U70] PHP：PDO 事务
来源：http://hz.yj20258.top/gtmvlkvtav.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hfpthk.cn/gtnkvyxdsd.html

[U71] PHP：抛出异常
来源：http://hz.nanxinkj.top/gtpyzdsukt.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gtpjvdewut.html

[U72] PHP：写错误日志
来源：http://hz.ehwqpu.com/gtsppqthcm.html

error_log("失败: " . $e->getMessage());
来源：http://hz.pengpengdd.cyou/gtkjwlpiwp.html

[U73] PHP：读取 ini 配置
来源：http://hz.zhongyouzk.top/gtscdyivfu.html

parse_ini_file("config.ini", true)
来源：http://hz.cqqwz.cn/gtuzcnqaqp.html

[U74] PHP：读取环境变量
来源：http://hz.ehwqpu.com/gtqukpfpdt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hysaishi.cn/gtbywraizt.html


<!-- 参考信息 -->