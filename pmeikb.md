代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.zycfv.cn/gthvppjpah.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtncizlcbj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cdnleiting.top/gtwuqffili.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtuttemage.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dashuyun.cn/gttasamoyh.html

[S51] C++：显式类型转换
来源：http://hz.dashuyun.cn/gtsyfshcnn.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gthplnzzuv.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gtorlhlbnk.html

int size() const noexcept { return n_; }
来源：http://hz.jlsjyb.cn/gtrarnhsrq.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtwvajfaha.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gthfaqplax.html

[S54] C++：异常处理
来源：http://hz.feifeiyinyue.top/gtxanpnqxa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenzaomai.com/gtsazdqsep.html

[S55] C++：结构化绑定
来源：http://hz.zhijiandao.cn/gtofwiobur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtwjwsdwsx.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtmfpjzkdi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cheryme.top/gtnbuyflvl.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtphnugzbg.html

constexpr int N = 10;
来源：http://hz.jqgfzy.top/gtnmvsyups.html

[S58] C++：命名空间
来源：http://hz.ppjwa.cn/gtbdlgfpoz.html

namespace ns { int f() { return 1; } }
来源：http://hz.ybcxt.top/gtbeseekfd.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtjdowrrbv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtnisarcfb.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gtpygmpfsc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.andypj.xyz/gthlpifjvi.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtiysmtkru.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtyxasidff.html

================================================================================
来源：http://hz.gzhubu.top/gtjafojopm.html

[T01] Kotlin：Hello World
来源：http://hz.yonumen.top/gtghpvfefm.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtqlcfpths.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtwivjtvfa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gogol.net.cn/gtnuxauvlx.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gtswzdwjnx.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtgazxuybz.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gtyapsbigv.html

val n: String? = null;  n?.length
来源：http://hz.andypj.xyz/gtsgaorfza.html

[T05] Kotlin：when 表达式
来源：http://hz.snrcjt.cn/gtayhrrmxh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yangfankeji.com/gtqefdfrcq.html

[T06] Kotlin：集合映射
来源：http://hz.shangyingyoupin.top/gtjjnppskw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zycfv.cn/gtymttbgms.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtjmdzhame.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aizwys.cn/gtwcyyzfks.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gtelzdyqdc.html

data class User(val name: String, val age: Int)
来源：http://hz.shzxlz.cn/gtjyrjxvvb.html

[T09] Kotlin：扩展函数
来源：http://hz.mhx1999.top/gtewwmzbkr.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtakvspzzq.html

[T10] Kotlin：默认参数
来源：http://hz.ywan-chungtsiang.top/gtkqooioxa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gtiupndjnv.html

[T11] Kotlin：协程
来源：http://hz.cucudq.cn/gtbnsebabe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cashguo.top/gtyowteslx.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtsjquqdgj.html

val (a, b) = Pair(1, 2)
来源：http://hz.jiagoushi.top/gthxwlkrrm.html

[T13] Kotlin：只读 Map
来源：http://hz.shanyushiyangkeji.top/gtybzjpkmr.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangkeji.top/gtvyfxabcx.html

[T14] Kotlin：循环
来源：http://hz.nanxinkj.top/gtetqbgeui.html

for (i in 1..10) println(i)
来源：http://hz.jyoumei.cn/gtsytpmedx.html

[T15] Kotlin：接口
来源：http://hz.iojbl.cn/gtuvzfxnsu.html

interface Shape { fun area(): Double }
来源：http://hz.tianlin.xyz/gtavncefst.html

[T16] Swift：Hello World
来源：http://hz.zhoulong.xyz/gtvocfrvut.html

print("Hello")
来源：http://hz.sysykeji.top/gtlgxxfmrl.html

[T17] Swift：变量与常量
来源：http://hz.nanxuanxn.top/gtyknlumlk.html

var a = 1;  let b = 2
来源：http://hz.zycfv.cn/gtufhlxmim.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtmtngivqa.html

"值: \(b)"
来源：http://hz.kuanghao11.cn/gtpfuungtk.html

[T19] Swift：可选绑定
来源：http://hz.guannengcc.top/gtcfjfjktu.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtikjkwska.html

[T20] Swift：数组操作
来源：http://hz.chenzaomai.com/gtfuerxwpz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hammf.cn/gtgxxvhnqd.html

[T21] Swift：遍历
来源：http://hz.xziqi.cn/gtvsxgnawm.html

for x in a { print(x) }
来源：http://hz.meibo888.top/gtsbhgpefm.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtlovdugzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtgkbqxxgw.html

