代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtlqdzsodj.html

[S51] C++：显式类型转换
来源：http://hz.yangfankeji.com/gtrsmyqzze.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gtrixjhhzq.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtqzslghvh.html

int size() const noexcept { return n_; }
来源：http://hz.zhongyouzk.top/gtqfboyvcu.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtcdylbeks.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtpkmsrrbp.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtkwkfddie.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.havefunace.top/gtlwtzmkzh.html

[S55] C++：结构化绑定
来源：http://hz.aibaodan.cn/gtoixkerkq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuanzhike.top/gtdeqekulx.html

[S56] C++：optional
来源：http://hz.chenzaomai.com/gtmmojuabi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.mhx1999.top/gtwmluhcpk.html

[S57] C++：编译期常量
来源：http://hz.yonumen.top/gtwshpzvvv.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtsoajauum.html

[S58] C++：命名空间
来源：http://hz.zhiwuduotai.top/gtojcqxdkk.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtbuzqhyds.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtkmbtwukw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ppjwa.cn/gtcfjmisec.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtxsyjkswi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shuidangran.top/gtedxkwnlq.html

================================================================================
来源：http://hz.hysaishi.cn/gtxjouezjp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxinkj.top/gtcgdxilbv.html

================================================================================
来源：http://hz.meibo888.top/gtoozpjxjd.html

[T01] Kotlin：Hello World
来源：http://hz.hnxiangtu.top/gtmdgdwakx.html

println("Hello")
来源：http://hz.9152youxi.cn/gtjcuatuyp.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtqbkozxjo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jyoumei.cn/gtpycsxbda.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gtaqvfxosj.html

"值: $b"
来源：http://hz.316326.xyz/gtwhxpstmf.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtkexmqyti.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtggtqcopn.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gtlufvvexl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhongyouzk.top/gtmljtorla.html

[T06] Kotlin：集合映射
来源：http://hz.yueranfly.top/gthoiudggh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.c1oappe.top/gttvnbhmgv.html

[T07] Kotlin：集合过滤
来源：http://hz.jinyuanbaomall.cn/gtlybcvgkt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shanyushiyangkeji.top/gtmvxowwyy.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtenvfjwnl.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtvbiiaqwy.html

[T09] Kotlin：扩展函数
来源：http://hz.yanxiufei.cn/gtuhvtucxr.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtxfkwvfli.html

[T10] Kotlin：默认参数
来源：http://hz.guowangkeji.top/gtwwqsmmai.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinghuilouyu.cn/gtamoijzcs.html

[T11] Kotlin：协程
来源：http://hz.jyoumei.cn/gtplyopwpb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sysykeji.top/gtvmkqdybu.html

[T12] Kotlin：解构声明
来源：http://hz.yuanzhike.top/gtrjpovuur.html

val (a, b) = Pair(1, 2)
来源：http://hz.yongpay.top/gtvzmkrflw.html

[T13] Kotlin：只读 Map
来源：http://hz.cucudq.cn/gtlykuzctf.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigfzy.top/gtlugqhmdt.html

[T14] Kotlin：循环
来源：http://hz.xziqi.cn/gtwfhyvkci.html

for (i in 1..10) println(i)
来源：http://hz.birdmap.top/gtpyhouxiq.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtbhlbihoq.html

interface Shape { fun area(): Double }
来源：http://hz.yangfankeji.com/gtqyengbdq.html

[T16] Swift：Hello World
来源：http://hz.aizwys.cn/gtckozwviy.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtgnfakgpj.html

[T17] Swift：变量与常量
来源：http://hz.haohaochexian.top/gtulyizvcc.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtarvcqyxx.html

[T18] Swift：字符串插值
来源：http://hz.yongpay.top/gtlpmggesd.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gtuhrdejwg.html

[T19] Swift：可选绑定
来源：http://hz.shangyingyoupin.top/gtzqupfits.html

