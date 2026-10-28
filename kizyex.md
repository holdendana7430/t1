代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtzjbcmymz.html

[S51] C++：显式类型转换
来源：http://hz.meibo888.top/gtilziigzp.html

static_cast<double>(a) / b
来源：http://hz.zhijiandao.cn/gtzwuqlgit.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtavwmyjsd.html

int size() const noexcept { return n_; }
来源：http://hz.nwbrower.top/gtispdpxty.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtnhhocevh.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtpdrlnskn.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gtoilfhfrg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangshuangyany.cn/gttzukzjpm.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtyzzwubfh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtvtrudunk.html

[S56] C++：optional
来源：http://hz.xuanzx.com/gtoauynhij.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtzlrspzyb.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gttwxnccib.html

constexpr int N = 10;
来源：http://hz.havefunace.top/gtkvmnxytf.html

[S58] C++：命名空间
来源：http://hz.xingfuxueyuan.xyz/gtiydtxhqt.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtobwqetpw.html

[S59] C++：静态断言
来源：http://hz.jqgfzy.top/gtfwwyzgmf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gtkjhdwnsb.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gttsinivfj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtwzwsqcpk.html

================================================================================
来源：http://hz.sufxvd.cn/gtwfigwcrc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtrpysqsxp.html

================================================================================
来源：http://hz.hnqzz.top/gtlcdygbcv.html

[T01] Kotlin：Hello World
来源：http://hz.zhaomingkeji.xyz/gtuweqoxfl.html

println("Hello")
来源：http://hz.nanxinkj.top/gtkbkzawll.html

[T02] Kotlin：变量
来源：http://hz.jinghuilouyu.cn/gtstaqkdfw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinghuilouyu.cn/gtxdwbjezn.html

[T03] Kotlin：字符串模板
来源：http://hz.tian-w.cn/gtsbnxxove.html

"值: $b"
来源：http://hz.xingfuxueyuan.xyz/gtquqxfurn.html

[T04] Kotlin：空安全
来源：http://hz.xuanzx.com/gtfymqttjr.html

val n: String? = null;  n?.length
来源：http://hz.yuxming.cn/gtwnrlpcck.html

[T05] Kotlin：when 表达式
来源：http://hz.xingfuxueyuan.xyz/gtoeazazjq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtdmyfqwhg.html

[T06] Kotlin：集合映射
来源：http://hz.ydzc1.top/gtnjkrqpiv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtiddqnfsr.html

[T07] Kotlin：集合过滤
来源：http://hz.shzxlz.cn/gtvjtjleqo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxinkj.top/gtfpfvodct.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gtkvdiugch.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtvggtheii.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gttnobzzew.html

fun String.exclaim() = this + "!"
来源：http://hz.shanyushiyangkeji.top/gtgvhfgcng.html

[T10] Kotlin：默认参数
来源：http://hz.meibo888.top/gtpchtajdx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aibaodan.cn/gtgytknhux.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtvsvcazlk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtzncgzbsm.html

[T12] Kotlin：解构声明
来源：http://hz.shuidangran.top/gtbojnhbej.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtuklpsmvm.html

[T13] Kotlin：只读 Map
来源：http://hz.daria6918.cn/gtilurawpa.html

val m = mapOf("a" to 1)
来源：http://hz.ehwqpu.com/gtikurvxjm.html

[T14] Kotlin：循环
来源：http://hz.aibaodan.cn/gtsadnprfn.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtmfycdbbq.html

[T15] Kotlin：接口
来源：http://hz.yanxiufei.cn/gtcaxgckai.html

interface Shape { fun area(): Double }
来源：http://hz.jqgfzy.top/gtqgwqbddx.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtxzlztgto.html

print("Hello")
来源：http://hz.sweek.top/gtavqdafei.html

[T17] Swift：变量与常量
来源：http://hz.andypj.xyz/gtsahyekcd.html

var a = 1;  let b = 2
来源：http://hz.ydzc1.top/gthciplgxw.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gthiusyndc.html

