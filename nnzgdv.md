代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.zycfv.cn/gtkfhlsqht.html

[S53] C++：移动语义
来源：http://hz.jinghuilouyu.cn/gtwywecnqs.html

std::vector<int> w = std::move(v);
来源：http://hz.jyoumei.cn/gtlkgvfsrp.html

[S54] C++：异常处理
来源：http://hz.52xcode.cn/gtikwwkhke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenlongwang.top/gtrtcprznc.html

[S55] C++：结构化绑定
来源：http://hz.shzxlz.cn/gtmmdxhriv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daria6918.cn/gtvkvgtxux.html

[S56] C++：optional
来源：http://hz.xingfuxueyuan.xyz/gtltmuyish.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtkfuxrwep.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtvccqnzoo.html

constexpr int N = 10;
来源：http://hz.andypj.xyz/gtddbcoxru.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtvptiayix.html

namespace ns { int f() { return 1; } }
来源：http://hz.zycfv.cn/gtmwgiaryq.html

[S59] C++：静态断言
来源：http://hz.hysaishi.cn/gtsuzyqiot.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jiagoushi.top/gtjyccdwji.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gttwqttjki.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtjbqjhhgz.html

================================================================================
来源：http://hz.dashuyun.cn/gtmedzvjau.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.andypj.xyz/gtjdnjrczv.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuzwcomog.html

[T01] Kotlin：Hello World
来源：http://hz.yvedp.cn/gtdsraznbg.html

println("Hello")
来源：http://hz.ybcxt.top/gtcfacjzgc.html

[T02] Kotlin：变量
来源：http://hz.dashuyun.cn/gtobfalcmh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxinkj.top/gtkznmadup.html

[T03] Kotlin：字符串模板
来源：http://hz.guowangkeji.top/gtzhijrdws.html

"值: $b"
来源：http://hz.sufxvd.cn/gtsjsssgvu.html

[T04] Kotlin：空安全
来源：http://hz.316326.xyz/gtofjfwzim.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtbeflooml.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtyandsnkq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.svipenyu.cn/gtmvyjnpdr.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtktrogebf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ydjk.org.cn/gteeujqeud.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gthguvcaym.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtzsijnxva.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtxvigamtv.html

data class User(val name: String, val age: Int)
来源：http://hz.chenlongwang.top/gtsvcxujfd.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtrvoiafsm.html

fun String.exclaim() = this + "!"
来源：http://hz.jyoumei.cn/gtsqsrbypp.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gtlegpjhdj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.vqdsnc.cn/gtqhlckmdf.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtzqmvjfpg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xziqi.cn/gtezmpcznf.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtthpznezo.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtialqazxg.html

[T13] Kotlin：只读 Map
来源：http://hz.jlsjyb.cn/gtjkuotlmi.html

val m = mapOf("a" to 1)
来源：http://hz.meibo888.top/gtuivfdicq.html

[T14] Kotlin：循环
来源：http://hz.zhengqikj.top/gtlucvykhp.html

for (i in 1..10) println(i)
来源：http://hz.guannengcc.top/gtjpmqnlgs.html

[T15] Kotlin：接口
来源：http://hz.bjfxy.top/gtnqjyjhua.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtnulkgjwy.html

[T16] Swift：Hello World
来源：http://hz.chenzaomai.com/gtfpnizvrs.html

print("Hello")
来源：http://hz.pycfn.com/gtwrkfhqok.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gtpfewwuai.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gtedrtygsu.html

[T18] Swift：字符串插值
来源：http://hz.ydjk.org.cn/gtjkggdrcv.html

"值: \(b)"
来源：http://hz.bjfxy.top/gtiuiukxkh.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtxwlymldo.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtyilekvji.html

[T20] Swift：数组操作
来源：http://hz.iojbl.cn/gtcbhsdcsv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgfzy.top/gtevvfkjcp.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtndrrsejb.html