[T23] Swift：函数
来源：http://hz.guannengcc.top/gtgchkirqp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gtagridldc.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtitulwqoc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuxming.cn/gthsaynmmf.html

[T25] Swift：结构体
来源：http://hz.cucudq.cn/gtwkevmryl.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gtpgosuzvb.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtxjvgnrnx.html

class A: Base { override func f() {} }
来源：http://hz.ywan-chungtsiang.top/gtfsorzavc.html

[T27] Swift：错误处理
来源：http://hz.52xcode.cn/gtgenilwyp.html

do { try f() } catch { print(error) }
来源：http://hz.vqdsnc.cn/gtotclmbuq.html

[T28] Swift：枚举
来源：http://hz.ybcxt.top/gtecsevxjg.html

enum Color { case red, green }
来源：http://hz.ppjwa.cn/gtutbxxscn.html

[T29] Swift：guard 提前返回
来源：http://hz.cheryme.top/gtjtylyjah.html

guard let x = opt else { return }
来源：http://hz.yj20258888.top/gtzjqukdcu.html

[T30] Swift：协议
来源：http://hz.jianghu66.top/gtvvukqksk.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtklottxzr.html

[T31] Lua：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtdgdccztp.html

print("Hello")
来源：http://hz.tanke756.top/gteedcptjk.html

[T32] Lua：局部变量
来源：http://hz.chenlongwang.top/gtwdwrlime.html

local a = 1
来源：http://hz.yuanzhike.top/gtmxwneopx.html

[T33] Lua：表（数组）
来源：http://hz.yongpay.top/gtrqhzpbxh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gtpmkwkhcu.html

[T34] Lua：遍历表
来源：http://hz.cqqwz.cn/gtgwhrmxjf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dianchejie.cn/gtyeyrytde.html

[T35] Lua：字典表
来源：http://hz.nwbrower.top/gtylaesnxm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gttpgdcxyv.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtbiyovkxo.html

function add(a, b) return a + b end
来源：http://hz.jqgufenzy.top/gtitovrroy.html

[T37] Lua：字符串拼接
来源：http://hz.hnqzz.top/gtprcikjvj.html

"a" .. "b"
来源：http://hz.guannengcc.top/gtniemubrb.html

[T38] Lua：条件
来源：http://hz.jinqigfzy.top/gtlylzrweo.html

if x > 0 then print("正") end
来源：http://hz.jinqigfzy.top/gtjnpvnimb.html

[T39] Lua：模式匹配
来源：http://hz.tanke756.top/gtuefljtll.html

string.find(s, "%d+")
来源：http://hz.shanyushiyangkeji.top/gtnqnifgjm.html

[T40] Lua：元表
来源：http://hz.hammf.cn/gtsiowwknu.html

setmetatable({}, { __index = base })
来源：http://hz.andypj.xyz/gtrfkhxjcf.html

[T41] Perl：Hello World
来源：http://hz.yangfankeji.com/gtcyxmgtxe.html

print "Hello\n";
来源：http://hz.tian-w.cn/gtjvhfzmbh.html

[T42] Perl：变量类型
来源：http://hz.yvedp.cn/gtyumhzytx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xylfe.cn/gtksucbrww.html

[T43] Perl：字符串插值
来源：http://hz.ivvv.top/gthlgqrwpr.html

"值: $a"
来源：http://hz.zhijiandao.cn/gtfktwjhiz.html

[T44] Perl：条件
来源：http://hz.ppjwa.cn/gtslpltvzd.html

if ($a > 0) { print "正"; }
来源：http://hz.cucudq.cn/gtgjzinpem.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtecnuengr.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258888.top/gtyeruhszh.html

[T46] Perl：哈希操作
来源：http://hz.iojbl.cn/gtllbbbuwe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenlongwang.top/gtyiifljuh.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gttmkojskt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.0kj1m.cn/gtpilawlpw.html

[T48] Perl：正则替换
来源：http://hz.jiagoushi.top/gtkwgpknbv.html

$s =~ s/old/new/g;
来源：http://hz.aibaodan.cn/gtxsyzoqgj.html

[T49] Perl：函数
来源：http://hz.zhengqikj.top/gtxbjjitjh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nwbrower.top/gtyqqvtsgj.html

[T50] Perl：逐行读文件
来源：http://hz.jqgfzy.top/gtsohqriuq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.guowangkeji.top/gtippbyyqn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yj20258.top/gtdmdbpojg.html

[T51] Scala：Hello World
来源：http://hz.fzhhl.top/gthxelpijp.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtobjgrpnh.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtujfmvfdj.html