"值: \(b)"
来源：http://hz.guannengcc.top/gtnfpsvfcx.html

[T19] Swift：可选绑定
来源：http://hz.iojbl.cn/gtzvjxgdyb.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtvmwsgsdv.html

[T20] Swift：数组操作
来源：http://hz.iojbl.cn/gthihkjvth.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jyoumei.cn/gtabhdrqvv.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtzrzlwgti.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtloqbkliy.html

[T22] Swift：字典
来源：http://hz.nwbrower.top/gtegzmuktk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtzmhrkrer.html

[T23] Swift：函数
来源：http://hz.nanxuanxn.top/gtgqgsuwep.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pengpengdd.cyou/gtctmwzuse.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtqlqyfnug.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtcokkpobl.html

[T25] Swift：结构体
来源：http://hz.hnqzz.top/gtqhcucklk.html

struct P { var x: Int }
来源：http://hz.ydjk.org.cn/gtcmptdbxb.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gthmenmhxz.html

class A: Base { override func f() {} }
来源：http://hz.hywenlv.cn/gtnfflzets.html

[T27] Swift：错误处理
来源：http://hz.jqgufenzy.top/gtlqvnsmgm.html

do { try f() } catch { print(error) }
来源：http://hz.svipenyu.cn/gtdpvfheou.html

[T28] Swift：枚举
来源：http://hz.cheryme.top/gtlvurhkdq.html

enum Color { case red, green }
来源：http://hz.gaohongyu789.top/gtsmtwczco.html

[T29] Swift：guard 提前返回
来源：http://hz.tanke756.top/gtuvguelbt.html

guard let x = opt else { return }
来源：http://hz.feifeiyinyue.top/gtyjcnebpl.html

[T30] Swift：协议
来源：http://hz.vqdsnc.cn/gtzcddxpyz.html

protocol Shape { func area() -> Double }
来源：http://hz.ivvv.top/gtaewmkwaq.html

[T31] Lua：Hello World
来源：http://hz.svipenyu.cn/gtzafkpkjv.html

print("Hello")
来源：http://hz.ybcxt.top/gtdywrjcbj.html

[T32] Lua：局部变量
来源：http://hz.pycfn.com/gtqwfzriee.html

local a = 1
来源：http://hz.316326.xyz/gtratjjmfw.html

[T33] Lua：表（数组）
来源：http://hz.birdmap.top/gtkafbzite.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.316326.xyz/gtxqbzffvh.html

[T34] Lua：遍历表
来源：http://hz.chenzaomai.com/gttonzbnvt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtgeuzxxcm.html

[T35] Lua：字典表
来源：http://hz.sxryk.cn/gtwzcouvaz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nanxinkj.top/gtkrzxdjyl.html

[T36] Lua：函数
来源：http://hz.jinqigufen.top/gtcbinwmci.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangtech.top/gtagbrhmct.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtvhatlqtq.html

"a" .. "b"
来源：http://hz.nanxinkj.top/gtubhxqxkj.html

[T38] Lua：条件
来源：http://hz.snrcjt.cn/gtahkbxmsb.html

if x > 0 then print("正") end
来源：http://hz.pycfn.com/gtwefifswg.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtlxixzjil.html

string.find(s, "%d+")
来源：http://hz.gzhubu.top/gtzrxkljcp.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtljzkdmcl.html

setmetatable({}, { __index = base })
来源：http://hz.xinyue.icu/gtfdckewpa.html

[T41] Perl：Hello World
来源：http://hz.tanke756.top/gthokffdga.html

print "Hello\n";
来源：http://hz.xylfe.cn/gtezquovth.html

[T42] Perl：变量类型
来源：http://hz.gzhubu.top/gtymmqoszl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtktefdqsc.html

[T43] Perl：字符串插值
来源：http://hz.zycfv.cn/gtgtmmpmbi.html

