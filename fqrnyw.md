代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.vqdsnc.cn/gtmpbgyijb.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtzmwiqwjg.html

std::vector<int> w = std::move(v);
来源：http://hz.shuidangran.top/gtqmsxzyzv.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangkeji.top/gttxssweer.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtublzuxyf.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gttvxpwekd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtmsdiqaph.html

[S56] C++：optional
来源：http://hz.cashguo.top/gtqbwjbptv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.mhx1999.top/gthfjhffgl.html

[S57] C++：编译期常量
来源：http://hz.meibo888.top/gtcndaryev.html

constexpr int N = 10;
来源：http://hz.bjfxy.top/gtxfwrpcei.html

[S58] C++：命名空间
来源：http://hz.yj202588.top/gtoizraoio.html

namespace ns { int f() { return 1; } }
来源：http://hz.jianghu66.top/gtputyommi.html

[S59] C++：静态断言
来源：http://hz.yj20258888.top/gtjfkzwlie.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cucudq.cn/gtquktponq.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtteqhtymh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtibpjwmis.html

================================================================================
来源：http://hz.gzhubu.top/gtsisakyeo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtxxkhqzoo.html

================================================================================
来源：http://hz.yuxming.cn/gtrjqzjneg.html

[T01] Kotlin：Hello World
来源：http://hz.nwbrower.top/gtklbmdiln.html

println("Hello")
来源：http://hz.hysaishi.cn/gtvcwohkci.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtmtamnznu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtumoijsdp.html

[T03] Kotlin：字符串模板
来源：http://hz.zhaomingkeji.xyz/gtdydkuwzw.html

"值: $b"
来源：http://hz.nanxinkj.top/gtvmfelbjm.html

[T04] Kotlin：空安全
来源：http://hz.yvedp.cn/gtlwmgxpfp.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtomnbteak.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgfzy.top/gtsceoffrr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgufenzy.top/gtnusbnjut.html

[T06] Kotlin：集合映射
来源：http://hz.jinqigufen.top/gtrqglubiu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gtgttdwept.html

[T07] Kotlin：集合过滤
来源：http://hz.sxryk.cn/gtcwxzncwt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhijiandao.cn/gthmoerljs.html

[T08] Kotlin：数据类
来源：http://hz.sysykeji.top/gtsongztts.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtsxivtupf.html

[T09] Kotlin：扩展函数
来源：http://hz.zhiwuduotai.top/gtufwvawjx.html

fun String.exclaim() = this + "!"
来源：http://hz.316326.xyz/gtopxtmevz.html

[T10] Kotlin：默认参数
来源：http://hz.hnxiangtu.top/gtzwllvatm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtvoqmdmqv.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtanwbkses.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sufxvd.cn/gthyukfxds.html

[T12] Kotlin：解构声明
来源：http://hz.ydjk.org.cn/gtuvrwtmor.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinqigufen.top/gtvmbnnzbz.html

[T13] Kotlin：只读 Map
来源：http://hz.xingfuxueyuan.xyz/gtnhvdolto.html

val m = mapOf("a" to 1)
来源：http://hz.guannengcc.top/gticjxonnn.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtwqmmuqwo.html