val a = 1;  var b = 2
来源：http://hz.snrcjt.cn/gttwlipgdc.html

[T53] Scala：字符串插值
来源：http://hz.jinqigufen.top/gtwfppuszv.html

s"值: $b"
来源：http://hz.zycfv.cn/gtfnqsgmpw.html

[T54] Scala：集合映射
来源：http://hz.yuanzhike.top/gtmqrziudy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtualxitcg.html

[T55] Scala：集合过滤
来源：http://hz.guowangkeji.top/gtysinijsu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtdwzhiiae.html

[T56] Scala：样例类
来源：http://hz.ydjk.org.cn/gtwoyegyqk.html

case class User(name: String, age: Int)
来源：http://hz.sufxvd.cn/gtkztoneic.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtgrbalkmj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hammf.cn/gtmngtmrba.html

[T58] Scala：函数定义
来源：http://hz.guowangkeji.top/gtddmhgvxh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258.top/gtbeufmmse.html

[T59] Scala：循环
来源：http://hz.jqgfzy.top/gtjtqtusvy.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangtech.top/gtfyfffshn.html

[T60] Scala：折叠
来源：http://hz.svipenyu.cn/gtpoggstgq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.dianchejie.cn/gtavagyzsw.html

================================================================================
来源：http://hz.mhx1999.top/gtgdagkxlp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhixingplan.top/gtpcpvhlyy.html

================================================================================
来源：http://hz.ydjk.org.cn/gtgnkcqzza.html

[U01] Py：创建虚拟环境
来源：http://hz.ywan-chungtsiang.top/gtabiwampc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.316326.xyz/gttehbxafo.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jianghu66.top/gtmnqeymaq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shuidangran.top/gthuhbkbib.html

[U03] Py：加载 .env 配置
来源：http://hz.iojbl.cn/gttwsvpere.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.316326.xyz/gtwhzsjeer.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gtvzljqqps.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guannengcc.top/gtwzimlqvi.html

[U05] Py：列表去重且保序
来源：http://hz.guowangkeji.top/gtuwlwaoko.html

list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtqjexlpbi.html

[U06] Py：合并两个字典
来源：http://hz.shzxlz.cn/gtknespurg.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtdwxtrtiy.html

[U07] Py：反转字典键值
来源：http://hz.dianchejie.cn/gtffvmroek.html

{v: k for k, v in d.items()}
来源：http://hz.nanxinkj.top/gtbjylupka.html

[U08] Py：展平二维列表
来源：http://hz.ivvv.top/gtvywjfxfp.html

[y for x in nested for y in x]
来源：http://hz.wangshuangyany.cn/gtdjgcspgb.html

[U09] Py：字典取最大值的键
来源：http://hz.nanxuanxn.top/gtnzjksoyq.html

max(d, key=d.get)
来源：http://hz.hywenlv.cn/gtotsfrhxu.html

[U10] Py：按值排序字典
来源：http://hz.shuidangran.top/gtrfdeijxb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxuanxn.top/gtvpdmshii.html

[U11] Py：生成器表达式
来源：http://hz.quarkkingdee.top/gtbqyzjmtx.html

(x * 2 for x in arr)
来源：http://hz.zhixingplan.top/gtcrrqjgzs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.daxiang520.top/gtcdzrnqww.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtpzjfxkcf.html

[U13] Py：固定长度队列
来源：http://hz.daxiang520.top/gtwbntkchi.html

deque(maxlen=10)
来源：http://hz.kuanghao11.cn/gtlhbmgjpq.html

[U14] Py：分组收集到列表
来源：http://hz.feifeiyinyue.top/gtwxwpmjkw.html

defaultdict(list)
来源：http://hz.ivvv.top/gtszjefqnj.html

[U15] Py：高精度计时
来源：http://hz.zycfv.cn/gtubbgccry.html

t = time.perf_counter()
来源：http://hz.shanyushiyangkeji.top/gteufzzvpp.html

[U16] Py：命令行参数解析
来源：http://hz.zhengqikj.top/gtxtbpposj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sxryk.cn/gttwxfdkzq.html

[U17] Py：初始化日志
来源：http://hz.havefunace.top/gtqmmbsmjj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cqqwz.cn/gteqzkyoar.html

[U18] Py：预编译正则
来源：http://hz.jlsjyb.cn/gtkawhrctd.html

pat = re.compile(r"\d+")
来源：http://hz.bjfxy.top/gtzyzaqqpn.html

[U19] Py：正则替换带回调
来源：http://hz.yanxiufei.cn/gtmsogghrk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gaohongyu789.top/gtzqebfqmq.html

