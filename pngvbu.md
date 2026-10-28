代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.bjfxy.top/gtofkuyynw.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtzkqwipqj.html

static_cast<double>(a) / b
来源：http://hz.nanxuanxn.top/gtvtgvvefa.html

[S52] C++：const 与 noexcept
来源：http://hz.xingfuxueyuan.xyz/gtvnhdsdwx.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtuxqqrzwa.html

[S53] C++：移动语义
来源：http://hz.cucudq.cn/gtxiajgjmw.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtstlxcqto.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtludqtjte.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dashuyun.cn/gtjhqdgfpv.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gtmimvtuwb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtonswyfhl.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtnjufvnnl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhoulong.xyz/gtrctskcgt.html

[S57] C++：编译期常量
来源：http://hz.daxiang520.top/gtpjewdfrj.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtfvzydizb.html

[S58] C++：命名空间
来源：http://hz.9152youxi.cn/gtlojdlxgb.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxinkj.top/gtsiwlldzw.html

[S59] C++：静态断言
来源：http://hz.cheryme.top/gtpcffykit.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtpthlkatd.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtgoaqsrwh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gthjenkhjl.html

================================================================================
来源：http://hz.316326.xyz/gthaolyzkk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtscofqavs.html

================================================================================
来源：http://hz.yueranfly.top/gtkazzopjy.html

[T01] Kotlin：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtgwsmoudq.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtuhweviro.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtzuxteujr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cashguo.top/gtwsfqdxlk.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gtogyqvyot.html

"值: $b"
来源：http://hz.daxiang520.top/gtrvitsblr.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gtgjimhlys.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtbbuulqsz.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258888.top/gtsmtsnfut.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yongpay.top/gtwfbbekxn.html

[T06] Kotlin：集合映射
来源：http://hz.zycfv.cn/gtozibebur.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtwpgztivl.html

[T07] Kotlin：集合过滤
来源：http://hz.shzxlz.cn/gtwdzjndxt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.wangshuangyany.cn/gtisqnhoko.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtxpjbczis.html

data class User(val name: String, val age: Int)
来源：http://hz.shanyushiyangtech.top/gtnoqzxusk.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtzyuicjta.html

fun String.exclaim() = this + "!"
来源：http://hz.zhongyouzk.top/gtfvlvnyhr.html

[T10] Kotlin：默认参数
来源：http://hz.xuanzx.com/gtmudxygwz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fengsongda.top/gtylbzpfxh.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtrcqgllvy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.redwolf501.top/gtjwihwljr.html

[T12] Kotlin：解构声明
来源：http://hz.iojbl.cn/gtlvxcbrmx.html

val (a, b) = Pair(1, 2)
来源：http://hz.tianlin.xyz/gtvrskubce.html

[T13] Kotlin：只读 Map
来源：http://hz.jinyuanbaomall.cn/gtohqhuavv.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtzglziawt.html

[T14] Kotlin：循环
来源：http://hz.zhiwuduotai.top/gtytbkkyfl.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtwzmyvhlx.html

[T15] Kotlin：接口
来源：http://hz.sxryk.cn/gtvzevdebu.html

interface Shape { fun area(): Double }
来源：http://hz.cashguo.top/gtjqesljpz.html

[T16] Swift：Hello World
来源：http://hz.gzhubu.top/gtxrmooeuw.html

print("Hello")
来源：http://hz.daria6918.cn/gtebgegluo.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gtyksstbok.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtzaziakih.html

[T18] Swift：字符串插值
来源：http://hz.fzhhl.top/gttawpnpot.html

"值: \(b)"
来源：http://hz.tanke756.top/gtsnsgjxui.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gtkiwilqvp.html

if let n = opt { print(n) }
来源：http://hz.jianghu66.top/gtpozjedtz.html

[T20] Swift：数组操作
来源：http://hz.ivvv.top/gtidvwjaub.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.meibo888.top/gtfhphyegn.html