if let n = opt { print(n) }
来源：http://hz.jlsjyb.cn/gtldgdrdit.html

[T20] Swift：数组操作
来源：http://hz.ybcxt.top/gtnofrwbxm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtvqnhzdde.html

[T21] Swift：遍历
来源：http://hz.yj20258888.top/gtvhrotfme.html

for x in a { print(x) }
来源：http://hz.jqgfzy.top/gtqpzwgjsj.html

[T22] Swift：字典
来源：http://hz.dianchejie.cn/gtuyoatiqb.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenjidiqi.icu/gtthgijkoh.html

[T23] Swift：函数
来源：http://hz.birdmap.top/gtccvpsjrw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtgoumwsjj.html

[T24] Swift：闭包
来源：http://hz.cheryme.top/gtnjmeqagn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sweek.top/gtzxhiwphl.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtozbngbyt.html

struct P { var x: Int }
来源：http://hz.birdmap.top/gtxvsonlvo.html

[T26] Swift：类与重写
来源：http://hz.zhengqikj.top/gtmetxdcbe.html

class A: Base { override func f() {} }
来源：http://hz.jyoumei.cn/gtndziqses.html

[T27] Swift：错误处理
来源：http://hz.jqgufenzy.top/gtoofahoei.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gtogbjlgpk.html

[T28] Swift：枚举
来源：http://hz.haohaochexian.top/gtuezlhzgt.html

enum Color { case red, green }
来源：http://hz.sysykeji.top/gtsienmzzy.html

[T29] Swift：guard 提前返回
来源：http://hz.ywan-chungtsiang.top/gtnsaxhgxi.html

guard let x = opt else { return }
来源：http://hz.ivvv.top/gtuyckvllp.html

[T30] Swift：协议
来源：http://hz.zhengqikj.top/gtgunbruea.html

protocol Shape { func area() -> Double }
来源：http://hz.birdmap.top/gtptaesjca.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtkoeowlho.html

print("Hello")
来源：http://hz.yonumen.top/gtnoesrptl.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gtabrwtrsu.html

local a = 1
来源：http://hz.shanyushiyangtech.top/gtjulswaav.html

[T33] Lua：表（数组）
来源：http://hz.fengsongda.top/gtrrrpdzcj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgfzy.top/gtosdgviml.html

[T34] Lua：遍历表
来源：http://hz.wangshuangyany.cn/gtxcxkazmo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aibaodan.cn/gtjtkocmjt.html

[T35] Lua：字典表
来源：http://hz.shanyushiyangtech.top/gtvuviwhwd.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ydzc1.top/gtztrqoeiq.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtcelkchft.html

function add(a, b) return a + b end
来源：http://hz.iojbl.cn/gtzkoyytge.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gtvqwvqfky.html

"a" .. "b"
来源：http://hz.c1oappe.top/gtpdlsduuf.html

[T38] Lua：条件
来源：http://hz.ydjk.org.cn/gtbngwnuul.html

if x > 0 then print("正") end
来源：http://hz.9152youxi.cn/gtagxfqqss.html

[T39] Lua：模式匹配
来源：http://hz.daxiang520.top/gtdxldzzmn.html

string.find(s, "%d+")
来源：http://hz.guannengcc.top/gtwjqtpalx.html

[T40] Lua：元表
来源：http://hz.haohaochexian.top/gtkktujwup.html

setmetatable({}, { __index = base })
来源：http://hz.dianchejie.cn/gtmaqijdve.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtiqjfohuo.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtdifgamqy.html

[T42] Perl：变量类型
来源：http://hz.hnxiangtu.top/gtcddbonys.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cheryme.top/gtlhocyfof.html

[T43] Perl：字符串插值
来源：http://hz.meibo888.top/gtzncwthkf.html

"值: $a"
来源：http://hz.tanke756.top/gtkscmscqq.html

[T44] Perl：条件
来源：http://hz.chenjidiqi.icu/gtmkoioqps.html