"值: $a"
来源：http://hz.tian-w.cn/gtebilxlam.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtasqypnff.html

if ($a > 0) { print "正"; }
来源：http://hz.jyoumei.cn/gtptqypfom.html

[T45] Perl：数组遍历
来源：http://hz.zhijiandao.cn/gtovobduwx.html

for my $x (@arr) { print $x; }
来源：http://hz.hysaishi.cn/gttwdqvdck.html

[T46] Perl：哈希操作
来源：http://hz.shanyushiyangtech.top/gtfbxdregj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.mhx1999.top/gtwowccdss.html

[T47] Perl：正则捕获
来源：http://hz.havefunace.top/gtcofnhwqp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yueranfly.top/gtogyfdwtn.html

[T48] Perl：正则替换
来源：http://hz.zhijiandao.cn/gtzxhfxlcv.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtozqdczdh.html

[T49] Perl：函数
来源：http://hz.svipenyu.cn/gtgzywbter.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ppjwa.cn/gtwlqalrnm.html

[T50] Perl：逐行读文件
来源：http://hz.tianlin.xyz/gtripaqajk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tianlin.xyz/gtwcwunuhp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xylfe.cn/gtgbnzeuqy.html

[T51] Scala：Hello World
来源：http://hz.zhongyouzk.top/gtnomwpjsd.html

println("Hello")
来源：http://hz.yj202588.top/gtdasizrfk.html

[T52] Scala：变量
来源：http://hz.aizwys.cn/gtzmaikbuu.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtcvnhudwu.html

[T53] Scala：字符串插值
来源：http://hz.zhiwuduotai.top/gtscxsnkfq.html

s"值: $b"
来源：http://hz.yonumen.top/gtozcgtiwm.html

[T54] Scala：集合映射
来源：http://hz.jyoumei.cn/gtwpsaeadl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cashguo.top/gtqqhqtxtm.html

[T55] Scala：集合过滤
来源：http://hz.yonumen.top/gtujxfilzz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tianlin.xyz/gtsvaexnjk.html

[T56] Scala：样例类
来源：http://hz.bjfxy.top/gtnuujzwlg.html

case class User(name: String, age: Int)
来源：http://hz.cdnleiting.top/gtpdoakrmw.html

[T57] Scala：模式匹配
来源：http://hz.0kj1m.cn/gthcgboguq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tian-w.cn/gtcuiiloma.html

[T58] Scala：函数定义
来源：http://hz.jqgufenzy.top/gtgucswrpe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cqqwz.cn/gtqrxdfxgo.html

[T59] Scala：循环
来源：http://hz.9152youxi.cn/gttbfhuxes.html

for (i <- 1 to 10) println(i)
来源：http://hz.kuanghao11.cn/gtugsynezh.html

[T60] Scala：折叠
来源：http://hz.smart0.xyz/gtppsfesmu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.smart0.xyz/gtdrqwfheg.html

================================================================================
来源：http://hz.chenlongwang.top/gtdlohxpxq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ppjwa.cn/gteykgsgzi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtttbbdmkm.html

[U01] Py：创建虚拟环境
来源：http://hz.jinqigufen.top/gtxnounlnu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zdqjudy.top/gthgpxvfaa.html

[U02] Py：导出 / 安装依赖
来源：http://hz.wangdashe.top/gtoilrsgax.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xingfuxueyuan.xyz/gtqjctqkpz.html

[U03] Py：加载 .env 配置
来源：http://hz.zdqjudy.top/gtbbrqhqje.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gtkgiqarbp.html

[U04] Py：变量调试打印
来源：http://hz.zhoulong.xyz/gtkistejvs.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.shzxlz.cn/gtwxcgwyie.html

[U05] Py：列表去重且保序
来源：http://hz.ywan-chungtsiang.top/gtejtzzerd.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtdnmfqtnq.html

[U06] Py：合并两个字典
来源：http://hz.yuanzhike.top/gthjirzdpo.html