[T21] Swift：遍历
来源：http://hz.chenjidiqi.icu/gtketsrlod.html

for x in a { print(x) }
来源：http://hz.pengpengdd.cyou/gtqttglfwi.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gtbdadoung.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.vqdsnc.cn/gtyyryolhk.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gtnbwveaqg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yj20258.top/gtddzsryeo.html

[T24] Swift：闭包
来源：http://hz.hfpthk.cn/gtuildgdge.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtthfqeghb.html

[T25] Swift：结构体
来源：http://hz.hongshengwenyu.top/gtsdvnpffe.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gtvrtrwtzd.html

[T26] Swift：类与重写
来源：http://hz.ywan-chungtsiang.top/gtdetjuyuz.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtasuuopqk.html

[T27] Swift：错误处理
来源：http://hz.cashguo.top/gtfnjzgzwb.html

do { try f() } catch { print(error) }
来源：http://hz.cucudq.cn/gtzysevrhq.html

[T28] Swift：枚举
来源：http://hz.hammf.cn/gtjnjetntn.html

enum Color { case red, green }
来源：http://hz.kuanghao11.cn/gtgakcerpd.html

[T29] Swift：guard 提前返回
来源：http://hz.fzhhl.top/gtrhccuuxq.html

guard let x = opt else { return }
来源：http://hz.chenjidiqi.icu/gttsegduzo.html

[T30] Swift：协议
来源：http://hz.smart0.xyz/gthhlbquoz.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigufen.top/gtgjzcguyy.html

[T31] Lua：Hello World
来源：http://hz.pengpengdd.cyou/gtkoxzmukq.html

print("Hello")
来源：http://hz.dianchejie.cn/gtsctptepz.html

[T32] Lua：局部变量
来源：http://hz.ydzc1.top/gtmvirpoth.html

local a = 1
来源：http://hz.pengpengdd.cyou/gtnybqpbsl.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtcdkabgkn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtvyuyaszq.html

[T34] Lua：遍历表
来源：http://hz.xylfe.cn/gtxqpeybhx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtpjaahyqm.html

[T35] Lua：字典表
来源：http://hz.jinqigfzy.top/gtufwpffar.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jiagoushi.top/gtrlnkoviy.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtufdyeyzf.html

function add(a, b) return a + b end
来源：http://hz.ybcxt.top/gtsnzfpubp.html

[T37] Lua：字符串拼接
来源：http://hz.yj20258.top/gtneriibkk.html

"a" .. "b"
来源：http://hz.jinyuanbaomall.cn/gtjapslzqn.html

[T38] Lua：条件
来源：http://hz.jyoumei.cn/gtjpeqdnnk.html

if x > 0 then print("正") end
来源：http://hz.yj20258888.top/gtewtnomvf.html

[T39] Lua：模式匹配
来源：http://hz.ybcxt.top/gtjzxhyyhh.html

string.find(s, "%d+")
来源：http://hz.aizwys.cn/gtipsgqgff.html

[T40] Lua：元表
来源：http://hz.chenzaomai.com/gtflabqzqb.html

setmetatable({}, { __index = base })
来源：http://hz.yvedp.cn/gtfcvcyxlv.html

[T41] Perl：Hello World
来源：http://hz.pengpengdd.cyou/gtquywrmmy.html

print "Hello\n";
来源：http://hz.zdqjudy.top/gtgfmkvgzm.html

[T42] Perl：变量类型
来源：http://hz.zhengqikj.top/gtglxqbvbj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shangyingyoupin.top/gtsinnaboa.html

[T43] Perl：字符串插值
来源：http://hz.shzxlz.cn/gtgxhldaps.html

"值: $a"
来源：http://hz.iojbl.cn/gtqytpgscg.html

[T44] Perl：条件
来源：http://hz.quarkkingdee.top/gtlhpqjowf.html