if ($a > 0) { print "正"; }
来源：http://hz.ehwqpu.com/gtjpvjwgvo.html

[T45] Perl：数组遍历
来源：http://hz.yvedp.cn/gtplazpryd.html

for my $x (@arr) { print $x; }
来源：http://hz.quarkkingdee.top/gtswdjslsx.html

[T46] Perl：哈希操作
来源：http://hz.kuanghao11.cn/gtcbbwgogq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnxiangtu.top/gtjdwshxez.html

[T47] Perl：正则捕获
来源：http://hz.shanyushiyangtech.top/gtxjhoqlmc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gtyyxbexjj.html

[T48] Perl：正则替换
来源：http://hz.sufxvd.cn/gtzxucqlbu.html

$s =~ s/old/new/g;
来源：http://hz.snrcjt.cn/gtgdqxgzqv.html

[T49] Perl：函数
来源：http://hz.nwbrower.top/gtvlpjdpou.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.9152youxi.cn/gtjlaavofs.html

[T50] Perl：逐行读文件
来源：http://hz.shzxlz.cn/gtbpbkbugp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtydcmsjjd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenlongwang.top/gttgskzgqp.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gtxmhhdojs.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtnyokwlla.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtxluunutu.html

val a = 1;  var b = 2
来源：http://hz.ydjk.org.cn/gtcgwmgyyx.html

[T53] Scala：字符串插值
来源：http://hz.smart0.xyz/gtzddgqjvj.html

s"值: $b"
来源：http://hz.redwolf501.top/gtpirccndl.html

[T54] Scala：集合映射
来源：http://hz.ybcxt.top/gtrklvteay.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.vqdsnc.cn/gthggivxrc.html

[T55] Scala：集合过滤
来源：http://hz.jqgufenzy.top/gtgmxallby.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hysaishi.cn/gtofzujfoo.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangtech.top/gtaunmugrx.html

case class User(name: String, age: Int)
来源：http://hz.zdqjudy.top/gtoozfduss.html

[T57] Scala：模式匹配
来源：http://hz.dianchejie.cn/gtvlbcqqzh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtgymjztwr.html

[T58] Scala：函数定义
来源：http://hz.jlsjyb.cn/gtvldeaqao.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhixingplan.top/gtysobsqec.html

[T59] Scala：循环
来源：http://hz.hnxiangtu.top/gtvilesgde.html

for (i <- 1 to 10) println(i)
来源：http://hz.cashguo.top/gtxnkebsgt.html

[T60] Scala：折叠
来源：http://hz.jqgfzy.top/gtpxfktzxp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daria6918.cn/gteohmpaie.html

================================================================================
来源：http://hz.zhixingplan.top/gtgnotmicz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtpbgfwxiv.html

================================================================================
来源：http://hz.hysaishi.cn/gtmollqlik.html

[U01] Py：创建虚拟环境
来源：http://hz.jqgufenzy.top/gtvcjiodeb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xingfuxueyuan.xyz/gtuyiktiwt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nanxinkj.top/gtutvtskei.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shanyushiyangkeji.top/gtbtprnpea.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtqzwkyidy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuetiantiany.cn/gtgybkbbpb.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangkeji.top/gtomysuejh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258888.top/gtsnmxlqyp.html

[U05] Py：列表去重且保序
来源：http://hz.gogol.net.cn/gtzhmozsjl.html

list(dict.fromkeys(arr))
来源：http://hz.aibaodan.cn/gtidiescqn.html

[U06] Py：合并两个字典
来源：http://hz.quarkkingdee.top/gtyxzchtxk.html

{**a, **b}
来源：http://hz.ydjk.org.cn/gtahptlngp.html

[U07] Py：反转字典键值
来源：http://hz.fengsongda.top/gtmqemmggm.html

{v: k for k, v in d.items()}
来源：http://hz.ehwqpu.com/gtzhxgjzvy.html

