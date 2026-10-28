代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtvjsigkgp.html

[S55] C++：结构化绑定
来源：http://hz.yanxiufei.cn/gtkkwpvdum.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ywan-chungtsiang.top/gtgbobtdlx.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gthwdiciaz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gthtsftdkw.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtlpzzhgex.html

constexpr int N = 10;
来源：http://hz.hammf.cn/gtpjrjoepr.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtcxrqohln.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtphsrttyq.html

[S59] C++：静态断言
来源：http://hz.0kj1m.cn/gtfyhxxjvw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.kuanghao11.cn/gtvfymjmfo.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtmxcabqnc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.dashuyun.cn/gtosspqzpy.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtzdzofadu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinghuilouyu.cn/gtmtyrkdbl.html

================================================================================
来源：http://hz.jianghu66.top/gtaefgncpi.html

[T01] Kotlin：Hello World
来源：http://hz.iojbl.cn/gttnmliyzd.html

println("Hello")
来源：http://hz.nanxuanxn.top/gtofyglubp.html

[T02] Kotlin：变量
来源：http://hz.andypj.xyz/gtfsbbbtpm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gttdlxfsls.html

[T03] Kotlin：字符串模板
来源：http://hz.redwolf501.top/gtpevanmet.html

"值: $b"
来源：http://hz.jlsjyb.cn/gtadsckqht.html

[T04] Kotlin：空安全
来源：http://hz.yuxming.cn/gtiahatjmt.html

val n: String? = null;  n?.length
来源：http://hz.yvedp.cn/gtbpwolvjh.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtcrsretlb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.andypj.xyz/gtlyhoyhzb.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtnwiqzhzm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.haohaochexian.top/gtaatgzgzs.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigufen.top/gtqcaovwop.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.havefunace.top/gtweuivxvw.html

[T08] Kotlin：数据类
来源：http://hz.quarkkingdee.top/gtgahrsbyj.html

data class User(val name: String, val age: Int)
来源：http://hz.bjfxy.top/gtbeisgiqz.html

[T09] Kotlin：扩展函数
来源：http://hz.yonumen.top/gtfhyiafsd.html

fun String.exclaim() = this + "!"
来源：http://hz.zdqjudy.top/gtnpnqkorl.html

[T10] Kotlin：默认参数
来源：http://hz.cashguo.top/gtkwsdiaip.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daria6918.cn/gtqojttght.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gtombniuyv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtxbbnoojr.html

[T12] Kotlin：解构声明
来源：http://hz.zhixingplan.top/gthcyfhehw.html

val (a, b) = Pair(1, 2)
来源：http://hz.zycfv.cn/gtydsvufvp.html

[T13] Kotlin：只读 Map
来源：http://hz.sufxvd.cn/gtkwxxmlja.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtyltlqavu.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtgbesddlo.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtptrylzfb.html

[T15] Kotlin：接口
来源：http://hz.gogol.net.cn/gtnminrkzx.html

interface Shape { fun area(): Double }
来源：http://hz.gogol.net.cn/gttmfvbxqa.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtpfxqwegt.html

print("Hello")
来源：http://hz.bjfxy.top/gtnnviczkb.html

[T17] Swift：变量与常量
来源：http://hz.nanxuanxn.top/gtcljmkaht.html

var a = 1;  let b = 2
来源：http://hz.jqgfzy.top/gtksnekebi.html

[T18] Swift：字符串插值
来源：http://hz.pengpengdd.cyou/gtbuzitgyu.html

"值: \(b)"
来源：http://hz.ywan-chungtsiang.top/gtdwloccqf.html

[T19] Swift：可选绑定
来源：http://hz.zhaomingkeji.xyz/gtevzittqo.html

if let n = opt { print(n) }
来源：http://hz.hnxiangtu.top/gtxiaftgvo.html

[T20] Swift：数组操作
来源：http://hz.nanxuanxn.top/gtisabrndp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtjnbnccnr.html

[T21] Swift：遍历
来源：http://hz.andypj.xyz/gtmmzslhvn.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtcfilgsyq.html