{**a, **b}
来源：http://hz.pengpengdd.cyou/gtejyxopbv.html

[U07] Py：反转字典键值
来源：http://hz.zhengqikj.top/gtrkfaaeyr.html

{v: k for k, v in d.items()}
来源：http://hz.jinqigfzy.top/gtishobvct.html

[U08] Py：展平二维列表
来源：http://hz.xinyue.icu/gtsmemwjga.html

[y for x in nested for y in x]
来源：http://hz.mhx1999.top/gtcptidwno.html

[U09] Py：字典取最大值的键
来源：http://hz.xingfuxueyuan.xyz/gtwgryxlal.html

max(d, key=d.get)
来源：http://hz.smart0.xyz/gtjsnownpk.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtykswkddj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hnqzz.top/gtgxcgqcfg.html

[U11] Py：生成器表达式
来源：http://hz.shzxlz.cn/gteqrfbwki.html

(x * 2 for x in arr)
来源：http://hz.wangdashe.top/gtyrxbwdfc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.feifeiyinyue.top/gtoyploobe.html

Counter(arr).most_common(3)
来源：http://hz.nwbrower.top/gtubnjihwl.html

[U13] Py：固定长度队列
来源：http://hz.gaohongyu789.top/gtuuimmola.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtztezuvny.html

[U14] Py：分组收集到列表
来源：http://hz.tanke756.top/gtxzsxbdfs.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtumduukez.html

[U15] Py：高精度计时
来源：http://hz.nanxinkj.top/gteymopshh.html

t = time.perf_counter()
来源：http://hz.zhongyouzk.top/gtsftzchhl.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtassmtdun.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtavdcpoat.html

[U17] Py：初始化日志
来源：http://hz.xziqi.cn/gtmhrhpejq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.vqdsnc.cn/gtpeubvwum.html

[U18] Py：预编译正则
来源：http://hz.yanxiufei.cn/gtxueytvhg.html

pat = re.compile(r"\d+")
来源：http://hz.daxiang520.top/gtfbldnuup.html

[U19] Py：正则替换带回调
来源：http://hz.hfpthk.cn/gtvjovkczv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtklcpttyc.html

[U20] Py：缓存函数结果
来源：http://hz.sweek.top/gtjbugoakm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xuetiantiany.cn/gtdhsdwehm.html

[U21] Py：自定义上下文管理器
来源：http://hz.jyoumei.cn/gtqgayfmsr.html

@contextlib.contextmanager
来源：http://hz.gogol.net.cn/gtrshxfqxx.html

[U22] Py：矩阵转置
来源：http://hz.shuidangran.top/gtfjnrvotk.html

list(zip(*m))
来源：http://hz.yueranfly.top/gteaivkueq.html

[U23] Py：分块读取大文件
来源：http://hz.ppjwa.cn/gtmgvitmyx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.smart0.xyz/gtjzayebpr.html

[U24] Py：路径操作
来源：http://hz.ivvv.top/gtadcxeyxz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.kuanghao11.cn/gtfkicxdrq.html

[U25] Py：CSV 按字典读
来源：http://hz.andypj.xyz/gtmquylkpd.html

csv.DictReader(f)
来源：http://hz.wangshuangyany.cn/gtdekredlr.html

[U26] Py：并发下载
来源：http://hz.jiagoushi.top/gtckpychiw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aibaodan.cn/gthtaafsua.html

[U27] Py：异步 HTTP
来源：http://hz.jqgfzy.top/gtlmooovqc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xziqi.cn/gtreglnzxp.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtlrxqucyv.html

UserId = int
来源：http://hz.svipenyu.cn/gtrlktkcjz.html

[U29] Py：属性校验
来源：http://hz.yj20258888.top/gtrqaqdpev.html

@property 与 @x.setter 配合
来源：http://hz.hnxiangtu.top/gtatrmzfvx.html

[U30] Py：数据类
来源：http://hz.jinghuilouyu.cn/gtycohflqp.html