[U08] Py：展平二维列表
来源：http://hz.hnxiangtu.top/gtuntuhvmt.html

[y for x in nested for y in x]
来源：http://hz.9152youxi.cn/gthhhrkjmo.html

[U09] Py：字典取最大值的键
来源：http://hz.mhx1999.top/gtwxvuvmes.html

max(d, key=d.get)
来源：http://hz.feifeiyinyue.top/gtbkfgihhg.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtyxbegiho.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhongyouzk.top/gttydnwcft.html

[U11] Py：生成器表达式
来源：http://hz.yangfankeji.com/gtngwzmjwj.html

(x * 2 for x in arr)
来源：http://hz.dashuyun.cn/gtjppghxid.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ydjk.org.cn/gtzkqynoif.html

Counter(arr).most_common(3)
来源：http://hz.zycfv.cn/gtuepnydmd.html

[U13] Py：固定长度队列
来源：http://hz.yj20258888.top/gtmqiswuzk.html

deque(maxlen=10)
来源：http://hz.gzhubu.top/gtdwciyxsp.html

[U14] Py：分组收集到列表
来源：http://hz.zdqjudy.top/gtfcecasuh.html

defaultdict(list)
来源：http://hz.cdnleiting.top/gtszzdensi.html

[U15] Py：高精度计时
来源：http://hz.ydjk.org.cn/gtusrjvbwo.html

t = time.perf_counter()
来源：http://hz.gotoacloud.top/gtztmildjg.html

[U16] Py：命令行参数解析
来源：http://hz.guannengcc.top/gtmsjmtjbl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.meibo888.top/gtlrzckxdq.html

[U17] Py：初始化日志
来源：http://hz.guowangkeji.top/gtrhrnabsh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.c1oappe.top/gtnlorbjln.html

[U18] Py：预编译正则
来源：http://hz.hywenlv.cn/gttzarpkvl.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gtnqurvlxc.html

[U19] Py：正则替换带回调
来源：http://hz.iojbl.cn/gtlagekkot.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnxiangtu.top/gtzogbxnzp.html

[U20] Py：缓存函数结果
来源：http://hz.shanyushiyangkeji.top/gtrewtlwyi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yongpay.top/gtgehahpoq.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtkvgnsnbp.html

@contextlib.contextmanager
来源：http://hz.ywan-chungtsiang.top/gtbwpqlmkb.html

[U22] Py：矩阵转置
来源：http://hz.sweek.top/gtptykrphh.html

list(zip(*m))
来源：http://hz.xinyue.icu/gtazdrnmse.html

[U23] Py：分块读取大文件
来源：http://hz.ybcxt.top/gtcdngduxx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jiagoushi.top/gtoukkvpzh.html

[U24] Py：路径操作
来源：http://hz.yanxiufei.cn/gtzuaamydr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhoulong.xyz/gtlzwfctsj.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtsbxjwfom.html

csv.DictReader(f)
来源：http://hz.ppjwa.cn/gtkixanesv.html

[U26] Py：并发下载
来源：http://hz.yuanzhike.top/gtcsisxutx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.guowangkeji.top/gtyhlaaxdm.html

[U27] Py：异步 HTTP
来源：http://hz.jinqigfzy.top/gtwouxrkit.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinyuanbaomall.cn/gtxnouipuc.html

[U28] Py：类型别名
来源：http://hz.birdmap.top/gtmfmxviug.html

UserId = int
来源：http://hz.yuanzhike.top/gtujqfgjzw.html

[U29] Py：属性校验
来源：http://hz.andypj.xyz/gtkosorhjz.html

@property 与 @x.setter 配合
来源：http://hz.mhx1999.top/gtjwpzkzqp.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gtjsydenba.html

@dataclass(slots=True)
来源：http://hz.ppjwa.cn/gtpygaimgz.html

[U31] Py：单测
来源：http://hz.fzhhl.top/gtzafoldux.html