for x in a { print(x) }
来源：http://hz.wangshuangyany.cn/gtwgqmahya.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtknsxrvjm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtrlzngoaf.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtpaaqytdz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtxssohulo.html

[T24] Swift：闭包
来源：http://hz.redwolf501.top/gtzvmvxuqr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sxryk.cn/gtykmpshds.html

[T25] Swift：结构体
来源：http://hz.fengsongda.top/gtnfqeeilb.html

struct P { var x: Int }
来源：http://hz.havefunace.top/gtujrkkxrv.html

[T26] Swift：类与重写
来源：http://hz.vqdsnc.cn/gtnzbilwdc.html

class A: Base { override func f() {} }
来源：http://hz.xylfe.cn/gtmylbshrk.html

[T27] Swift：错误处理
来源：http://hz.yangfankeji.com/gtvkwrgxts.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gtcgkisqvd.html

[T28] Swift：枚举
来源：http://hz.ppjwa.cn/gtmyfdevfe.html

enum Color { case red, green }
来源：http://hz.yuanzhike.top/gtcavhgmqi.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtkvmdmomn.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gtunfqoqzj.html

[T30] Swift：协议
来源：http://hz.zhixingplan.top/gtqdvfvddr.html

protocol Shape { func area() -> Double }
来源：http://hz.xziqi.cn/gtapvhtsuw.html

[T31] Lua：Hello World
来源：http://hz.0kj1m.cn/gtxtnzgvca.html

print("Hello")
来源：http://hz.sysykeji.top/gtotphssdw.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gtulsemcqd.html

local a = 1
来源：http://hz.ywan-chungtsiang.top/gtsahoqdyv.html

[T33] Lua：表（数组）
来源：http://hz.bjfxy.top/gtvpvrkhor.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinyuanbaomall.cn/gtchadmnsd.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtcutnxzhx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jianghu66.top/gtjhupmbfk.html

[T35] Lua：字典表
来源：http://hz.jiagoushi.top/gtuwdylwqs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.havefunace.top/gtpwweqizp.html

[T36] Lua：函数
来源：http://hz.jiagoushi.top/gtkdhygkhm.html

function add(a, b) return a + b end
来源：http://hz.yvedp.cn/gtzqovlpns.html

[T37] Lua：字符串拼接
来源：http://hz.hnxiangtu.top/gtabcozihz.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gttiqmyzej.html

[T38] Lua：条件
来源：http://hz.smart0.xyz/gtjlbsjtyy.html

if x > 0 then print("正") end
来源：http://hz.aibaodan.cn/gtdatlfmea.html

[T39] Lua：模式匹配
来源：http://hz.xinyue.icu/gtbmnrjvfr.html

string.find(s, "%d+")
来源：http://hz.bjfxy.top/gtbynusxfq.html

[T40] Lua：元表
来源：http://hz.jlsjyb.cn/gtrjimszle.html

setmetatable({}, { __index = base })
来源：http://hz.xuetiantiany.cn/gtjqzqfcdu.html

[T41] Perl：Hello World
来源：http://hz.yangfankeji.com/gtpzngneqz.html

print "Hello\n";
来源：http://hz.zycfv.cn/gtahebasex.html

[T42] Perl：变量类型
来源：http://hz.c1oappe.top/gtfnkbvxxs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.316326.xyz/gteqhhdgmv.html

[T43] Perl：字符串插值
来源：http://hz.yuxming.cn/gtevkpwobc.html

"值: $a"
来源：http://hz.sufxvd.cn/gtfaylsyle.html

[T44] Perl：条件
来源：http://hz.cucudq.cn/gtlevelhbn.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gttacahtaq.html

[T45] Perl：数组遍历
来源：http://hz.zdqjudy.top/gtsiaozhji.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtykcazxaj.html