[U20] Py：缓存函数结果
来源：http://hz.ydzc1.top/gtnqrnaemj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.ywan-chungtsiang.top/gtqkodozhf.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinyuanbaomall.cn/gtdveuynrz.html

@contextlib.contextmanager
来源：http://hz.bjfxy.top/gtopihymen.html

[U22] Py：矩阵转置
来源：http://hz.quarkkingdee.top/gtpaknnrty.html

list(zip(*m))
来源：http://hz.hnxiangtu.top/gtarccwbwm.html

[U23] Py：分块读取大文件
来源：http://hz.yongpay.top/gtkjqpxmqa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnxiangtu.top/gtzewvwxir.html

[U24] Py：路径操作
来源：http://hz.quarkkingdee.top/gtmnnruzlp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.52xcode.cn/gtpyhdiygn.html

[U25] Py：CSV 按字典读
来源：http://hz.tianlin.xyz/gtoqpwsbnr.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtfyosmjgn.html

[U26] Py：并发下载
来源：http://hz.hnxiangtu.top/gtgapawqnu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gzhubu.top/gtarkkzhww.html

[U27] Py：异步 HTTP
来源：http://hz.xinyue.icu/gttrsfvdfe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ybcxt.top/gtegovfcbq.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtdpsnoefy.html

UserId = int
来源：http://hz.cucudq.cn/gtpnzwflqg.html

[U29] Py：属性校验
来源：http://hz.tianlin.xyz/gtwttvmjfm.html

@property 与 @x.setter 配合
来源：http://hz.jinqigufen.top/gttikxwiem.html

[U30] Py：数据类
来源：http://hz.yongpay.top/gtayxksako.html

@dataclass(slots=True)
来源：http://hz.guannengcc.top/gtkuyjtpgy.html

[U31] Py：单测
来源：http://hz.xziqi.cn/gtzajauxpt.html

python -m pytest -q
来源：http://hz.yonumen.top/gtqyzebknz.html

[U32] Py：代码格式化
来源：http://hz.yvedp.cn/gtdzaqpxml.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtndyfgkim.html

[U33] Py：打包发布
来源：http://hz.vqdsnc.cn/gtcrnallhf.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.fengsongda.top/gtwyarfnfw.html

[U34] Py：判断编码
来源：http://hz.wangshuangyany.cn/gtzhsxnalj.html

chardet.detect(raw)
来源：http://hz.xuetiantiany.cn/gtbpoesmax.html

[U35] Py：发送邮件
来源：http://hz.andypj.xyz/gtgloxilst.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.fengsongda.top/gtujbdbyqe.html

[U36] Py：定时任务
来源：http://hz.hnxiangtu.top/gtlpbrvjei.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtjfiieeue.html

[U37] Py：读写 Excel
来源：http://hz.yuxming.cn/gtoiaegnxd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ehwqpu.com/gtwjdmpqct.html

[U38] Py：获取脚本所在目录
来源：http://hz.yueranfly.top/gtfdqpahdh.html

Path(__file__).resolve().parent
来源：http://hz.jiagoushi.top/gtttubqmtp.html

[U39] Py：判断是否在交互环境
来源：http://hz.ehwqpu.com/gtyderzmti.html

sys.stdout.isatty()
来源：http://hz.fzhhl.top/gtlofjhpzs.html

[U40] Py：打印到标准错误
来源：http://hz.chenzaomai.com/gtqglntbem.html

print("err", file=sys.stderr)
来源：http://hz.jianghu66.top/gtqktcposn.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yongpay.top/gtrxovlfjq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jinqigfzy.top/gtjwxguqbk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zycfv.cn/gtbxtmkyfv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gotoacloud.top/gtorypkicv.html

[U43] PHP：声明命名空间
来源：http://hz.tianlin.xyz/gtnhlgtjlb.html

namespace App\Http;
来源：http://hz.xuanzx.com/gtslfqhpex.html

[U44] PHP：开启严格类型
来源：http://hz.jiagoushi.top/gtjrtcmwmb.html

declare(strict_types=1);
来源：http://hz.ydjk.org.cn/gtznvsxyzt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxinkj.top/gtolayueaj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtdymmmcen.html

[U46] PHP：可空类型
来源：http://hz.xziqi.cn/gtdaygvvty.html

?string $name = null
来源：http://hz.jlsjyb.cn/gtxyqhkbuj.html

[U47] PHP：联合类型
来源：http://hz.zhijiandao.cn/gtlqjexvtw.html

int|string $id
来源：http://hz.wangdashe.top/gtvectcfmv.html