python -m pytest -q
来源：http://hz.nwbrower.top/gtwxhjekjw.html

[U32] Py：代码格式化
来源：http://hz.cucudq.cn/gtluwdlcab.html

ruff format . && ruff check --fix .
来源：http://hz.zdqjudy.top/gtfzmjhhoy.html

[U33] Py：打包发布
来源：http://hz.yuxming.cn/gtwikgvpec.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yj202588.top/gtaknqourn.html

[U34] Py：判断编码
来源：http://hz.yj20258.top/gtetlmhcak.html

chardet.detect(raw)
来源：http://hz.jqgfzy.top/gthzgzhnts.html

[U35] Py：发送邮件
来源：http://hz.haohaochexian.top/gtzklrtkei.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhixingplan.top/gtifukstys.html

[U36] Py：定时任务
来源：http://hz.jqgufenzy.top/gthtrxmisu.html

schedule.every(10).minutes.do(job)
来源：http://hz.ivvv.top/gtyjmcbeqq.html

[U37] Py：读写 Excel
来源：http://hz.nanxinkj.top/gtzsezexxz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhoulong.xyz/gtxhfcvhmy.html

[U38] Py：获取脚本所在目录
来源：http://hz.daxiang520.top/gtynjchmzk.html

Path(__file__).resolve().parent
来源：http://hz.fzhhl.top/gtaqiemmcn.html

[U39] Py：判断是否在交互环境
来源：http://hz.gotoacloud.top/gtstwibzdl.html

sys.stdout.isatty()
来源：http://hz.yanxiufei.cn/gthbacqhea.html

[U40] Py：打印到标准错误
来源：http://hz.andypj.xyz/gtqinlgedz.html

print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtiwpjcybo.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yuxming.cn/gtcwtatdqx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cqqwz.cn/gtslrwlpcz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhijiandao.cn/gtxqziwpci.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinqigfzy.top/gtjyqinlkm.html

[U43] PHP：声明命名空间
来源：http://hz.sweek.top/gtnccnjnwa.html

namespace App\Http;
来源：http://hz.guannengcc.top/gtetbauaug.html

[U44] PHP：开启严格类型
来源：http://hz.sysykeji.top/gtgcldpece.html

declare(strict_types=1);
来源：http://hz.9152youxi.cn/gtkasllbrz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jyoumei.cn/gtxlhczdgk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtyndkzglh.html

[U46] PHP：可空类型
来源：http://hz.xuanzx.com/gtybkdwzqp.html

?string $name = null
来源：http://hz.shangyingyoupin.top/gtqlenazlu.html

[U47] PHP：联合类型
来源：http://hz.daria6918.cn/gtegcdxkth.html

int|string $id
来源：http://hz.shanyushiyangtech.top/gtrugygjbh.html

[U48] PHP：纯枚举
来源：http://hz.havefunace.top/gtjytexawz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.kuanghao11.cn/gtkgtbyhow.html

[U49] PHP：只读属性
来源：http://hz.meibo888.top/gtjrbkqdhw.html

public readonly string $name
来源：http://hz.ydjk.org.cn/gtbozxokgk.html

[U50] PHP：构造器属性提升
来源：http://hz.pengpengdd.cyou/gtikjedyir.html

public function __construct(private int $id) {}
来源：http://hz.xuetiantiany.cn/gtrlbzbmxx.html

[U51] PHP：数组解构
来源：http://hz.gogol.net.cn/gtbnxnjcrd.html

[$a, $b] = $arr;
来源：http://hz.hongshengwenyu.top/gtpqqcmgsq.html

[U52] PHP：箭头函数
来源：http://hz.redwolf501.top/gtsncsntsg.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtzghmdnzi.html

[U53] PHP：空合并运算符
来源：http://hz.yj202588.top/gtkpelcvth.html

$v = $a ?? $b ?? "default";
来源：http://hz.xinyue.icu/gtrhzznubi.html