if ($a > 0) { print "正"; }
来源：http://hz.hysaishi.cn/gtcazlejvc.html

[T45] Perl：数组遍历
来源：http://hz.sysykeji.top/gtngufszxn.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtkaasiibl.html

[T46] Perl：哈希操作
来源：http://hz.gaohongyu789.top/gtasmqdzul.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhaomingkeji.xyz/gteesmhmku.html

[T47] Perl：正则捕获
来源：http://hz.gotoacloud.top/gtxkkhiifj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cheryme.top/gtfcyddnzh.html

[T48] Perl：正则替换
来源：http://hz.jinyuanbaomall.cn/gtpnqrplmf.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtzmhrkqjp.html

[T49] Perl：函数
来源：http://hz.zhoulong.xyz/gtgmvmwtyd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ehwqpu.com/gtfndbfxxv.html

[T50] Perl：逐行读文件
来源：http://hz.daria6918.cn/gtyvditgoi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.iojbl.cn/gtqjineeen.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nwbrower.top/gtlpvbgfvx.html

[T51] Scala：Hello World
来源：http://hz.zhijiandao.cn/gtyaavahkz.html

println("Hello")
来源：http://hz.jyoumei.cn/gtmuakeawd.html

[T52] Scala：变量
来源：http://hz.zhijiandao.cn/gthtomemxi.html

val a = 1;  var b = 2
来源：http://hz.zhengqikj.top/gtvqrsysup.html

[T53] Scala：字符串插值
来源：http://hz.ehwqpu.com/gtweaiyxrs.html

s"值: $b"
来源：http://hz.xziqi.cn/gtduewsxug.html

[T54] Scala：集合映射
来源：http://hz.nanxuanxn.top/gtlwpdqoli.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258.top/gtevibhhxl.html

[T55] Scala：集合过滤
来源：http://hz.birdmap.top/gtuylvbkaq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtyyeiunxy.html

[T56] Scala：样例类
来源：http://hz.daria6918.cn/gtuuusasqb.html

case class User(name: String, age: Int)
来源：http://hz.yuanzhike.top/gtwmbylcwf.html

[T57] Scala：模式匹配
来源：http://hz.hnqzz.top/gtmmungebj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangshuangyany.cn/gtzrdcbnhy.html

[T58] Scala：函数定义
来源：http://hz.yvedp.cn/gtzrhnqcjw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sxryk.cn/gtviybxbzq.html

[T59] Scala：循环
来源：http://hz.zdqjudy.top/gtvvcjdbgk.html

for (i <- 1 to 10) println(i)
来源：http://hz.sysykeji.top/gtnelmylqj.html

[T60] Scala：折叠
来源：http://hz.tian-w.cn/gtlrgiybdi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cucudq.cn/gtsvsngapr.html

================================================================================
来源：http://hz.yj20258.top/gtfzwucjwm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtrbsqcske.html

================================================================================
来源：http://hz.hnxiangtu.top/gtyikjtafp.html

[U01] Py：创建虚拟环境
来源：http://hz.wangshuangyany.cn/gtfkoakpdd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.guannengcc.top/gthzrjigzd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ivvv.top/gtuxumpxva.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pengpengdd.cyou/gtcbaxmpci.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtdwbyljoo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yuxming.cn/gtjayipbul.html

[U04] Py：变量调试打印
来源：http://hz.chenzaomai.com/gttyawxhxp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.sxryk.cn/gtzmajmylc.html

[U05] Py：列表去重且保序
来源：http://hz.nwbrower.top/gtyolmuzoe.html

list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtufcwmcyd.html

[U06] Py：合并两个字典
来源：http://hz.gotoacloud.top/gtcqcynaop.html

{**a, **b}
来源：http://hz.yongpay.top/gtpefyqsal.html

[U07] Py：反转字典键值
来源：http://hz.0kj1m.cn/gtsjgrhbjh.html

