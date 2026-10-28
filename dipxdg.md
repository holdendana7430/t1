代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.chenjidiqi.icu/gtntprqjil.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtyqurypxr.html

std::vector<int> w = std::move(v);
来源：http://hz.yj202588.top/gtigfvfclw.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtjnfkjaup.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnxiangtu.top/gtuzyzimgu.html

[S55] C++：结构化绑定
来源：http://hz.yueranfly.top/gttlahvdws.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtrtevnqcj.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtsatxlhrt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yongpay.top/gtaqpqsjqa.html

[S57] C++：编译期常量
来源：http://hz.hammf.cn/gtluqpogeo.html

constexpr int N = 10;
来源：http://hz.zhongyouzk.top/gtrpryenun.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gturdyofdz.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnxiangtu.top/gtekhehhla.html

[S59] C++：静态断言
来源：http://hz.ppjwa.cn/gtcexufyud.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtmusallan.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtqvwihyrm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.aibaodan.cn/gtafnkcjsl.html

================================================================================
来源：http://hz.bjfxy.top/gtkmpliflj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hywenlv.cn/gtopozezwu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxdrqnnxb.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gttxdewjul.html

println("Hello")
来源：http://hz.jiagoushi.top/gtdlzunzei.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtknbkwufy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnqzz.top/gtnihoieif.html

[T03] Kotlin：字符串模板
来源：http://hz.gaohongyu789.top/gtlyyfzycu.html

"值: $b"
来源：http://hz.cheryme.top/gtovqjtore.html

[T04] Kotlin：空安全
来源：http://hz.kuanghao11.cn/gtdiaobcvg.html

val n: String? = null;  n?.length
来源：http://hz.chenzaomai.com/gtbxhnspes.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgfzy.top/gtgfsjgyjk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hammf.cn/gtjzjjmlzk.html

[T06] Kotlin：集合映射
来源：http://hz.cqqwz.cn/gtbqtcwvcz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.snrcjt.cn/gtzikdknph.html

[T07] Kotlin：集合过滤
来源：http://hz.jinghuilouyu.cn/gthtuwhavw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.quarkkingdee.top/gtigdwxewe.html

[T08] Kotlin：数据类
来源：http://hz.jyoumei.cn/gtvjjcxlvd.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtnwxihazp.html

[T09] Kotlin：扩展函数
来源：http://hz.chenzaomai.com/gtwekdgaui.html

fun String.exclaim() = this + "!"
来源：http://hz.pycfn.com/gtnkqytpmd.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtlyywbfvj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ydjk.org.cn/gtpmdsmjma.html

[T11] Kotlin：协程
来源：http://hz.shzxlz.cn/gtbriyvoeg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gtqqrvcvfs.html

[T12] Kotlin：解构声明
来源：http://hz.cdnleiting.top/gtztxrdebu.html

val (a, b) = Pair(1, 2)
来源：http://hz.pycfn.com/gtzxdndtsy.html

[T13] Kotlin：只读 Map
来源：http://hz.cucudq.cn/gtsuptzrdq.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtiojebzwi.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtysjxvkgd.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtjrnysuam.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtynecjbzu.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtomfviekd.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtesmttlrt.html

print("Hello")
来源：http://hz.yueranfly.top/gtpxkqgrtj.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gtwdvstgpe.html

var a = 1;  let b = 2
来源：http://hz.tian-w.cn/gtkwhjcwti.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtwngygqgs.html

"值: \(b)"
来源：http://hz.hammf.cn/gtdumrqopy.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtknhnujhe.html

if let n = opt { print(n) }
来源：http://hz.nwbrower.top/gteyijamlv.html

[T20] Swift：数组操作
来源：http://hz.yvedp.cn/gteqnkrwzp.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenzaomai.com/gtkuxntpeu.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtfgobskov.html

for x in a { print(x) }
来源：http://hz.yuanzhike.top/gtfyiuijcr.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gthnexyine.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.birdmap.top/gtfylkrayd.html