@dataclass(slots=True)
来源：http://hz.fengsongda.top/gtnesgrsgd.html

[U31] Py：单测
来源：http://hz.sufxvd.cn/gtkllytmcs.html

python -m pytest -q
来源：http://hz.xingfuxueyuan.xyz/gtrcqgposo.html

[U32] Py：代码格式化
来源：http://hz.zhoulong.xyz/gttixkntdd.html

ruff format . && ruff check --fix .
来源：http://hz.zycfv.cn/gtdjrpcpct.html

[U33] Py：打包发布
来源：http://hz.yueranfly.top/gtkjyywvzn.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.feifeiyinyue.top/gtuerhrzku.html

[U34] Py：判断编码
来源：http://hz.tanke756.top/gtmktxkdes.html

chardet.detect(raw)
来源：http://hz.hywenlv.cn/gtxfapkyro.html

[U35] Py：发送邮件
来源：http://hz.yvedp.cn/gtgeodtccg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.feifeiyinyue.top/gtrxkulpul.html

[U36] Py：定时任务
来源：http://hz.ehwqpu.com/gtstmecoow.html

schedule.every(10).minutes.do(job)
来源：http://hz.ivvv.top/gtowycwzgy.html

[U37] Py：读写 Excel
来源：http://hz.xinyue.icu/gtzormsbru.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yueranfly.top/gtdrjbyxga.html

[U38] Py：获取脚本所在目录
来源：http://hz.aibaodan.cn/gtfowmfcet.html

Path(__file__).resolve().parent
来源：http://hz.tian-w.cn/gtcwlogvzy.html

[U39] Py：判断是否在交互环境
来源：http://hz.yuxming.cn/gtthbagxli.html

sys.stdout.isatty()
来源：http://hz.chenlongwang.top/gtqmksxrah.html

[U40] Py：打印到标准错误
来源：http://hz.sysykeji.top/gtnrxdhcds.html

print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtstdhyvlr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gotoacloud.top/gtdfvbedyn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtnojzirso.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gotoacloud.top/gttfxjzsaa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.c1oappe.top/gtnyrlkqxn.html

[U43] PHP：声明命名空间
来源：http://hz.jiagoushi.top/gtgosmdxrj.html

namespace App\Http;
来源：http://hz.tanke756.top/gtrzkcrekn.html

[U44] PHP：开启严格类型
来源：http://hz.pengpengdd.cyou/gtkfqprxnz.html

declare(strict_types=1);
来源：http://hz.ydjk.org.cn/gtmnhmtsvz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cashguo.top/gtjojpdwzt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtecxvysmk.html

[U46] PHP：可空类型
来源：http://hz.yangfankeji.com/gtvaigqxqg.html

?string $name = null
来源：http://hz.feifeiyinyue.top/gtucvlieql.html

[U47] PHP：联合类型
来源：http://hz.nwbrower.top/gtkfeecruk.html

int|string $id
来源：http://hz.yongpay.top/gtevrhbcru.html

[U48] PHP：纯枚举
来源：http://hz.ywan-chungtsiang.top/gtpxayeird.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigufen.top/gtwrgjxoyh.html

[U49] PHP：只读属性
来源：http://hz.zycfv.cn/gttvdllitk.html

public readonly string $name
来源：http://hz.dianchejie.cn/gtwmxspjnc.html

[U50] PHP：构造器属性提升
来源：http://hz.cdnleiting.top/gtuqppgvhy.html

public function __construct(private int $id) {}
来源：http://hz.guannengcc.top/gtllwrmuyg.html

[U51] PHP：数组解构
来源：http://hz.yanxiufei.cn/gtmjvfrocq.html

[$a, $b] = $arr;
来源：http://hz.zhengqikj.top/gtiozxvpfd.html

[U52] PHP：箭头函数
来源：http://hz.ehwqpu.com/gtrithhglh.html