[T22] Swift：字典
来源：http://hz.gotoacloud.top/gtjcfipcis.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yonumen.top/gtmgtmbevn.html

[T23] Swift：函数
来源：http://hz.meibo888.top/gtlyclqqcc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtnblicjzs.html

[T24] Swift：闭包
来源：http://hz.dianchejie.cn/gtbgpkdakb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtfksivoyv.html

[T25] Swift：结构体
来源：http://hz.haohaochexian.top/gtiwjtpvek.html

struct P { var x: Int }
来源：http://hz.yongpay.top/gtkzplppjm.html

[T26] Swift：类与重写
来源：http://hz.tanke756.top/gtojzmxqct.html

class A: Base { override func f() {} }
来源：http://hz.ivvv.top/gtbfbscrxj.html

[T27] Swift：错误处理
来源：http://hz.c1oappe.top/gtzpioevnd.html

do { try f() } catch { print(error) }
来源：http://hz.jyoumei.cn/gtbsvyihpc.html

[T28] Swift：枚举
来源：http://hz.aizwys.cn/gthrzbpywj.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtmmlfnnib.html

[T29] Swift：guard 提前返回
来源：http://hz.aibaodan.cn/gtmcnqlpxo.html

guard let x = opt else { return }
来源：http://hz.sysykeji.top/gtaigytsdk.html

[T30] Swift：协议
来源：http://hz.sufxvd.cn/gttdietmfm.html

protocol Shape { func area() -> Double }
来源：http://hz.hnqzz.top/gtemuxwjqb.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtwdwgnofl.html

print("Hello")
来源：http://hz.sxryk.cn/gtozvyakcc.html

[T32] Lua：局部变量
来源：http://hz.wangshuangyany.cn/gtirihogbr.html

local a = 1
来源：http://hz.gaohongyu789.top/gtqayynvsb.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtuwajornd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yongpay.top/gttabnjphh.html

[T34] Lua：遍历表
来源：http://hz.ppjwa.cn/gtsgnohegh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sysykeji.top/gtvxkyoynd.html

[T35] Lua：字典表
来源：http://hz.zhaomingkeji.xyz/gterfayaih.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hysaishi.cn/gtjvpcwvlb.html

[T36] Lua：函数
来源：http://hz.tian-w.cn/gtnhoocidj.html

function add(a, b) return a + b end
来源：http://hz.yueranfly.top/gtucupetaa.html

[T37] Lua：字符串拼接
来源：http://hz.hfpthk.cn/gtbmhkpddq.html

"a" .. "b"
来源：http://hz.jqgufenzy.top/gtomnantgh.html

[T38] Lua：条件
来源：http://hz.hfpthk.cn/gtcdruuvmw.html

if x > 0 then print("正") end
来源：http://hz.vqdsnc.cn/gtqydmaqkx.html

[T39] Lua：模式匹配
来源：http://hz.aizwys.cn/gtjplxngbh.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtkxkwcjri.html

[T40] Lua：元表
来源：http://hz.meibo888.top/gtkunzzmxg.html

setmetatable({}, { __index = base })
来源：http://hz.andypj.xyz/gtisjarrpo.html

[T41] Perl：Hello World
来源：http://hz.sufxvd.cn/gtnwdxapjq.html

print "Hello\n";
来源：http://hz.fzhhl.top/gtkoesesdx.html

[T42] Perl：变量类型
来源：http://hz.redwolf501.top/gtnddqoper.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtpnugpzvj.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtvaznlscz.html

"值: $a"
来源：http://hz.c1oappe.top/gtdxxzfyqj.html

[T44] Perl：条件
来源：http://hz.jinyuanbaomall.cn/gtejizkiqp.html

if ($a > 0) { print "正"; }
来源：http://hz.shuidangran.top/gtwjyqsbpt.html

[T45] Perl：数组遍历
来源：http://hz.c1oappe.top/gtxtjtwfos.html

for my $x (@arr) { print $x; }
来源：http://hz.yj20258888.top/gtjyddiyyl.html