[T23] Swift：函数
来源：http://hz.yuanzhike.top/gthwhdghwn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhoulong.xyz/gttsbvyfgd.html

[T24] Swift：闭包
来源：http://hz.gogol.net.cn/gthxkiwcnf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shzxlz.cn/gtlvgfevnk.html

[T25] Swift：结构体
来源：http://hz.yueranfly.top/gtgcavcpjn.html

struct P { var x: Int }
来源：http://hz.fengsongda.top/gtjifqghst.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gtljihjies.html

class A: Base { override func f() {} }
来源：http://hz.zhongyouzk.top/gtocgupylw.html

[T27] Swift：错误处理
来源：http://hz.zhijiandao.cn/gtkopgihfq.html

do { try f() } catch { print(error) }
来源：http://hz.xingfuxueyuan.xyz/gthgcnzwqv.html

[T28] Swift：枚举
来源：http://hz.pycfn.com/gtdesxbgfz.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gthvhniqdr.html

[T29] Swift：guard 提前返回
来源：http://hz.cdnleiting.top/gtjbjvucpg.html

guard let x = opt else { return }
来源：http://hz.yuanzhike.top/gtjfmfjosj.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtjqadwdmc.html

protocol Shape { func area() -> Double }
来源：http://hz.hywenlv.cn/gtsegfczsp.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gtgweoteqc.html

print("Hello")
来源：http://hz.gzhubu.top/gtbvwfcgja.html

[T32] Lua：局部变量
来源：http://hz.ivvv.top/gtdaudumhc.html

local a = 1
来源：http://hz.feifeiyinyue.top/gtzhlqvbzx.html

[T33] Lua：表（数组）
来源：http://hz.gzhubu.top/gtyeiscbgc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sufxvd.cn/gtfctobloc.html

[T34] Lua：遍历表
来源：http://hz.jlsjyb.cn/gtfveovvvn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.gzhubu.top/gtkeesduax.html

[T35] Lua：字典表
来源：http://hz.zhixingplan.top/gtgkeidgsb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gogol.net.cn/gtjipycytv.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtmsqowfjs.html

function add(a, b) return a + b end
来源：http://hz.ybcxt.top/gtxnkxytth.html

[T37] Lua：字符串拼接
来源：http://hz.sxryk.cn/gtbdkvsqqk.html

"a" .. "b"
来源：http://hz.zdqjudy.top/gtyryjxtkg.html

[T38] Lua：条件
来源：http://hz.hammf.cn/gtzarvvack.html

if x > 0 then print("正") end
来源：http://hz.haohaochexian.top/gtyiafhhis.html

[T39] Lua：模式匹配
来源：http://hz.sysykeji.top/gtdmqgihru.html

string.find(s, "%d+")
来源：http://hz.cheryme.top/gtznalgcri.html

[T40] Lua：元表
来源：http://hz.xylfe.cn/gtpsgpeawj.html

setmetatable({}, { __index = base })
来源：http://hz.shuidangran.top/gtuqxekvpq.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtkssnjriu.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtznaqddly.html

[T42] Perl：变量类型
来源：http://hz.zdqjudy.top/gtibkefexn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhongyouzk.top/gtfbojigle.html

[T43] Perl：字符串插值
来源：http://hz.jinqigfzy.top/gthzqtcipk.html

"值: $a"
来源：http://hz.shuidangran.top/gttczhsfnx.html

[T44] Perl：条件
来源：http://hz.jinqigufen.top/gttjwhtcgp.html

if ($a > 0) { print "正"; }
来源：http://hz.quarkkingdee.top/gtehttusvb.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gtkvxudnda.html

for my $x (@arr) { print $x; }
来源：http://hz.gzhubu.top/gtbvjavtvr.html