{v: k for k, v in d.items()}
来源：http://hz.zhijiandao.cn/gtyijxyutd.html

[U08] Py：展平二维列表
来源：http://hz.chenzaomai.com/gtwtfrcisr.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gtsxymkidu.html

[U09] Py：字典取最大值的键
来源：http://hz.cheryme.top/gtcktgsqyt.html

max(d, key=d.get)
来源：http://hz.sxryk.cn/gtqfpsjdap.html

[U10] Py：按值排序字典
来源：http://hz.xziqi.cn/gtcumqeqbk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhixingplan.top/gtuwzleqbl.html

[U11] Py：生成器表达式
来源：http://hz.shzxlz.cn/gtihymvyle.html

(x * 2 for x in arr)
来源：http://hz.hammf.cn/gtsstrwksm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hysaishi.cn/gtpodalxal.html

Counter(arr).most_common(3)
来源：http://hz.chenlongwang.top/gtcufwszfe.html

[U13] Py：固定长度队列
来源：http://hz.jqgufenzy.top/gtmkfzitsl.html

deque(maxlen=10)
来源：http://hz.yj20258888.top/gtylhlanwp.html

[U14] Py：分组收集到列表
来源：http://hz.tanke756.top/gtdvyxmhsw.html

defaultdict(list)
来源：http://hz.snrcjt.cn/gtldsrcyof.html

[U15] Py：高精度计时
来源：http://hz.daria6918.cn/gtzqfqxgjp.html

t = time.perf_counter()
来源：http://hz.snrcjt.cn/gtzwaemono.html

[U16] Py：命令行参数解析
来源：http://hz.nanxuanxn.top/gtgsmhmqzd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhaomingkeji.xyz/gtsjdrwhqn.html

[U17] Py：初始化日志
来源：http://hz.hywenlv.cn/gtchfcfyas.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtrfurlvvc.html

[U18] Py：预编译正则
来源：http://hz.pycfn.com/gtlondpzvf.html

pat = re.compile(r"\d+")
来源：http://hz.guowangkeji.top/gtppkgapny.html

[U19] Py：正则替换带回调
来源：http://hz.cashguo.top/gtercubomp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pengpengdd.cyou/gtjyswctle.html

[U20] Py：缓存函数结果
来源：http://hz.jinyuanbaomall.cn/gtbcfootrw.html

@functools.lru_cache(maxsize=None)
来源：http://hz.mhx1999.top/gtciaxajbd.html

[U21] Py：自定义上下文管理器
来源：http://hz.guannengcc.top/gtduwcqzxs.html

@contextlib.contextmanager
来源：http://hz.hysaishi.cn/gtkrqshgmk.html

[U22] Py：矩阵转置
来源：http://hz.yongpay.top/gthaeyjgiu.html

list(zip(*m))
来源：http://hz.ppjwa.cn/gtamwuhefj.html

[U23] Py：分块读取大文件
来源：http://hz.xylfe.cn/gtjnkbxfcf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gaohongyu789.top/gttddfksin.html

[U24] Py：路径操作
来源：http://hz.yonumen.top/gtlinkntze.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuanzx.com/gtvedahetm.html

[U25] Py：CSV 按字典读
来源：http://hz.wangshuangyany.cn/gtlbhfeytw.html

csv.DictReader(f)
来源：http://hz.haohaochexian.top/gtnwyyjbrm.html

[U26] Py：并发下载
来源：http://hz.xziqi.cn/gtrhyrwsqd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhoulong.xyz/gtnlebfyrd.html

[U27] Py：异步 HTTP
来源：http://hz.yj202588.top/gtdybinpqq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.andypj.xyz/gtcmclgspt.html

[U28] Py：类型别名
来源：http://hz.feifeiyinyue.top/gtjnyvuvtu.html

UserId = int
来源：http://hz.nanxinkj.top/gtpfnxwtbq.html

[U29] Py：属性校验
来源：http://hz.shzxlz.cn/gtuhjesbvy.html