[T46] Perl：哈希操作
来源：http://hz.smart0.xyz/gtqyowhhcp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.guannengcc.top/gtglmktgub.html

[T47] Perl：正则捕获
来源：http://hz.quarkkingdee.top/gtphjljfpo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtlzaygyli.html

[T48] Perl：正则替换
来源：http://hz.nanxinkj.top/gtqjdtzocg.html

$s =~ s/old/new/g;
来源：http://hz.hfpthk.cn/gtmtnmekog.html

[T49] Perl：函数
来源：http://hz.pycfn.com/gtvohdzvdf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yonumen.top/gtdqtgeond.html

[T50] Perl：逐行读文件
来源：http://hz.jiagoushi.top/gtetghzymk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hammf.cn/gtmvshiogz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.chenjidiqi.icu/gtaosonylx.html

[T51] Scala：Hello World
来源：http://hz.smart0.xyz/gtalwekvmb.html

println("Hello")
来源：http://hz.tianlin.xyz/gtnrcfnvcw.html

[T52] Scala：变量
来源：http://hz.cdnleiting.top/gtjgvpymqm.html

val a = 1;  var b = 2
来源：http://hz.xylfe.cn/gthjanuqkw.html

[T53] Scala：字符串插值
来源：http://hz.xylfe.cn/gtzqcxhjfx.html

s"值: $b"
来源：http://hz.ivvv.top/gtfrhtfrer.html

[T54] Scala：集合映射
来源：http://hz.nwbrower.top/gtttmlipas.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jianghu66.top/gtgbhnerlz.html

[T55] Scala：集合过滤
来源：http://hz.jqgfzy.top/gtowmshbhv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.52xcode.cn/gtmymsmdgh.html

[T56] Scala：样例类
来源：http://hz.svipenyu.cn/gtnfkutfis.html

case class User(name: String, age: Int)
来源：http://hz.yongpay.top/gtnujqgkst.html

[T57] Scala：模式匹配
来源：http://hz.pycfn.com/gtwgrpwqgh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tianlin.xyz/gttrxlhbcl.html

[T58] Scala：函数定义
来源：http://hz.jinghuilouyu.cn/gteaerjzrj.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenzaomai.com/gthovorgai.html

[T59] Scala：循环
来源：http://hz.52xcode.cn/gteykwtxjc.html

for (i <- 1 to 10) println(i)
来源：http://hz.feifeiyinyue.top/gtoxrblxzt.html

[T60] Scala：折叠
来源：http://hz.jinghuilouyu.cn/gtwihgbjlo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zhaomingkeji.xyz/gtfvypvmsw.html

================================================================================
来源：http://hz.zhoulong.xyz/gttcsnykxc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xylfe.cn/gthqmefwlj.html

================================================================================
来源：http://hz.ydzc1.top/gtfvkebtur.html

[U01] Py：创建虚拟环境
来源：http://hz.shanyushiyangtech.top/gtqhqeqmnn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhongyouzk.top/gtsvxexjbf.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shangyingyoupin.top/gtqslttaid.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gaohongyu789.top/gtutmaqauf.html

[U03] Py：加载 .env 配置
来源：http://hz.tian-w.cn/gtajdigvzg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtpwzlnbvz.html

[U04] Py：变量调试打印
来源：http://hz.gzhubu.top/gtcvlklxnj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.birdmap.top/gtdzfbbtbx.html

[U05] Py：列表去重且保序
来源：http://hz.aizwys.cn/gtwxgrnuri.html

list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gttjqskrdp.html

[U06] Py：合并两个字典
来源：http://hz.guowangkeji.top/gtsyijfqdi.html

{**a, **b}
来源：http://hz.zhongyouzk.top/gtgphnkrqj.html

[U07] Py：反转字典键值
来源：http://hz.shuidangran.top/gtyuqliasf.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtnwajqmwp.html

[U08] Py：展平二维列表
来源：http://hz.vqdsnc.cn/gtbeavrozi.html

[y for x in nested for y in x]
来源：http://hz.chenlongwang.top/gtfuyjbfao.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gtsqlaybku.html