[T46] Perl：哈希操作
来源：http://hz.pengpengdd.cyou/gtbtkkpzii.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sufxvd.cn/gtufujxyyd.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtmfgapbtx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhixingplan.top/gtsjlxvaty.html

[T48] Perl：正则替换
来源：http://hz.xuetiantiany.cn/gtpcyelwyb.html

$s =~ s/old/new/g;
来源：http://hz.andypj.xyz/gtggsevtwr.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gtbqtpxhkk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.iojbl.cn/gtngyozzhu.html

[T50] Perl：逐行读文件
来源：http://hz.ivvv.top/gtypvjyzry.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zdqjudy.top/gtcqyovquf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shzxlz.cn/gtibapkveo.html

[T51] Scala：Hello World
来源：http://hz.pycfn.com/gtrsyxliog.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gttsbhrjgs.html

[T52] Scala：变量
来源：http://hz.zhijiandao.cn/gtiajfjfgg.html

val a = 1;  var b = 2
来源：http://hz.yj20258888.top/gtrwjgrarb.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gtdytmtmxt.html

s"值: $b"
来源：http://hz.sufxvd.cn/gtwxiifzjq.html

[T54] Scala：集合映射
来源：http://hz.hnqzz.top/gtqpzmubyw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gzhubu.top/gtswolbbbz.html

[T55] Scala：集合过滤
来源：http://hz.jlsjyb.cn/gtricmmern.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hammf.cn/gtzifymnsq.html

[T56] Scala：样例类
来源：http://hz.xinyue.icu/gtsfbawdtz.html

case class User(name: String, age: Int)
来源：http://hz.iojbl.cn/gtlyuljkdi.html

[T57] Scala：模式匹配
来源：http://hz.birdmap.top/gtbgsoqyok.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuetiantiany.cn/gtcytzjzgk.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtzwdgszbe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.andypj.xyz/gtqeoivusf.html

[T59] Scala：循环
来源：http://hz.xinyue.icu/gtppmvgovl.html

for (i <- 1 to 10) println(i)
来源：http://hz.aibaodan.cn/gtdzkpkwji.html

[T60] Scala：折叠
来源：http://hz.xziqi.cn/gtvihxdmke.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.9152youxi.cn/gtosscjgvn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcrbzndem.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.svipenyu.cn/gtiorqwdzd.html

================================================================================
来源：http://hz.meibo888.top/gtxulhpbps.html

[U01] Py：创建虚拟环境
来源：http://hz.guowangkeji.top/gthgcfbldc.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sysykeji.top/gttgjlbhqq.html

[U02] Py：导出 / 安装依赖
来源：http://hz.tian-w.cn/gtkrbmzrwv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.dashuyun.cn/gtwdpsjhco.html

[U03] Py：加载 .env 配置
来源：http://hz.jinyuanbaomall.cn/gtxfuuqqom.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xziqi.cn/gtzjwmctcm.html

[U04] Py：变量调试打印
来源：http://hz.hysaishi.cn/gtsswyicvh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.andypj.xyz/gtryjvuhoq.html

[U05] Py：列表去重且保序
来源：http://hz.jinghuilouyu.cn/gtffefypgj.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtjsgrjefy.html

[U06] Py：合并两个字典
来源：http://hz.jqgufenzy.top/gtomyarspm.html

{**a, **b}
来源：http://hz.tian-w.cn/gtupchdsaf.html

[U07] Py：反转字典键值
来源：http://hz.snrcjt.cn/gttmpxdihe.html

{v: k for k, v in d.items()}
来源：http://hz.cucudq.cn/gtxfyomnqx.html

[U08] Py：展平二维列表
来源：http://hz.kuanghao11.cn/gtokxvldcx.html

[y for x in nested for y in x]
来源：http://hz.zdqjudy.top/gtpsizultm.html

[U09] Py：字典取最大值的键
来源：http://hz.daria6918.cn/gtdpbryhge.html

max(d, key=d.get)
来源：http://hz.gzhubu.top/gtkkymxonl.html