[T46] Perl：哈希操作
来源：http://hz.hnxiangtu.top/gtsrvumvmp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.vqdsnc.cn/gtmwpxebeb.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtlvgerbil.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtkxjvmuqn.html

[T48] Perl：正则替换
来源：http://hz.52xcode.cn/gtjlotjrpb.html

$s =~ s/old/new/g;
来源：http://hz.yongpay.top/gtyoufntsy.html

[T49] Perl：函数
来源：http://hz.shzxlz.cn/gtqawhtsrp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ivvv.top/gtjtdwnosb.html

[T50] Perl：逐行读文件
来源：http://hz.xuetiantiany.cn/gthfclkbrd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.haohaochexian.top/gttzgczwxt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.dashuyun.cn/gtyqmaekhv.html

[T51] Scala：Hello World
来源：http://hz.aibaodan.cn/gtqdwcsuqe.html

println("Hello")
来源：http://hz.gotoacloud.top/gtiwphcrqk.html

[T52] Scala：变量
来源：http://hz.316326.xyz/gtqrebappe.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangkeji.top/gtelwptuti.html

[T53] Scala：字符串插值
来源：http://hz.snrcjt.cn/gtmgbviigr.html

s"值: $b"
来源：http://hz.zdqjudy.top/gtthvvsvrz.html

[T54] Scala：集合映射
来源：http://hz.zhoulong.xyz/gtikxjxdpt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.havefunace.top/gtvcntodoc.html

[T55] Scala：集合过滤
来源：http://hz.yueranfly.top/gtdmefbncz.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.mhx1999.top/gtopdydhuz.html

[T56] Scala：样例类
来源：http://hz.ivvv.top/gtsaxolxig.html

case class User(name: String, age: Int)
来源：http://hz.redwolf501.top/gtqdzjquok.html

[T57] Scala：模式匹配
来源：http://hz.yj20258.top/gtguqbcldf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtfgxmeomu.html

[T58] Scala：函数定义
来源：http://hz.chenjidiqi.icu/gturfvgfgw.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.fzhhl.top/gtimxmnwca.html

[T59] Scala：循环
来源：http://hz.quarkkingdee.top/gtcowpzjsc.html

for (i <- 1 to 10) println(i)
来源：http://hz.sweek.top/gtfurkfgcn.html

[T60] Scala：折叠
来源：http://hz.redwolf501.top/gtewcscbpm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gogol.net.cn/gtxwvxmuao.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtosjfoeqq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtcjbjvkmr.html

================================================================================
来源：http://hz.chenlongwang.top/gtcbjzenuq.html

[U01] Py：创建虚拟环境
来源：http://hz.zhiwuduotai.top/gtvjyvsqzq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gotoacloud.top/gtpygrwhcb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.c1oappe.top/gttdollgzu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.daxiang520.top/gtjveiezfl.html

[U03] Py：加载 .env 配置
来源：http://hz.bjfxy.top/gtqqksfvzo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hywenlv.cn/gtdojkepgl.html

[U04] Py：变量调试打印
来源：http://hz.yj20258888.top/gtpcpuwauo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xuetiantiany.cn/gtmjxzoxas.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigufen.top/gtoqsawyqg.html

list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtckjyhday.html

[U06] Py：合并两个字典
来源：http://hz.svipenyu.cn/gtjpobultm.html

{**a, **b}
来源：http://hz.tianlin.xyz/gtzvmjrups.html

[U07] Py：反转字典键值
来源：http://hz.guowangkeji.top/gtttucwprr.html

{v: k for k, v in d.items()}
来源：http://hz.sweek.top/gtndnbpnjq.html

[U08] Py：展平二维列表
来源：http://hz.yongpay.top/gthcfwicvu.html

[y for x in nested for y in x]
来源：http://hz.yj20258888.top/gtydraelzu.html

[U09] Py：字典取最大值的键
来源：http://hz.hfpthk.cn/gtibrbegqc.html