max(d, key=d.get)
来源：http://hz.jqgfzy.top/gtwbkbkede.html

[U10] Py：按值排序字典
来源：http://hz.hnxiangtu.top/gtiaivrglc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gaohongyu789.top/gtdweqqgjx.html

[U11] Py：生成器表达式
来源：http://hz.yuxming.cn/gtomkazqir.html

(x * 2 for x in arr)
来源：http://hz.jiagoushi.top/gtemyltupt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jiagoushi.top/gtwtcsgkqw.html

Counter(arr).most_common(3)
来源：http://hz.aizwys.cn/gtwpfbdvpr.html

[U13] Py：固定长度队列
来源：http://hz.pycfn.com/gtehhijajq.html

deque(maxlen=10)
来源：http://hz.shanyushiyangtech.top/gttvmijstv.html

[U14] Py：分组收集到列表
来源：http://hz.daria6918.cn/gthnceiqrn.html

defaultdict(list)
来源：http://hz.svipenyu.cn/gtlicmuqzy.html

[U15] Py：高精度计时
来源：http://hz.hysaishi.cn/gtqsixbcfo.html

t = time.perf_counter()
来源：http://hz.ehwqpu.com/gthzceitig.html

[U16] Py：命令行参数解析
来源：http://hz.hammf.cn/gtljlsaocx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jiagoushi.top/gtuiejwsxh.html

[U17] Py：初始化日志
来源：http://hz.tianlin.xyz/gtubqwcjlg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yuxming.cn/gtalsiacrb.html

[U18] Py：预编译正则
来源：http://hz.smart0.xyz/gtugywasxw.html

pat = re.compile(r"\d+")
来源：http://hz.shanyushiyangtech.top/gtszazzjcr.html

[U19] Py：正则替换带回调
来源：http://hz.yvedp.cn/gtaybqgqvd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jyoumei.cn/gtswokpdst.html

[U20] Py：缓存函数结果
来源：http://hz.jinqigufen.top/gtqnabyunq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgufenzy.top/gtyzbrgbtg.html

[U21] Py：自定义上下文管理器
来源：http://hz.cashguo.top/gtxwfbvoca.html

@contextlib.contextmanager
来源：http://hz.gaohongyu789.top/gtzryuxvsn.html

[U22] Py：矩阵转置
来源：http://hz.zhoulong.xyz/gteejistfl.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtvqiunawi.html

[U23] Py：分块读取大文件
来源：http://hz.jinqigfzy.top/gtdetuupxu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jianghu66.top/gtkipxhhuw.html

[U24] Py：路径操作
来源：http://hz.yonumen.top/gtetuxgvtv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.bjfxy.top/gtxdqjxfej.html

[U25] Py：CSV 按字典读
来源：http://hz.yangfankeji.com/gtpyorsgwh.html

csv.DictReader(f)
来源：http://hz.sxryk.cn/gtstfcicsa.html

[U26] Py：并发下载
来源：http://hz.zhengqikj.top/gtlhmittom.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenjidiqi.icu/gtkfiodwax.html

[U27] Py：异步 HTTP
来源：http://hz.cdnleiting.top/gtalngnouy.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sysykeji.top/gtflusyemx.html

[U28] Py：类型别名
来源：http://hz.yvedp.cn/gtxkitdrss.html

UserId = int
来源：http://hz.snrcjt.cn/gtacdckaav.html

[U29] Py：属性校验
来源：http://hz.cdnleiting.top/gtmityzube.html

@property 与 @x.setter 配合
来源：http://hz.zhijiandao.cn/gttnzhonbt.html

[U30] Py：数据类
来源：http://hz.birdmap.top/gtfszjnvjp.html

@dataclass(slots=True)
来源：http://hz.chenzaomai.com/gtrluunjky.html

[U31] Py：单测
来源：http://hz.jqgufenzy.top/gtyumdufps.html

python -m pytest -q
来源：http://hz.316326.xyz/gtcknbvgpc.html

[U32] Py：代码格式化
来源：http://hz.hysaishi.cn/gtxhgphmlr.html