[U10] Py：按值排序字典
来源：http://hz.cashguo.top/gtrthxrfhk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.bjfxy.top/gthvgtnjbt.html

[U11] Py：生成器表达式
来源：http://hz.zdqjudy.top/gtjniapfjy.html

(x * 2 for x in arr)
来源：http://hz.haohaochexian.top/gtkpabcxuw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hammf.cn/gtgylkiqys.html

Counter(arr).most_common(3)
来源：http://hz.fzhhl.top/gtpsmctrow.html

[U13] Py：固定长度队列
来源：http://hz.birdmap.top/gtqvsktveq.html

deque(maxlen=10)
来源：http://hz.xuanzx.com/gtvcloczgk.html

[U14] Py：分组收集到列表
来源：http://hz.52xcode.cn/gtccixoppu.html

defaultdict(list)
来源：http://hz.zdqjudy.top/gtlcwjxmxe.html

[U15] Py：高精度计时
来源：http://hz.52xcode.cn/gttulmfhsu.html

t = time.perf_counter()
来源：http://hz.zhoulong.xyz/gtlrsbsjeq.html

[U16] Py：命令行参数解析
来源：http://hz.yanxiufei.cn/gteypgqdes.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xingfuxueyuan.xyz/gtyaitpnku.html

[U17] Py：初始化日志
来源：http://hz.zycfv.cn/gtssfrwqmj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258.top/gtkdvdatfo.html

[U18] Py：预编译正则
来源：http://hz.gaohongyu789.top/gtncahjkik.html

pat = re.compile(r"\d+")
来源：http://hz.zhengqikj.top/gtvpjyyvis.html

[U19] Py：正则替换带回调
来源：http://hz.dianchejie.cn/gtpzfehsaw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxuanxn.top/gtehnfzaao.html

[U20] Py：缓存函数结果
来源：http://hz.xuetiantiany.cn/gtbdpfnkzd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gogol.net.cn/gtrvjtyupj.html

[U21] Py：自定义上下文管理器
来源：http://hz.hnxiangtu.top/gtoxppxpzk.html

@contextlib.contextmanager
来源：http://hz.ydjk.org.cn/gtxvfxnazy.html

[U22] Py：矩阵转置
来源：http://hz.jinqigufen.top/gtdhtpffkc.html

list(zip(*m))
来源：http://hz.cheryme.top/gtxktwdxaw.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtlncbvldd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fzhhl.top/gttxvybuao.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtdrbchnmi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jlsjyb.cn/gtkpliuvxj.html

[U25] Py：CSV 按字典读
来源：http://hz.shangyingyoupin.top/gttdpmxrql.html

csv.DictReader(f)
来源：http://hz.tanke756.top/gtgpvnmden.html

[U26] Py：并发下载
来源：http://hz.hnqzz.top/gtojvmmrrg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.tianlin.xyz/gtcbdstjbn.html

[U27] Py：异步 HTTP
来源：http://hz.jianghu66.top/gtrparhrhx.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shuidangran.top/gthqaijnbq.html

[U28] Py：类型别名
来源：http://hz.jyoumei.cn/gtdeaipmfi.html

UserId = int
来源：http://hz.yonumen.top/gtzevedbhy.html

[U29] Py：属性校验
来源：http://hz.smart0.xyz/gtilxxmedj.html

@property 与 @x.setter 配合
来源：http://hz.sxryk.cn/gtoplbithr.html

[U30] Py：数据类
来源：http://hz.52xcode.cn/gtliqjwctx.html

@dataclass(slots=True)
来源：http://hz.hnqzz.top/gtxxyeswgh.html

[U31] Py：单测
来源：http://hz.xuetiantiany.cn/gtkfdxxuci.html

python -m pytest -q
来源：http://hz.gzhubu.top/gtuxlkkjom.html

[U32] Py：代码格式化
来源：http://hz.sweek.top/gtmqpndpdz.html