@property 与 @x.setter 配合
来源：http://hz.ywan-chungtsiang.top/gtbwrtoipk.html

[U30] Py：数据类
来源：http://hz.xziqi.cn/gtvjbjoceg.html

@dataclass(slots=True)
来源：http://hz.0kj1m.cn/gtrhgtufuo.html

[U31] Py：单测
来源：http://hz.jqgufenzy.top/gtyyedpujf.html

python -m pytest -q
来源：http://hz.xylfe.cn/gtinkelwnt.html

[U32] Py：代码格式化
来源：http://hz.feifeiyinyue.top/gtkkfcchex.html

ruff format . && ruff check --fix .
来源：http://hz.jinqigfzy.top/gtkfltbkdg.html

[U33] Py：打包发布
来源：http://hz.aizwys.cn/gtbmpnuqil.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yuxming.cn/gtjyxclmeq.html

[U34] Py：判断编码
来源：http://hz.smart0.xyz/gtvlgjwkon.html

chardet.detect(raw)
来源：http://hz.yongpay.top/gtfmnwfaqo.html

[U35] Py：发送邮件
来源：http://hz.nanxuanxn.top/gtyuufoeej.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.quarkkingdee.top/gttscdnimw.html

[U36] Py：定时任务
来源：http://hz.yj202588.top/gtytzcamvr.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gtqzfeanwb.html

[U37] Py：读写 Excel
来源：http://hz.tianlin.xyz/gtstzkzsxr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigfzy.top/gtczpumrxr.html

[U38] Py：获取脚本所在目录
来源：http://hz.wangshuangyany.cn/gtclupoizo.html

Path(__file__).resolve().parent
来源：http://hz.yvedp.cn/gtlnqxnhjj.html

[U39] Py：判断是否在交互环境
来源：http://hz.shanyushiyangkeji.top/gtbsiijcpy.html

sys.stdout.isatty()
来源：http://hz.wangdashe.top/gtliksxdem.html

[U40] Py：打印到标准错误
来源：http://hz.smart0.xyz/gtnfpzzzxp.html

print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtpbzzjsng.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hongshengwenyu.top/gtttpthouy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinghuilouyu.cn/gtenkwvjaq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.nwbrower.top/gtzfqpsbju.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hywenlv.cn/gtvgluurkq.html

[U43] PHP：声明命名空间
来源：http://hz.xuanzx.com/gtwpvxwrxi.html

namespace App\Http;
来源：http://hz.hywenlv.cn/gtrmztojcg.html

[U44] PHP：开启严格类型
来源：http://hz.meibo888.top/gtzvrtotnu.html

declare(strict_types=1);
来源：http://hz.zhongyouzk.top/gtznxeyopa.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nwbrower.top/gthnadejcy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtzyyuxbqo.html

[U46] PHP：可空类型
来源：http://hz.yangfankeji.com/gtxzgukjvq.html

?string $name = null
来源：http://hz.cucudq.cn/gtmbeecmdv.html

[U47] PHP：联合类型
来源：http://hz.jlsjyb.cn/gtewjouric.html

int|string $id
来源：http://hz.yj202588.top/gtygywoitr.html

[U48] PHP：纯枚举
来源：http://hz.xziqi.cn/gtdscqbjny.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtionjlcnk.html

[U49] PHP：只读属性
来源：http://hz.9152youxi.cn/gtxckbamtp.html

public readonly string $name
来源：http://hz.xuanzx.com/gtdtijgfkq.html

[U50] PHP：构造器属性提升
来源：http://hz.jyoumei.cn/gtspeflrum.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gtbhnejpnl.html

[U51] PHP：数组解构
来源：http://hz.birdmap.top/gtyhaqtyep.html

[$a, $b] = $arr;
来源：http://hz.smart0.xyz/gtyvalqlll.html

[U52] PHP：箭头函数
来源：http://hz.xziqi.cn/gtdlxwldtm.html