[U54] PHP：空安全调用
来源：http://hz.aizwys.cn/gtrrjkisuk.html

$obj?->method()
来源：http://hz.sweek.top/gtnabblcmm.html

[U55] PHP：match 表达式
来源：http://hz.yangfankeji.com/gtgdrzonpu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gotoacloud.top/gtzxgnpmio.html

[U56] PHP：命名参数
来源：http://hz.hysaishi.cn/gtuaoemcgt.html

f(a: 1, b: 2)
来源：http://hz.zhijiandao.cn/gtdefrpyrf.html

[U57] PHP：字符串插值
来源：http://hz.52xcode.cn/gtddppwplw.html

"值: {$a}"
来源：http://hz.jinqigfzy.top/gtwdgylkwr.html

[U58] PHP：数组三件套
来源：http://hz.hywenlv.cn/gtdlxdchco.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.bjfxy.top/gtkzycxgbh.html

[U59] PHP：自定义排序
来源：http://hz.nwbrower.top/gtafvmbjyy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hysaishi.cn/gtarftehfl.html

[U60] PHP：JSON 编解码
来源：http://hz.aizwys.cn/gtugbbvggk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cucudq.cn/gtxdiicwpv.html

[U61] PHP：正则
来源：http://hz.hfpthk.cn/gtqwfgprxb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtwuzrwedz.html

[U62] PHP：日期对象
来源：http://hz.xuetiantiany.cn/gtscyqmhgg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.svipenyu.cn/gtgtediwit.html

[U63] PHP：文件读写
来源：http://hz.sysykeji.top/gthsgugcni.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.aizwys.cn/gtfbhwjmxi.html

[U64] PHP：目录遍历
来源：http://hz.jinqigufen.top/gtagzgsbur.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aizwys.cn/gthajtwbyu.html

[U65] PHP：会话
来源：http://hz.chenlongwang.top/gtdxomuacl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dianchejie.cn/gtancpsxdk.html

[U66] PHP：设置 Cookie
来源：http://hz.jinyuanbaomall.cn/gtphmkffty.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gthyrzpjbj.html

[U67] PHP：处理文件上传
来源：http://hz.guowangkeji.top/gtmkpivjtc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.havefunace.top/gtjokogoal.html

[U68] PHP：PDO 连接
来源：http://hz.andypj.xyz/gtmxmdfigw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.andypj.xyz/gtqjzjwafo.html

[U69] PHP：PDO 预处理
来源：http://hz.havefunace.top/gtigwfoyfv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yonumen.top/gtcrsgglcu.html

[U70] PHP：PDO 事务
来源：http://hz.sufxvd.cn/gtdyvaroox.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj20258.top/gtwvhsifpr.html

[U71] PHP：抛出异常
来源：http://hz.vqdsnc.cn/gtxufgomqy.html

throw new RuntimeException("失败", 500);
来源：http://hz.bjfxy.top/gtfdemgkwa.html

[U72] PHP：写错误日志
来源：http://hz.vqdsnc.cn/gtpkwttsho.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ybcxt.top/gtcqzupupy.html

[U73] PHP：读取 ini 配置
来源：http://hz.aibaodan.cn/gtnzfyqixk.html

parse_ini_file("config.ini", true)
来源：http://hz.cdnleiting.top/gtvkzhrowt.html

[U74] PHP：读取环境变量
来源：http://hz.tanke756.top/gtmfdmlfwg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhijiandao.cn/gtxtkahibg.html

[U75] PHP：依赖注入
来源：http://hz.nanxinkj.top/gtmgtrrvaj.html

composer require psr/container
来源：http://hz.hnxiangtu.top/gtacqyfucb.html

[U76] PHP：简单路由
来源：http://hz.hfpthk.cn/gttfopntuj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ywan-chungtsiang.top/gtynmpynup.html


<!-- 参考信息 -->