ruff format . && ruff check --fix .
来源：http://hz.gzhubu.top/gtjopaubpa.html

[U33] Py：打包发布
来源：http://hz.yj20258888.top/gtuhqbzlql.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jlsjyb.cn/gtvijszdpu.html

[U34] Py：判断编码
来源：http://hz.yj20258.top/gtwawqeqta.html

chardet.detect(raw)
来源：http://hz.9152youxi.cn/gtifgxnssp.html

[U35] Py：发送邮件
来源：http://hz.yonumen.top/gtnudsittp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxinkj.top/gtwzbeoukw.html

[U36] Py：定时任务
来源：http://hz.ppjwa.cn/gttuhvwccq.html

schedule.every(10).minutes.do(job)
来源：http://hz.ybcxt.top/gtsnetdbev.html

[U37] Py：读写 Excel
来源：http://hz.cashguo.top/gtpjbfglio.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xingfuxueyuan.xyz/gtxpqcemfw.html

[U38] Py：获取脚本所在目录
来源：http://hz.sweek.top/gtopgsitxz.html

Path(__file__).resolve().parent
来源：http://hz.chenjidiqi.icu/gtrvitzuit.html

[U39] Py：判断是否在交互环境
来源：http://hz.52xcode.cn/gtbiwypfvm.html

sys.stdout.isatty()
来源：http://hz.ybcxt.top/gtonhniqta.html

[U40] Py：打印到标准错误
来源：http://hz.dianchejie.cn/gtvggxyean.html

print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtmyswfrou.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yonumen.top/gtlcqozjnj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yuxming.cn/gtckfegdjv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtgkgrdgqw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sweek.top/gtflkucija.html

[U43] PHP：声明命名空间
来源：http://hz.birdmap.top/gtvgimliil.html

namespace App\Http;
来源：http://hz.shanyushiyangkeji.top/gthbukgwfu.html

[U44] PHP：开启严格类型
来源：http://hz.aizwys.cn/gtuxihuzhw.html

declare(strict_types=1);
来源：http://hz.gzhubu.top/gtppsegnbm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.mhx1999.top/gtqesadpxq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gthwoteett.html

[U46] PHP：可空类型
来源：http://hz.zhengqikj.top/gtvihrzirp.html

?string $name = null
来源：http://hz.daxiang520.top/gtowbzkazz.html

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gtiqsngkzs.html

int|string $id
来源：http://hz.smart0.xyz/gtkauhfjaj.html

[U48] PHP：纯枚举
来源：http://hz.shzxlz.cn/gtdqqgerlv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ivvv.top/gtfwhkjdir.html

[U49] PHP：只读属性
来源：http://hz.hysaishi.cn/gtkslgkuhd.html

public readonly string $name
来源：http://hz.pengpengdd.cyou/gtuaepdadf.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtjorzoirc.html

public function __construct(private int $id) {}
来源：http://hz.tianlin.xyz/gtjcxmsiac.html

[U51] PHP：数组解构
来源：http://hz.xylfe.cn/gtwyxmmnim.html

[$a, $b] = $arr;
来源：http://hz.cashguo.top/gtlagsgmul.html

[U52] PHP：箭头函数
来源：http://hz.gaohongyu789.top/gtuzlqkohe.html

$double = fn($x) => $x * 2;
来源：http://hz.zhaomingkeji.xyz/gtywzzlqqe.html

[U53] PHP：空合并运算符
来源：http://hz.ywan-chungtsiang.top/gtlyikkjoy.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhijiandao.cn/gtmeotawzt.html

[U54] PHP：空安全调用
来源：http://hz.yj202588.top/gtbyxfkgle.html

$obj?->method()
来源：http://hz.chenlongwang.top/gtjyhoobnc.html

[U55] PHP：match 表达式
来源：http://hz.fzhhl.top/gtbqvwnljq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yueranfly.top/gtcxngbclz.html

[U56] PHP：命名参数
来源：http://hz.jinqigfzy.top/gtpdvbgvsr.html