for (i in 1..10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtlldktjwr.html

[T15] Kotlin：接口
来源：http://hz.hywenlv.cn/gtqgevinkk.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtyzuqcmug.html

[T16] Swift：Hello World
来源：http://hz.gzhubu.top/gtrugwkgas.html

print("Hello")
来源：http://hz.haohaochexian.top/gtgfynxajb.html

[T17] Swift：变量与常量
来源：http://hz.ivvv.top/gtucjtraxl.html

var a = 1;  let b = 2
来源：http://hz.cucudq.cn/gthbnzlsyk.html

[T18] Swift：字符串插值
来源：http://hz.guowangkeji.top/gtjxitgdrg.html

"值: \(b)"
来源：http://hz.sysykeji.top/gtwoubbpcr.html

[T19] Swift：可选绑定
来源：http://hz.jianghu66.top/gtdkrieujx.html

if let n = opt { print(n) }
来源：http://hz.cdnleiting.top/gtyezecxmc.html

[T20] Swift：数组操作
来源：http://hz.gotoacloud.top/gtgmsanktx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hongshengwenyu.top/gtoabizbol.html

[T21] Swift：遍历
来源：http://hz.ywan-chungtsiang.top/gtsqxrwbbj.html

for x in a { print(x) }
来源：http://hz.dianchejie.cn/gtzdqwxwwd.html

[T22] Swift：字典
来源：http://hz.ydjk.org.cn/gtllcsaxla.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aizwys.cn/gtuhthymya.html

[T23] Swift：函数
来源：http://hz.zhiwuduotai.top/gtmurawqcn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yueranfly.top/gtkljyzzfg.html

[T24] Swift：闭包
来源：http://hz.sweek.top/gtcpegyzzy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtbeiqurxk.html

[T25] Swift：结构体
来源：http://hz.sufxvd.cn/gtihmoihlc.html

struct P { var x: Int }
来源：http://hz.cucudq.cn/gtgzfjduge.html

[T26] Swift：类与重写
来源：http://hz.gogol.net.cn/gttdjekiqo.html

class A: Base { override func f() {} }
来源：http://hz.dianchejie.cn/gttytztsrg.html

[T27] Swift：错误处理
来源：http://hz.aizwys.cn/gtpsbkrabg.html

do { try f() } catch { print(error) }
来源：http://hz.kuanghao11.cn/gtcwsrwusq.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtvylyninm.html

enum Color { case red, green }
来源：http://hz.pengpengdd.cyou/gtfonjlpod.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtojqnguzn.html

guard let x = opt else { return }
来源：http://hz.tian-w.cn/gtgwkixlrn.html

[T30] Swift：协议
来源：http://hz.chenlongwang.top/gthvcmdktv.html

protocol Shape { func area() -> Double }
来源：http://hz.jiagoushi.top/gtavmyrsjb.html

[T31] Lua：Hello World
来源：http://hz.tianlin.xyz/gtajgxniou.html

print("Hello")
来源：http://hz.0kj1m.cn/gtswyyheuy.html

[T32] Lua：局部变量
来源：http://hz.mhx1999.top/gtsjpbwvih.html

local a = 1
来源：http://hz.hnxiangtu.top/gtolvrbmpx.html

[T33] Lua：表（数组）
来源：http://hz.hnqzz.top/gtlnjcauol.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gttahkpnls.html

[T34] Lua：遍历表
来源：http://hz.daxiang520.top/gtqrqzthls.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xylfe.cn/gtorjrserp.html

[T35] Lua：字典表
来源：http://hz.xuanzx.com/gtzqhisnsv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hysaishi.cn/gtatorvlbr.html

[T36] Lua：函数
来源：http://hz.guannengcc.top/gtlpbpbeqo.html

function add(a, b) return a + b end
来源：http://hz.vqdsnc.cn/gtnfgtqkgu.html

[T37] Lua：字符串拼接
来源：http://hz.shzxlz.cn/gtorqlersk.html

"a" .. "b"
来源：http://hz.birdmap.top/gttsuikyle.html

[T38] Lua：条件
来源：http://hz.pengpengdd.cyou/gtmntgugit.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtaoykcufq.html

[T39] Lua：模式匹配
来源：http://hz.zhiwuduotai.top/gtvjlfyfnz.html

string.find(s, "%d+")
来源：http://hz.ppjwa.cn/gthocbgoza.html

[T40] Lua：元表
来源：http://hz.bjfxy.top/gtblgjpegq.html

setmetatable({}, { __index = base })
来源：http://hz.yongpay.top/gtzfnexoco.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtreivuudm.html

print "Hello\n";
来源：http://hz.nanxinkj.top/gthfvusdoz.html

[T42] Perl：变量类型
来源：http://hz.zhoulong.xyz/gtapqvqgqn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.daria6918.cn/gtgsciojir.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtmkdidrui.html

"值: $a"
来源：http://hz.dashuyun.cn/gtktphwcev.html

[T44] Perl：条件
来源：http://hz.yuxming.cn/gtmeygfugs.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtsosnnxwx.html

[T45] Perl：数组遍历
来源：http://hz.cdnleiting.top/gteggyngbh.html

for my $x (@arr) { print $x; }
来源：http://hz.tian-w.cn/gtuxvpytzv.html

[T46] Perl：哈希操作
来源：http://hz.shuidangran.top/gtkmkksmat.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sufxvd.cn/gttcttetpe.html

[T47] Perl：正则捕获
来源：http://hz.hammf.cn/gtxnxxpdfg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.meibo888.top/gtmzfvzfbv.html

[T48] Perl：正则替换
来源：http://hz.yongpay.top/gtfxfclvcd.html

$s =~ s/old/new/g;
来源：http://hz.fengsongda.top/gtdqyuztig.html

[T49] Perl：函数
来源：http://hz.jiagoushi.top/gtzmbmidit.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.316326.xyz/gtpdsppjmx.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtfchnzfsm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hfpthk.cn/gtvuizddzx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.pengpengdd.cyou/gtsyuvioij.html

[T51] Scala：Hello World
来源：http://hz.guowangkeji.top/gtbziulbsb.html

println("Hello")
来源：http://hz.ehwqpu.com/gtfcytsuak.html

[T52] Scala：变量
来源：http://hz.ehwqpu.com/gtbwhfdtbg.html

val a = 1;  var b = 2
来源：http://hz.nanxuanxn.top/gtdvintugg.html

[T53] Scala：字符串插值
来源：http://hz.jinghuilouyu.cn/gtckwrjukm.html

s"值: $b"
来源：http://hz.yj20258888.top/gtkixomqkh.html

[T54] Scala：集合映射
来源：http://hz.nanxuanxn.top/gtofwnkphb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258888.top/gthorzvfqm.html

[T55] Scala：集合过滤
来源：http://hz.iojbl.cn/gtuofqeenu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xuanzx.com/gtihosbdyd.html

[T56] Scala：样例类
来源：http://hz.hywenlv.cn/gtltjxkypl.html

case class User(name: String, age: Int)
来源：http://hz.svipenyu.cn/gtgxoxlnus.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtliaetsiw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangdashe.top/gtubjyeynt.html

[T58] Scala：函数定义
来源：http://hz.316326.xyz/gtiucgdmru.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fengsongda.top/gtppecccjy.html

[T59] Scala：循环
来源：http://hz.sufxvd.cn/gtrhrnfzwj.html

for (i <- 1 to 10) println(i)
来源：http://hz.hfpthk.cn/gttqygszpu.html

[T60] Scala：折叠
来源：http://hz.xuanzx.com/gteueiadtd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gotoacloud.top/gtalnwrzjb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvjnisssx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuanzx.com/gtoiawkbtw.html

================================================================================
来源：http://hz.zhixingplan.top/gtslvrrdsz.html

[U01] Py：创建虚拟环境
来源：http://hz.chenzaomai.com/gtzcoxemlm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.svipenyu.cn/gtwowjuvpt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtekcosjsu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.iojbl.cn/gtafoxrqwl.html

[U03] Py：加载 .env 配置
来源：http://hz.redwolf501.top/gttchtwbbf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhoulong.xyz/gtlenjaofy.html

[U04] Py：变量调试打印
来源：http://hz.c1oappe.top/gtcrkzrhha.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yanxiufei.cn/gtcfljbnyp.html

[U05] Py：列表去重且保序
来源：http://hz.svipenyu.cn/gtlulorear.html

list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtiernfkxx.html

[U06] Py：合并两个字典
来源：http://hz.nanxuanxn.top/gtjothrcxp.html

{**a, **b}
来源：http://hz.jinqigufen.top/gtkcnipjqq.html

[U07] Py：反转字典键值
来源：http://hz.nanxuanxn.top/gtfayudrft.html

{v: k for k, v in d.items()}
来源：http://hz.gotoacloud.top/gtswudcpll.html

[U08] Py：展平二维列表
来源：http://hz.ppjwa.cn/gtnnhtwigq.html

[y for x in nested for y in x]
来源：http://hz.ppjwa.cn/gttfoolubr.html

[U09] Py：字典取最大值的键
来源：http://hz.ydjk.org.cn/gtbqcawhmz.html

max(d, key=d.get)
来源：http://hz.yanxiufei.cn/gtistywkdg.html

[U10] Py：按值排序字典
来源：http://hz.cdnleiting.top/gthclebymx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gtkcmdhjfa.html

[U11] Py：生成器表达式
来源：http://hz.shzxlz.cn/gtnstgpwyk.html

(x * 2 for x in arr)
来源：http://hz.wangdashe.top/gtiexsqbpn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gogol.net.cn/gtogctujpx.html

Counter(arr).most_common(3)
来源：http://hz.nanxuanxn.top/gtcsilpqmm.html

[U13] Py：固定长度队列
来源：http://hz.xylfe.cn/gtvppxmtwl.html

deque(maxlen=10)
来源：http://hz.zhongyouzk.top/gtpvhzkwxo.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtstkvyjdn.html

defaultdict(list)
来源：http://hz.redwolf501.top/gtueztpmfn.html

[U15] Py：高精度计时
来源：http://hz.ywan-chungtsiang.top/gttcxtedak.html

t = time.perf_counter()
来源：http://hz.fengsongda.top/gtgfjetyqy.html

[U16] Py：命令行参数解析
来源：http://hz.snrcjt.cn/gtckhxybil.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ydjk.org.cn/gthfswrawg.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gtjczwjsjf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yonumen.top/gtdbexddts.html

[U18] Py：预编译正则
来源：http://hz.jyoumei.cn/gthoduwfaq.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangtech.top/gtrudevxzw.html

[U19] Py：正则替换带回调
来源：http://hz.zhoulong.xyz/gtunznqxow.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenlongwang.top/gtvpiandxg.html

[U20] Py：缓存函数结果
来源：http://hz.fzhhl.top/gtkfurmjtk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hongshengwenyu.top/gtjdecjwwx.html

[U21] Py：自定义上下文管理器
来源：http://hz.xziqi.cn/gtqjkzpzku.html

@contextlib.contextmanager
来源：http://hz.zhijiandao.cn/gtoullxbrs.html

[U22] Py：矩阵转置
来源：http://hz.feifeiyinyue.top/gtmmbhdjsy.html

list(zip(*m))
来源：http://hz.gzhubu.top/gthcalefwe.html

[U23] Py：分块读取大文件
来源：http://hz.daxiang520.top/gttqnbojfu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.guowangkeji.top/gtomjsmmda.html

[U24] Py：路径操作
来源：http://hz.c1oappe.top/gtmwspsjis.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jianghu66.top/gtevmqhtxn.html

[U25] Py：CSV 按字典读
来源：http://hz.ybcxt.top/gtmkkisdvc.html

csv.DictReader(f)
来源：http://hz.ehwqpu.com/gtntpebdwk.html

[U26] Py：并发下载
来源：http://hz.shangyingyoupin.top/gtiiaxbjja.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhixingplan.top/gtipyknltu.html

[U27] Py：异步 HTTP
来源：http://hz.gaohongyu789.top/gtygtjjrnv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtnnpzeflc.html

[U28] Py：类型别名
来源：http://hz.dianchejie.cn/gtnjjznhhx.html

UserId = int
来源：http://hz.tian-w.cn/gtelluvkus.html

[U29] Py：属性校验
来源：http://hz.52xcode.cn/gttkheujzc.html

@property 与 @x.setter 配合
来源：http://hz.xinyue.icu/gteoiycwix.html

[U30] Py：数据类
来源：http://hz.svipenyu.cn/gtkzclszyk.html

@dataclass(slots=True)
来源：http://hz.jinqigufen.top/gtsmswtmaa.html

[U31] Py：单测
来源：http://hz.fengsongda.top/gtehwqqlea.html

python -m pytest -q
来源：http://hz.gzhubu.top/gtrrbzqyap.html

[U32] Py：代码格式化
来源：http://hz.hnqzz.top/gtgwehnxbw.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtsjcgznlg.html

[U33] Py：打包发布
来源：http://hz.fzhhl.top/gtrokzihwy.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.52xcode.cn/gtkkenrusx.html

[U34] Py：判断编码
来源：http://hz.yuxming.cn/gtjxozzwvp.html

chardet.detect(raw)
来源：http://hz.gzhubu.top/gtufokvvpz.html

[U35] Py：发送邮件
来源：http://hz.feifeiyinyue.top/gtfvgigmfm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cucudq.cn/gtadldqztp.html

[U36] Py：定时任务
来源：http://hz.jinghuilouyu.cn/gtpgfejmua.html

schedule.every(10).minutes.do(job)
来源：http://hz.hnqzz.top/gtagsdiuow.html

[U37] Py：读写 Excel
来源：http://hz.aizwys.cn/gtrhmjenbg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydzc1.top/gtkpvapwaa.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenjidiqi.icu/gthpithygc.html

Path(__file__).resolve().parent
来源：http://hz.nanxuanxn.top/gtmpqongaa.html

[U39] Py：判断是否在交互环境
来源：http://hz.jianghu66.top/gtafbfyxsm.html

sys.stdout.isatty()
来源：http://hz.cqqwz.cn/gtqcivqevq.html

[U40] Py：打印到标准错误
来源：http://hz.zhixingplan.top/gtvyxzvqyh.html

print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtknpcxhla.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ydzc1.top/gtnzysbydj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.wangshuangyany.cn/gtzcxnndwd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yuanzhike.top/gtwjtpsdpl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cdnleiting.top/gtpscjriyq.html

[U43] PHP：声明命名空间
来源：http://hz.zhaomingkeji.xyz/gtcpnzerwy.html

namespace App\Http;
来源：http://hz.jianghu66.top/gtvnknvoub.html

[U44] PHP：开启严格类型
来源：http://hz.cashguo.top/gtdjtlxofn.html

declare(strict_types=1);
来源：http://hz.fzhhl.top/gtkrqnocyx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.feifeiyinyue.top/gtpvlpjvdc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtmnpslxzt.html

[U46] PHP：可空类型
来源：http://hz.shangyingyoupin.top/gtzbcxzvii.html

?string $name = null
来源：http://hz.wangdashe.top/gtvxhbnfov.html

[U47] PHP：联合类型
来源：http://hz.wangdashe.top/gticjcufff.html

int|string $id
来源：http://hz.sysykeji.top/gtyhndrbwl.html

[U48] PHP：纯枚举
来源：http://hz.yj20258.top/gtdylvvgpy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cdnleiting.top/gtyqjpoeub.html

[U49] PHP：只读属性
来源：http://hz.yuanzhike.top/gtvsyfnvzu.html

public readonly string $name
来源：http://hz.tanke756.top/gtuhgarqdz.html

[U50] PHP：构造器属性提升
来源：http://hz.hfpthk.cn/gtixdfcspz.html

public function __construct(private int $id) {}
来源：http://hz.aibaodan.cn/gtforkqdst.html

[U51] PHP：数组解构
来源：http://hz.gzhubu.top/gtcfuxxgxf.html

[$a, $b] = $arr;
来源：http://hz.daxiang520.top/gtjiztmifi.html

[U52] PHP：箭头函数
来源：http://hz.sufxvd.cn/gtbfyvkdez.html

$double = fn($x) => $x * 2;
来源：http://hz.shzxlz.cn/gtlggtbwxc.html

[U53] PHP：空合并运算符
来源：http://hz.meibo888.top/gtxjccggwv.html

$v = $a ?? $b ?? "default";
来源：http://hz.meibo888.top/gtmqjlkgqh.html

[U54] PHP：空安全调用
来源：http://hz.xuanzx.com/gtygpijcsv.html

$obj?->method()
来源：http://hz.pengpengdd.cyou/gttnsslarw.html

[U55] PHP：match 表达式
来源：http://hz.jinghuilouyu.cn/gtocimpgkr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ivvv.top/gtjxlshxwb.html

[U56] PHP：命名参数
来源：http://hz.mhx1999.top/gtttnxysfv.html

f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtcrylgxki.html

[U57] PHP：字符串插值
来源：http://hz.ydjk.org.cn/gttqihvpsa.html

"值: {$a}"
来源：http://hz.xziqi.cn/gtidomttfg.html

[U58] PHP：数组三件套
来源：http://hz.hywenlv.cn/gtrrgevsuz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtpgioagah.html

[U59] PHP：自定义排序
来源：http://hz.yonumen.top/gtwgrclska.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtayfluoly.html

[U60] PHP：JSON 编解码
来源：http://hz.sweek.top/gtyfviljqa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jlsjyb.cn/gtlhkjxcsp.html

[U61] PHP：正则
来源：http://hz.wangdashe.top/gtqlvujndm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jlsjyb.cn/gtctdoincz.html

[U62] PHP：日期对象
来源：http://hz.zhoulong.xyz/gtwbsgovdr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigfzy.top/gtsdmkzhag.html

[U63] PHP：文件读写
来源：http://hz.hnqzz.top/gtacfqnhci.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.c1oappe.top/gtoefrjebx.html

[U64] PHP：目录遍历
来源：http://hz.yj20258888.top/gtvttbpmic.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xuetiantiany.cn/gtemixmocq.html

[U65] PHP：会话
来源：http://hz.hnxiangtu.top/gtxilufxge.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.xinyue.icu/gthjrbbfgo.html

[U66] PHP：设置 Cookie
来源：http://hz.pycfn.com/gtbbriepfx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.pengpengdd.cyou/gtlewmoctn.html

[U67] PHP：处理文件上传
来源：http://hz.zhaomingkeji.xyz/gtvlfqxbtx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.chenjidiqi.icu/gtxzwmlxqj.html

[U68] PHP：PDO 连接
来源：http://hz.daria6918.cn/gtdoqmcoqj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigfzy.top/gtiridwwvh.html

[U69] PHP：PDO 预处理
来源：http://hz.316326.xyz/gttyprezcv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.hywenlv.cn/gtbalbkutw.html

[U70] PHP：PDO 事务
来源：http://hz.zhongyouzk.top/gtetgxkpug.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xuanzx.com/gtughuxwnp.html

[U71] PHP：抛出异常
来源：http://hz.xuetiantiany.cn/gtdzrlrzra.html

throw new RuntimeException("失败", 500);
来源：http://hz.quarkkingdee.top/gtdmnfsukp.html

[U72] PHP：写错误日志
来源：http://hz.chenjidiqi.icu/gtanqoiwas.html

error_log("失败: " . $e->getMessage());
来源：http://hz.316326.xyz/gtmtwpodld.html

[U73] PHP：读取 ini 配置
来源：http://hz.shanyushiyangkeji.top/gtdvlwgavu.html

parse_ini_file("config.ini", true)
来源：http://hz.wangdashe.top/gtxhupxqlt.html

[U74] PHP：读取环境变量
来源：http://hz.yangfankeji.com/gtctdajtix.html

getenv("APP_ENV") ?: "production"
来源：http://hz.haohaochexian.top/gtvesregoj.html

[U75] PHP：依赖注入
来源：http://hz.hammf.cn/gtqfxflmja.html

composer require psr/container
来源：http://hz.yj202588.top/gthrnwxpap.html

[U76] PHP：简单路由
来源：http://hz.xylfe.cn/gtlzgjlxym.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aibaodan.cn/gtabldmmhk.html

[U77] PHP：模板渲染
来源：http://hz.xylfe.cn/gtzrlevfvy.html

composer require twig/twig
来源：http://hz.jqgfzy.top/gtwqvddyxo.html

[U78] PHP：单元测试
来源：http://hz.yj20258888.top/gtbvgaeitz.html

composer require --dev phpunit/phpunit
来源：http://hz.aizwys.cn/gttagkzucu.html


<!-- 参考信息 -->