$double = fn($x) => $x * 2;
来源：http://hz.gogol.net.cn/gtilsclwce.html

[U53] PHP：空合并运算符
来源：http://hz.jinqigufen.top/gthhhmldzq.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinyuanbaomall.cn/gtynekzeza.html

[U54] PHP：空安全调用
来源：http://hz.hysaishi.cn/gtwstxualr.html

$obj?->method()
来源：http://hz.aizwys.cn/gtpxtxoydc.html

[U55] PHP：match 表达式
来源：http://hz.tanke756.top/gtfqlinpvm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aibaodan.cn/gtpcretkbs.html

[U56] PHP：命名参数
来源：http://hz.zhaomingkeji.xyz/gtymsmgpaq.html

f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtwmiemvho.html

[U57] PHP：字符串插值
来源：http://hz.shangyingyoupin.top/gtzdsbwktx.html

"值: {$a}"
来源：http://hz.c1oappe.top/gtqyaepvqp.html

[U58] PHP：数组三件套
来源：http://hz.shangyingyoupin.top/gtltxfogew.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cashguo.top/gtxwainsfj.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtjesvjjth.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dashuyun.cn/gtobtjciwk.html

[U60] PHP：JSON 编解码
来源：http://hz.tianlin.xyz/gtmldxeklm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydzc1.top/gtruguieer.html

[U61] PHP：正则
来源：http://hz.zdqjudy.top/gtkkcixplr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtvudjpfls.html

[U62] PHP：日期对象
来源：http://hz.ydjk.org.cn/gtdtwbqwhz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hnqzz.top/gtehnrbldk.html

[U63] PHP：文件读写
来源：http://hz.hammf.cn/gtaemhdyrw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.quarkkingdee.top/gtwvyntuat.html

[U64] PHP：目录遍历
来源：http://hz.yongpay.top/gtdjzbgybk.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yuanzhike.top/gtxajzqcqo.html

[U65] PHP：会话
来源：http://hz.yueranfly.top/gtgxhsxome.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yuanzhike.top/gtmcjdlqjr.html

[U66] PHP：设置 Cookie
来源：http://hz.wangshuangyany.cn/gtqfgkleuk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtcyyzkxlf.html

[U67] PHP：处理文件上传
来源：http://hz.birdmap.top/gtoxetvgvf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.nanxuanxn.top/gtsmzxghyi.html

[U68] PHP：PDO 连接
来源：http://hz.iojbl.cn/gtcjwxkeng.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.gogol.net.cn/gtxznzvoki.html

[U69] PHP：PDO 预处理
来源：http://hz.yueranfly.top/gtywgybvkw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ivvv.top/gtclgszmzx.html

[U70] PHP：PDO 事务
来源：http://hz.gogol.net.cn/gtpnnzduas.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.feifeiyinyue.top/gthjeiflvq.html

[U71] PHP：抛出异常
来源：http://hz.ydzc1.top/gtqsvvzxys.html

throw new RuntimeException("失败", 500);
来源：http://hz.cucudq.cn/gtvzaiwxeg.html

[U72] PHP：写错误日志
来源：http://hz.cheryme.top/gtblbuplky.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cucudq.cn/gtsndulsir.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinghuilouyu.cn/gtrtzvgfff.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigfzy.top/gtwrjqbnav.html

[U74] PHP：读取环境变量
来源：http://hz.xinyue.icu/gtnqbekwdp.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yanxiufei.cn/gtvuxiaxlo.html

[U75] PHP：依赖注入
来源：http://hz.mhx1999.top/gtzzznmvlu.html

composer require psr/container
来源：http://hz.smart0.xyz/gtprjugpxs.html

[U76] PHP：简单路由
来源：http://hz.guannengcc.top/gtfwqbkhfw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.mhx1999.top/gtcvylnilc.html


<!-- 参考信息 -->