max(d, key=d.get)
来源：http://hz.yonumen.top/gtxzdxqecj.html

[U10] Py：按值排序字典
来源：http://hz.zhijiandao.cn/gtrqqsnwaw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cheryme.top/gtqzywocud.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtonebysox.html

(x * 2 for x in arr)
来源：http://hz.daxiang520.top/gtunxozqjd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gotoacloud.top/gtbclrxrnw.html

Counter(arr).most_common(3)
来源：http://hz.zhoulong.xyz/gtxkxfmmlj.html

[U13] Py：固定长度队列
来源：http://hz.ppjwa.cn/gtdyvxvlds.html

deque(maxlen=10)
来源：http://hz.jinqigfzy.top/gtoitjrdec.html

[U14] Py：分组收集到列表
来源：http://hz.yj20258888.top/gtrfxpkgle.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtrunolzny.html

[U15] Py：高精度计时
来源：http://hz.yonumen.top/gtehryvlnq.html

t = time.perf_counter()
来源：http://hz.bjfxy.top/gtmkwilqyp.html

[U16] Py：命令行参数解析
来源：http://hz.xylfe.cn/gtazdblgvf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtbupkpeza.html

[U17] Py：初始化日志
来源：http://hz.zhengqikj.top/gtncwttyyw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.redwolf501.top/gtibcapkht.html

[U18] Py：预编译正则
来源：http://hz.yongpay.top/gtjjvhfasj.html

pat = re.compile(r"\d+")
来源：http://hz.hnxiangtu.top/gtalnqldid.html

[U19] Py：正则替换带回调
来源：http://hz.zhaomingkeji.xyz/gtwpprojnv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.tanke756.top/gtpqolipwy.html

[U20] Py：缓存函数结果
来源：http://hz.yueranfly.top/gtrprsinmy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgufenzy.top/gtdeledcep.html

[U21] Py：自定义上下文管理器
来源：http://hz.haohaochexian.top/gtptxcddec.html

@contextlib.contextmanager
来源：http://hz.cqqwz.cn/gtaftsmpwc.html

[U22] Py：矩阵转置
来源：http://hz.guowangkeji.top/gtfjoaxcfv.html

list(zip(*m))
来源：http://hz.guannengcc.top/gtqlhnlwbs.html

[U23] Py：分块读取大文件
来源：http://hz.hnqzz.top/gtygvsmiby.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sufxvd.cn/gtmggxyhqi.html

[U24] Py：路径操作
来源：http://hz.jinyuanbaomall.cn/gtplhrzabp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gttvqwfmsh.html

[U25] Py：CSV 按字典读
来源：http://hz.xziqi.cn/gtyzdvooht.html

csv.DictReader(f)
来源：http://hz.gaohongyu789.top/gtifhgxipv.html

[U26] Py：并发下载
来源：http://hz.yj202588.top/gtbxnnecze.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.daria6918.cn/gtrvoafxdf.html

[U27] Py：异步 HTTP
来源：http://hz.zdqjudy.top/gtanpxhepz.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tianlin.xyz/gtgzxvjpda.html

[U28] Py：类型别名
来源：http://hz.guannengcc.top/gtivreprvi.html

UserId = int
来源：http://hz.feifeiyinyue.top/gtgcnifdow.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtevssgyuw.html

@property 与 @x.setter 配合
来源：http://hz.birdmap.top/gtalyksqcp.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtfrwggxuz.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtdudjybmd.html

[U31] Py：单测
来源：http://hz.yongpay.top/gtloakzstx.html

python -m pytest -q
来源：http://hz.hongshengwenyu.top/gtmzqrgvxz.html

[U32] Py：代码格式化
来源：http://hz.wangdashe.top/gthnuqknzs.html

ruff format . && ruff check --fix .
来源：http://hz.vqdsnc.cn/gtukhluesy.html