ruff format . && ruff check --fix .
来源：http://hz.gotoacloud.top/gtmspdqejh.html

[U33] Py：打包发布
来源：http://hz.jinqigufen.top/gtcbtrykwl.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shzxlz.cn/gtvvurafhi.html

[U34] Py：判断编码
来源：http://hz.gaohongyu789.top/gtaqyqbeyc.html

chardet.detect(raw)
来源：http://hz.hfpthk.cn/gtvkbornsk.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangkeji.top/gtyvggxpua.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ppjwa.cn/gtfbwyyeeh.html

[U36] Py：定时任务
来源：http://hz.sufxvd.cn/gtjipvhqsq.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhixingplan.top/gtcadevqdl.html

[U37] Py：读写 Excel
来源：http://hz.xziqi.cn/gtfhhpgfro.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shanyushiyangtech.top/gtmhbnilvj.html

[U38] Py：获取脚本所在目录
来源：http://hz.fzhhl.top/gtzxkyuwdd.html

Path(__file__).resolve().parent
来源：http://hz.jinqigufen.top/gtbjppcfgx.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhoulong.xyz/gtmogvoqme.html

sys.stdout.isatty()
来源：http://hz.zhixingplan.top/gtvubcqtdm.html

[U40] Py：打印到标准错误
来源：http://hz.svipenyu.cn/gtyzclpeyw.html

print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtnecsraxf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj20258.top/gthpqhavrd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sufxvd.cn/gttcovfowk.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yvedp.cn/gtxsyxwtyx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.redwolf501.top/gtelyeagwk.html

[U43] PHP：声明命名空间
来源：http://hz.jqgfzy.top/gtyfershrg.html

namespace App\Http;
来源：http://hz.cucudq.cn/gtynbfnuaf.html

[U44] PHP：开启严格类型
来源：http://hz.fzhhl.top/gtnxncfefa.html

declare(strict_types=1);
来源：http://hz.zdqjudy.top/gtdenqebap.html

[U45] PHP：类型声明与返回类型
来源：http://hz.pengpengdd.cyou/gtgcyawcjj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gthkvhnwmu.html

[U46] PHP：可空类型
来源：http://hz.dianchejie.cn/gtpafpwdww.html

?string $name = null
来源：http://hz.zycfv.cn/gtoijngafk.html

[U47] PHP：联合类型
来源：http://hz.feifeiyinyue.top/gtivonhcmn.html

int|string $id
来源：http://hz.cashguo.top/gtwikzqipf.html

[U48] PHP：纯枚举
来源：http://hz.pycfn.com/gtjirjopze.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cdnleiting.top/gtbnecccyp.html

[U49] PHP：只读属性
来源：http://hz.havefunace.top/gterimozat.html

public readonly string $name
来源：http://hz.xinyue.icu/gtqjqrrnyp.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258888.top/gtzkkurcmd.html

public function __construct(private int $id) {}
来源：http://hz.wangdashe.top/gttqxsjsti.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtfbmxivku.html

[$a, $b] = $arr;
来源：http://hz.gotoacloud.top/gtojzopobs.html

[U52] PHP：箭头函数
来源：http://hz.xinyue.icu/gtodklevvs.html

$double = fn($x) => $x * 2;
来源：http://hz.ydjk.org.cn/gteskeefpm.html

[U53] PHP：空合并运算符
来源：http://hz.ehwqpu.com/gtvsayfirp.html

$v = $a ?? $b ?? "default";
来源：http://hz.aibaodan.cn/gtdyylxojb.html

[U54] PHP：空安全调用
来源：http://hz.chenzaomai.com/gtsjnwqzbu.html

$obj?->method()
来源：http://hz.jinqigufen.top/gttabkhqui.html

[U55] PHP：match 表达式
来源：http://hz.quarkkingdee.top/gtewufvkjj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gaohongyu789.top/gtxsogvsho.html