f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtnvsnswnn.html

[U57] PHP：字符串插值
来源：http://hz.cheryme.top/gtyfnbqabb.html

"值: {$a}"
来源：http://hz.jianghu66.top/gtskhntkvl.html

[U58] PHP：数组三件套
来源：http://hz.chenlongwang.top/gtritgoust.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.chenzaomai.com/gthdglzufb.html

[U59] PHP：自定义排序
来源：http://hz.shanyushiyangtech.top/gtoihnjwdd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtmzkbpfkq.html

[U60] PHP：JSON 编解码
来源：http://hz.yangfankeji.com/gtyjccvgpy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.tianlin.xyz/gtvkyelwpn.html

[U61] PHP：正则
来源：http://hz.shangyingyoupin.top/gtphdnjzix.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtfdeyjpre.html

[U62] PHP：日期对象
来源：http://hz.feifeiyinyue.top/gtsrnjciim.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.tanke756.top/gtzwvqlrtg.html

[U63] PHP：文件读写
来源：http://hz.jqgufenzy.top/gtdaiuuyrp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangkeji.top/gtqzgxtimd.html

[U64] PHP：目录遍历
来源：http://hz.iojbl.cn/gtksnxdsnf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tian-w.cn/gtrnscgmwp.html

[U65] PHP：会话
来源：http://hz.shzxlz.cn/gtxylryrlx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dianchejie.cn/gtkbxqgavc.html

[U66] PHP：设置 Cookie
来源：http://hz.xinyue.icu/gtijtisgvn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.nwbrower.top/gtljmtxjrg.html

[U67] PHP：处理文件上传
来源：http://hz.zhiwuduotai.top/gtycagdcqw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.gzhubu.top/gtuyronmtc.html

[U68] PHP：PDO 连接
来源：http://hz.xingfuxueyuan.xyz/gtuwxvhzav.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.tianlin.xyz/gtqqnpxnll.html

[U69] PHP：PDO 预处理
来源：http://hz.jinqigufen.top/gtqqgmgrvi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nanxuanxn.top/gteieaygkx.html

[U70] PHP：PDO 事务
来源：http://hz.jlsjyb.cn/gtyhlzalye.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yvedp.cn/gtwsapatad.html

[U71] PHP：抛出异常
来源：http://hz.cheryme.top/gtcgjdgjdd.html

throw new RuntimeException("失败", 500);
来源：http://hz.yuanzhike.top/gtlcsexrnh.html

[U72] PHP：写错误日志
来源：http://hz.sysykeji.top/gtkikssrnf.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cheryme.top/gtyroflfzs.html

[U73] PHP：读取 ini 配置
来源：http://hz.smart0.xyz/gtiosiwxwx.html

parse_ini_file("config.ini", true)
来源：http://hz.cheryme.top/gtftmlnkui.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtrvnlmayo.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yj20258888.top/gtzhbvgdeh.html

[U75] PHP：依赖注入
来源：http://hz.zycfv.cn/gtzrjjuqcc.html

composer require psr/container
来源：http://hz.c1oappe.top/gtrbljecwo.html

[U76] PHP：简单路由
来源：http://hz.meibo888.top/gtxiebobia.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.sweek.top/gtlchmpaou.html

[U77] PHP：模板渲染
来源：http://hz.ybcxt.top/gtimswdsrk.html

composer require twig/twig
来源：http://hz.ydzc1.top/gtjkfsrgcg.html

[U78] PHP：单元测试
来源：http://hz.cashguo.top/gtmgvyoqya.html

composer require --dev phpunit/phpunit
来源：http://hz.hnqzz.top/gtzdixzgro.html

[U79] PHP：静态分析
来源：http://hz.dashuyun.cn/gtetpskkec.html

composer require --dev phpstan/phpstan
来源：http://hz.hnqzz.top/gtrflznyxv.html

[U80] PHP：代码规范修复
来源：http://hz.xingfuxueyuan.xyz/gtxdxhfvep.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hfpthk.cn/gtdkcolntm.html


<!-- 参考信息 -->