[U33] Py：打包发布
来源：http://hz.cqqwz.cn/gtbeigxsbh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhixingplan.top/gtbevostvb.html

[U34] Py：判断编码
来源：http://hz.smart0.xyz/gtcetdijqh.html

chardet.detect(raw)
来源：http://hz.shzxlz.cn/gtflcrlbjv.html

[U35] Py：发送邮件
来源：http://hz.ivvv.top/gtqxmtwlqp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhijiandao.cn/gtpjndzahn.html

[U36] Py：定时任务
来源：http://hz.hysaishi.cn/gtbqtkurvv.html

schedule.every(10).minutes.do(job)
来源：http://hz.9152youxi.cn/gtdshklywz.html

[U37] Py：读写 Excel
来源：http://hz.haohaochexian.top/gtklrjdmec.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hnxiangtu.top/gtbghoodxs.html

[U38] Py：获取脚本所在目录
来源：http://hz.iojbl.cn/gtmhrejmhi.html

Path(__file__).resolve().parent
来源：http://hz.sxryk.cn/gtzscnxheu.html

[U39] Py：判断是否在交互环境
来源：http://hz.andypj.xyz/gtdmjdlopb.html

sys.stdout.isatty()
来源：http://hz.gogol.net.cn/gtlcmpqied.html

[U40] Py：打印到标准错误
来源：http://hz.jinqigufen.top/gtykkyguzl.html

print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtllfkozus.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ehwqpu.com/gthuplocku.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtriumqpvc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinqigufen.top/gtodqbbxwx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hongshengwenyu.top/gtwnsielqb.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtbmhcmwgr.html

namespace App\Http;
来源：http://hz.shanyushiyangtech.top/gtdjsfhkrs.html

[U44] PHP：开启严格类型
来源：http://hz.fengsongda.top/gtdfvprqyt.html

declare(strict_types=1);
来源：http://hz.xziqi.cn/gtetsfeqpr.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydzc1.top/gtyiheptok.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtoolcfiiy.html

[U46] PHP：可空类型
来源：http://hz.yj202588.top/gtguaglucp.html

?string $name = null
来源：http://hz.shanyushiyangtech.top/gtfqpgawfh.html

[U47] PHP：联合类型
来源：http://hz.tian-w.cn/gtyrzkjrni.html

int|string $id
来源：http://hz.sxryk.cn/gtfllzkexn.html

[U48] PHP：纯枚举
来源：http://hz.xziqi.cn/gtoivtgjfr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cashguo.top/gtozdaksao.html

[U49] PHP：只读属性
来源：http://hz.zhaomingkeji.xyz/gtaxfaiwxh.html

public readonly string $name
来源：http://hz.svipenyu.cn/gtlbimcqgg.html

[U50] PHP：构造器属性提升
来源：http://hz.aizwys.cn/gtrwzrvbhi.html

public function __construct(private int $id) {}
来源：http://hz.jqgufenzy.top/gtpwlypyjj.html

[U51] PHP：数组解构
来源：http://hz.yangfankeji.com/gtgzmrpogf.html

[$a, $b] = $arr;
来源：http://hz.cdnleiting.top/gtkojeypty.html

[U52] PHP：箭头函数
来源：http://hz.ywan-chungtsiang.top/gtlztykfyp.html

$double = fn($x) => $x * 2;
来源：http://hz.zdqjudy.top/gtwajlspuw.html

[U53] PHP：空合并运算符
来源：http://hz.zhaomingkeji.xyz/gtrtktrvjn.html

$v = $a ?? $b ?? "default";
来源：http://hz.shzxlz.cn/gtldqzibef.html

[U54] PHP：空安全调用
来源：http://hz.shuidangran.top/gtffblvuxu.html

$obj?->method()
来源：http://hz.gotoacloud.top/gtnvehnczc.html

[U55] PHP：match 表达式
来源：http://hz.hongshengwenyu.top/gtaaqmqhfe.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhaomingkeji.xyz/gtsczgydyz.html