[U48] PHP：纯枚举
来源：http://hz.hnxiangtu.top/gtmyuckmsz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hysaishi.cn/gtcjmsfarz.html

[U49] PHP：只读属性
来源：http://hz.chenjidiqi.icu/gtutcmmbml.html

public readonly string $name
来源：http://hz.gaohongyu789.top/gtrfrefeqi.html

[U50] PHP：构造器属性提升
来源：http://hz.guannengcc.top/gtbgzwluoo.html

public function __construct(private int $id) {}
来源：http://hz.wangdashe.top/gtedsmergz.html

[U51] PHP：数组解构
来源：http://hz.shzxlz.cn/gtmoqpgzkd.html

[$a, $b] = $arr;
来源：http://hz.sysykeji.top/gttxlkhnwu.html

[U52] PHP：箭头函数
来源：http://hz.nanxinkj.top/gtoenoozne.html

$double = fn($x) => $x * 2;
来源：http://hz.chenzaomai.com/gtmlivxrvu.html

[U53] PHP：空合并运算符
来源：http://hz.xuetiantiany.cn/gtdteiihby.html

$v = $a ?? $b ?? "default";
来源：http://hz.hongshengwenyu.top/gtfniwradc.html

[U54] PHP：空安全调用
来源：http://hz.ybcxt.top/gtbggscfcz.html

$obj?->method()
来源：http://hz.daxiang520.top/gtoouxwsbx.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtytgyinrq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yongpay.top/gtvmhbapxa.html

[U56] PHP：命名参数
来源：http://hz.mhx1999.top/gtagyaqqrl.html

f(a: 1, b: 2)
来源：http://hz.sweek.top/gttzfjydyv.html

[U57] PHP：字符串插值
来源：http://hz.sxryk.cn/gtegdbrloc.html

"值: {$a}"
来源：http://hz.9152youxi.cn/gtbeoagppe.html

[U58] PHP：数组三件套
来源：http://hz.wangshuangyany.cn/gtqkejngbj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtxgfihdfg.html

[U59] PHP：自定义排序
来源：http://hz.zycfv.cn/gtiplhdvlu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dashuyun.cn/gtawnwsdoy.html

[U60] PHP：JSON 编解码
来源：http://hz.jiagoushi.top/gtazavzftq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.chenlongwang.top/gtdaymgxab.html

[U61] PHP：正则
来源：http://hz.daria6918.cn/gtcaxwaqre.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgfzy.top/gtstddxuhq.html

[U62] PHP：日期对象
来源：http://hz.havefunace.top/gtpxmtgena.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.chenzaomai.com/gtdtopched.html

[U63] PHP：文件读写
来源：http://hz.svipenyu.cn/gtjknpvyfw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.birdmap.top/gtoznytdqd.html

[U64] PHP：目录遍历
来源：http://hz.daria6918.cn/gtobgqsfti.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.svipenyu.cn/gtvaiujwzp.html

[U65] PHP：会话
来源：http://hz.zhiwuduotai.top/gttpquksvo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.svipenyu.cn/gtjuewstod.html

[U66] PHP：设置 Cookie
来源：http://hz.daxiang520.top/gtfbqnsugv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cashguo.top/gtygabcnmo.html

[U67] PHP：处理文件上传
来源：http://hz.hongshengwenyu.top/gtxgfvzhdd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.bjfxy.top/gtwstbaysk.html

[U68] PHP：PDO 连接
来源：http://hz.zhijiandao.cn/gttwjckzai.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.guowangkeji.top/gtaxeucemd.html

[U69] PHP：PDO 预处理
来源：http://hz.daria6918.cn/gtxgjjgpye.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.fengsongda.top/gtlzoswtyt.html

[U70] PHP：PDO 事务
来源：http://hz.jinqigufen.top/gtptfnbvrt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.sufxvd.cn/gtbmujsuzm.html

[U71] PHP：抛出异常
来源：http://hz.bjfxy.top/gtzgdqvyox.html

throw new RuntimeException("失败", 500);
来源：http://hz.guannengcc.top/gtklgwftoh.html

[U72] PHP：写错误日志
来源：http://hz.cheryme.top/gtxgkcughe.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zdqjudy.top/gttggkcxpm.html

[U73] PHP：读取 ini 配置
来源：http://hz.c1oappe.top/gtirbpllfe.html

parse_ini_file("config.ini", true)
来源：http://hz.cucudq.cn/gtuvjzvbyr.html

[U74] PHP：读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtwygfkfss.html

getenv("APP_ENV") ?: "production"
来源：http://hz.nwbrower.top/gtiezxisqt.html


<!-- 参考信息 -->