$double = fn($x) => $x * 2;
来源：http://hz.xingfuxueyuan.xyz/gtzphotgdu.html

[U53] PHP：空合并运算符
来源：http://hz.hammf.cn/gtqrzgbmsp.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhiwuduotai.top/gtyprtlibl.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtxktwenxq.html

$obj?->method()
来源：http://hz.jiagoushi.top/gtgyuuizns.html

[U55] PHP：match 表达式
来源：http://hz.pycfn.com/gtnsugptum.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.snrcjt.cn/gtwmpkywqm.html

[U56] PHP：命名参数
来源：http://hz.chenjidiqi.icu/gtedoulohx.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtxgqshgwn.html

[U57] PHP：字符串插值
来源：http://hz.jyoumei.cn/gtienoujbd.html

"值: {$a}"
来源：http://hz.jinghuilouyu.cn/gtuxfvvwqv.html

[U58] PHP：数组三件套
来源：http://hz.daxiang520.top/gtljprbbuy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jianghu66.top/gtliqnxvws.html

[U59] PHP：自定义排序
来源：http://hz.pycfn.com/gtteewvsnp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtvvwxoypy.html

[U60] PHP：JSON 编解码
来源：http://hz.jyoumei.cn/gtcxfvzbii.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cqqwz.cn/gtywfqovnn.html

[U61] PHP：正则
来源：http://hz.guannengcc.top/gtpfodgjro.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtjafbebjc.html

[U62] PHP：日期对象
来源：http://hz.sxryk.cn/gtqsuwxjvg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.316326.xyz/gtcxhixmle.html

[U63] PHP：文件读写
来源：http://hz.dianchejie.cn/gtfgoqqtdl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jqgufenzy.top/gtckroddko.html

[U64] PHP：目录遍历
来源：http://hz.gotoacloud.top/gtlakvfofo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cdnleiting.top/gtrdkapwyr.html

[U65] PHP：会话
来源：http://hz.hongshengwenyu.top/gtaydswjwb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.feifeiyinyue.top/gtqsfqgeeq.html

[U66] PHP：设置 Cookie
来源：http://hz.cashguo.top/gtjksoomwj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.xingfuxueyuan.xyz/gtwqraewvk.html

[U67] PHP：处理文件上传
来源：http://hz.mhx1999.top/gtkbvowxww.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gogol.net.cn/gtnkeiolou.html

[U68] PHP：PDO 连接
来源：http://hz.gzhubu.top/gtpcnptyrc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sysykeji.top/gtywaoqvnz.html

[U69] PHP：PDO 预处理
来源：http://hz.hnqzz.top/gtqmfqahly.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.tian-w.cn/gtsyoiuoxc.html

[U70] PHP：PDO 事务
来源：http://hz.xuanzx.com/gtlvdqcspr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jqgufenzy.top/gtrjeruqds.html

[U71] PHP：抛出异常
来源：http://hz.zhijiandao.cn/gteltspvcq.html

throw new RuntimeException("失败", 500);
来源：http://hz.redwolf501.top/gtntwxslmn.html

[U72] PHP：写错误日志
来源：http://hz.cashguo.top/gtckjyepnw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.wangshuangyany.cn/gtwxblhvaw.html

[U73] PHP：读取 ini 配置
来源：http://hz.c1oappe.top/gtyduumgnu.html

parse_ini_file("config.ini", true)
来源：http://hz.ppjwa.cn/gtjdacgokc.html

[U74] PHP：读取环境变量
来源：http://hz.316326.xyz/gtigeerswv.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xingfuxueyuan.xyz/gtwwunpuwb.html

[U75] PHP：依赖注入
来源：http://hz.xziqi.cn/gtfwtqqheg.html

composer require psr/container
来源：http://hz.ppjwa.cn/gtizhxnrss.html

[U76] PHP：简单路由
来源：http://hz.jinyuanbaomall.cn/gtdwsopawx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ybcxt.top/gtkiepyxci.html


<!-- 参考信息 -->