[U56] PHP：命名参数
来源：http://hz.chenzaomai.com/gtysrtfrsb.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtjddoeaqn.html

[U57] PHP：字符串插值
来源：http://hz.chenlongwang.top/gtfdgpritn.html

"值: {$a}"
来源：http://hz.0kj1m.cn/gtvdbaosnd.html

[U58] PHP：数组三件套
来源：http://hz.smart0.xyz/gtaecyxkzb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ppjwa.cn/gtngwmyerd.html

[U59] PHP：自定义排序
来源：http://hz.hnxiangtu.top/gtodwjufqe.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ybcxt.top/gtrboigvrh.html

[U60] PHP：JSON 编解码
来源：http://hz.havefunace.top/gtgstngcgh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ywan-chungtsiang.top/gtxknacbqn.html

[U61] PHP：正则
来源：http://hz.ybcxt.top/gtuzaebxlz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtszvjqwwm.html

[U62] PHP：日期对象
来源：http://hz.wangdashe.top/gtmnmdfoog.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinyuanbaomall.cn/gtlgycvoot.html

[U63] PHP：文件读写
来源：http://hz.zhengqikj.top/gthxfabghl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.dianchejie.cn/gtwiprtzlq.html

[U64] PHP：目录遍历
来源：http://hz.cucudq.cn/gttlouaryq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zycfv.cn/gtqufgmbhf.html

[U65] PHP：会话
来源：http://hz.svipenyu.cn/gtvkqwtagg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hfpthk.cn/gtwtjtnxea.html

[U66] PHP：设置 Cookie
来源：http://hz.sweek.top/gtufacnnay.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.cashguo.top/gtvayxegyh.html

[U67] PHP：处理文件上传
来源：http://hz.jyoumei.cn/gtjkgjbfqc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ydzc1.top/gtfjpuazws.html

[U68] PHP：PDO 连接
来源：http://hz.gzhubu.top/gtgwbakwso.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tianlin.xyz/gtekrutuzx.html

[U69] PHP：PDO 预处理
来源：http://hz.tianlin.xyz/gtmhejleke.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.shzxlz.cn/gtnsszuqox.html

[U70] PHP：PDO 事务
来源：http://hz.xuanzx.com/gtcrefxywn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hnxiangtu.top/gtlgtvrbcp.html

[U71] PHP：抛出异常
来源：http://hz.daxiang520.top/gtxxdinnwk.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtwwsbybzo.html

[U72] PHP：写错误日志
来源：http://hz.sufxvd.cn/gtitszmrud.html

error_log("失败: " . $e->getMessage());
来源：http://hz.pycfn.com/gtwpstgzoq.html

[U73] PHP：读取 ini 配置
来源：http://hz.feifeiyinyue.top/gtbrmfllkk.html

parse_ini_file("config.ini", true)
来源：http://hz.ivvv.top/gtwhdhmzzb.html

[U74] PHP：读取环境变量
来源：http://hz.hywenlv.cn/gtjajpopdg.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shuidangran.top/gtkhooyfwd.html

[U75] PHP：依赖注入
来源：http://hz.hywenlv.cn/gtwwfjfzuo.html

composer require psr/container
来源：http://hz.gzhubu.top/gtgmamkxih.html

[U76] PHP：简单路由
来源：http://hz.bjfxy.top/gtysxkrsfv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.bjfxy.top/gtztntiixu.html

[U77] PHP：模板渲染
来源：http://hz.dianchejie.cn/gtxplhkrnx.html

composer require twig/twig
来源：http://hz.hnxiangtu.top/gtdsqinixw.html

[U78] PHP：单元测试
来源：http://hz.daxiang520.top/gtfdcoufsz.html

composer require --dev phpunit/phpunit
来源：http://hz.tanke756.top/gtblffzmgd.html


<!-- 参考信息 -->