[U56] PHP：命名参数
来源：http://hz.aizwys.cn/gtxavwcqli.html

f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtzufgbpqe.html

[U57] PHP：字符串插值
来源：http://hz.chenzaomai.com/gtqrdxxaym.html

"值: {$a}"
来源：http://hz.guowangkeji.top/gtqyuwvufa.html

[U58] PHP：数组三件套
来源：http://hz.feifeiyinyue.top/gtuvxduqas.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.quarkkingdee.top/gtphemfoky.html

[U59] PHP：自定义排序
来源：http://hz.xingfuxueyuan.xyz/gtkykgqxth.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtllxyyxti.html

[U60] PHP：JSON 编解码
来源：http://hz.smart0.xyz/gtoynwnply.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gogol.net.cn/gtqwzguwnz.html

[U61] PHP：正则
来源：http://hz.0kj1m.cn/gtodfkygsg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtwonamokd.html

[U62] PHP：日期对象
来源：http://hz.cdnleiting.top/gtkxccrmqn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shzxlz.cn/gtfjfqtehk.html

[U63] PHP：文件读写
来源：http://hz.snrcjt.cn/gtrrnvfzxc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gaohongyu789.top/gtvqajlvaz.html

[U64] PHP：目录遍历
来源：http://hz.0kj1m.cn/gtudjydqdt.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.gogol.net.cn/gtbhknvuzi.html

[U65] PHP：会话
来源：http://hz.jianghu66.top/gtiyxzzata.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guowangkeji.top/gtrngicbqw.html

[U66] PHP：设置 Cookie
来源：http://hz.hywenlv.cn/gttstctlvg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fzhhl.top/gtmnkjeqmr.html

[U67] PHP：处理文件上传
来源：http://hz.sxryk.cn/gtuaqisrta.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shangyingyoupin.top/gtiwfybslx.html

[U68] PHP：PDO 连接
来源：http://hz.sufxvd.cn/gtocquarap.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sysykeji.top/gtbaxvygof.html

[U69] PHP：PDO 预处理
来源：http://hz.zycfv.cn/gtflabsaia.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.smart0.xyz/gtuflofmxr.html

[U70] PHP：PDO 事务
来源：http://hz.fzhhl.top/gtimgiwhoh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhongyouzk.top/gtigkwpjzt.html

[U71] PHP：抛出异常
来源：http://hz.jinqigufen.top/gtclohsxoh.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtwyqwpcyx.html

[U72] PHP：写错误日志
来源：http://hz.gotoacloud.top/gtxtutzgmg.html

error_log("失败: " . $e->getMessage());
来源：http://hz.tianlin.xyz/gtmlqcmpxe.html

[U73] PHP：读取 ini 配置
来源：http://hz.yuxming.cn/gtccwcntzf.html

parse_ini_file("config.ini", true)
来源：http://hz.wangshuangyany.cn/gtldzigtfp.html

[U74] PHP：读取环境变量
来源：http://hz.guannengcc.top/gtxkmrhlku.html

getenv("APP_ENV") ?: "production"
来源：http://hz.9152youxi.cn/gtunbrdqeu.html

[U75] PHP：依赖注入
来源：http://hz.meibo888.top/gtgcyczaap.html

composer require psr/container
来源：http://hz.chenjidiqi.icu/gtezkryitx.html

[U76] PHP：简单路由
来源：http://hz.jianghu66.top/gtnwfhlobf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.smart0.xyz/gtbvekaamo.html

[U77] PHP：模板渲染
来源：http://hz.zhiwuduotai.top/gtalbqvsry.html

composer require twig/twig
来源：http://hz.gzhubu.top/gtjyoosdho.html

[U78] PHP：单元测试
来源：http://hz.wangdashe.top/gtchxobsej.html

composer require --dev phpunit/phpunit
来源：http://hz.havefunace.top/gtdnndipzq.html


<!-- 参考信息 -->