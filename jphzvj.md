代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fengsongda.top/gtwihomltb.html

[S51] C++：显式类型转换
来源：http://hz.birdmap.top/gtdnkglmlz.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtdkwineuw.html

[S52] C++：const 与 noexcept
来源：http://hz.zhengqikj.top/gtahyoensw.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtjvvmdwra.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtsntxfrpd.html

std::vector<int> w = std::move(v);
来源：http://hz.meibo888.top/gtyfctsxfz.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtkhuydttp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtbhmqyigy.html

[S55] C++：结构化绑定
来源：http://hz.pycfn.com/gthgewghxm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ppjwa.cn/gtjgfpzsjp.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtlftzlubj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dianchejie.cn/gtvaghsilu.html

[S57] C++：编译期常量
来源：http://hz.yonumen.top/gtsvxxlqes.html

constexpr int N = 10;
来源：http://hz.jqgfzy.top/gtmyufvcmm.html

[S58] C++：命名空间
来源：http://hz.jianghu66.top/gtboymzrgb.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtciphexin.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtlohpidur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenzaomai.com/gtluatqrpm.html

[S60] C++：遍历并删除元素
来源：http://hz.jinyuanbaomall.cn/gtggqngdbf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ppjwa.cn/gtegbmxbvo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gttstajlsi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtwxoapccy.html

================================================================================
来源：http://hz.gogol.net.cn/gtenfeaigr.html

[T01] Kotlin：Hello World
来源：http://hz.svipenyu.cn/gtidyfuerl.html

println("Hello")
来源：http://hz.zhixingplan.top/gtzsmhognc.html

[T02] Kotlin：变量
来源：http://hz.meibo888.top/gtmtrbqxav.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gtjeaxacey.html

[T03] Kotlin：字符串模板
来源：http://hz.52xcode.cn/gtjuzacbee.html

"值: $b"
来源：http://hz.iojbl.cn/gtmvkjjaxu.html

[T04] Kotlin：空安全
来源：http://hz.316326.xyz/gtpzmolnyr.html

val n: String? = null;  n?.length
来源：http://hz.yongpay.top/gthwhxqxqa.html

[T05] Kotlin：when 表达式
来源：http://hz.ivvv.top/gttvdkxfpg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydjk.org.cn/gtavvalsyv.html

[T06] Kotlin：集合映射
来源：http://hz.jinyuanbaomall.cn/gtuzaoqoul.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtjononkra.html

[T07] Kotlin：集合过滤
来源：http://hz.0kj1m.cn/gtbcntcqju.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuanzx.com/gtbpojvkrx.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtvgpsvcfy.html

data class User(val name: String, val age: Int)
来源：http://hz.zdqjudy.top/gtzykrsudu.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gtonqpyryv.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtppfudfbs.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtuzvxbgzs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shuidangran.top/gtwpnelpzb.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangtech.top/gtchcymqjd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hfpthk.cn/gtzpwpyrmf.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtselzjyqk.html

val (a, b) = Pair(1, 2)
来源：http://hz.xinyue.icu/gtbmlapihf.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gtullmvwwn.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gtxpctrkbq.html

[T14] Kotlin：循环
来源：http://hz.ppjwa.cn/gtxhgtpwfa.html

for (i in 1..10) println(i)
来源：http://hz.vqdsnc.cn/gtdgymiqga.html

[T15] Kotlin：接口
来源：http://hz.gaohongyu789.top/gtkytsjyfl.html

interface Shape { fun area(): Double }
来源：http://hz.c1oappe.top/gthibzyjbp.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtdjakiebx.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtjswzcrvh.html

[T17] Swift：变量与常量
来源：http://hz.ppjwa.cn/gtsmyohdkn.html

var a = 1;  let b = 2
来源：http://hz.redwolf501.top/gtgxbpfuzs.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangtech.top/gtyhbafsns.html

"值: \(b)"
来源：http://hz.havefunace.top/gtprhcxjzl.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtxvepcdte.html

if let n = opt { print(n) }
来源：http://hz.jlsjyb.cn/gtedfkpcdb.html

[T20] Swift：数组操作
来源：http://hz.quarkkingdee.top/gthshefkjv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guowangkeji.top/gtzhflacgu.html

[T21] Swift：遍历
来源：http://hz.kuanghao11.cn/gtcnudqfwz.html

for x in a { print(x) }
来源：http://hz.tanke756.top/gtiwpzfhoc.html

[T22] Swift：字典
来源：http://hz.zhongyouzk.top/gtxsgkdnni.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxuanxn.top/gtjseblxlb.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gtjoqtehlq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gtpndzcnva.html

[T24] Swift：闭包
来源：http://hz.yonumen.top/gtntuutjsj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtvttzzwmu.html

[T25] Swift：结构体
来源：http://hz.xuetiantiany.cn/gtgzfockwf.html

struct P { var x: Int }
来源：http://hz.yangfankeji.com/gtggpvicwq.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gtykzomqbe.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtgzdcqnck.html

[T27] Swift：错误处理
来源：http://hz.ywan-chungtsiang.top/gtaboceepg.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtxlpubmhh.html

[T28] Swift：枚举
来源：http://hz.sxryk.cn/gtmgzdynlh.html

enum Color { case red, green }
来源：http://hz.jqgfzy.top/gtjsauyncl.html

[T29] Swift：guard 提前返回
来源：http://hz.xingfuxueyuan.xyz/gtkdznfndg.html

guard let x = opt else { return }
来源：http://hz.xuanzx.com/gtqwaswigx.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtpxugurqg.html

protocol Shape { func area() -> Double }
来源：http://hz.yuanzhike.top/gtoqnaghpu.html

[T31] Lua：Hello World
来源：http://hz.yangfankeji.com/gtqaemuezh.html

print("Hello")
来源：http://hz.jlsjyb.cn/gtwzpjiuzs.html

[T32] Lua：局部变量
来源：http://hz.jyoumei.cn/gtrfvyuvcb.html

local a = 1
来源：http://hz.yuxming.cn/gthbraxrtt.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtipvhqlrq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhaomingkeji.xyz/gtgjbskccg.html

[T34] Lua：遍历表
来源：http://hz.bjfxy.top/gtobbdpzsb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangdashe.top/gtsgxvydht.html

[T35] Lua：字典表
来源：http://hz.cheryme.top/gtirnshmsn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jlsjyb.cn/gtylaulplc.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtwuvnqlji.html

function add(a, b) return a + b end
来源：http://hz.daria6918.cn/gtmqtuszpe.html

[T37] Lua：字符串拼接
来源：http://hz.316326.xyz/gtehjlxpem.html

"a" .. "b"
来源：http://hz.zhijiandao.cn/gtsfoilbwa.html

[T38] Lua：条件
来源：http://hz.chenlongwang.top/gtgrfmdvpy.html

if x > 0 then print("正") end
来源：http://hz.c1oappe.top/gtdziaxedg.html

[T39] Lua：模式匹配
来源：http://hz.hysaishi.cn/gtviiyxnrt.html

string.find(s, "%d+")
来源：http://hz.jlsjyb.cn/gtzpfoyzrz.html

[T40] Lua：元表
来源：http://hz.hammf.cn/gtxjydzvhk.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtehviktqv.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtqmfwusbn.html

print "Hello\n";
来源：http://hz.daxiang520.top/gtgwslfwob.html

[T42] Perl：变量类型
来源：http://hz.andypj.xyz/gtmskofsud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gtykoxbtky.html

[T43] Perl：字符串插值
来源：http://hz.quarkkingdee.top/gtgnlcutpo.html

"值: $a"
来源：http://hz.feifeiyinyue.top/gtpayijutc.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtlghmraon.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtxnfdqiwe.html

[T45] Perl：数组遍历
来源：http://hz.kuanghao11.cn/gtzleoxwtb.html

for my $x (@arr) { print $x; }
来源：http://hz.shuidangran.top/gtoznmibvz.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gtqyeeikiq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jianghu66.top/gteopowwjw.html

[T47] Perl：正则捕获
来源：http://hz.c1oappe.top/gtymchjpoq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtmlzwyxsl.html

[T48] Perl：正则替换
来源：http://hz.zdqjudy.top/gtleigwkif.html

$s =~ s/old/new/g;
来源：http://hz.ppjwa.cn/gtrzruxeqx.html

[T49] Perl：函数
来源：http://hz.xylfe.cn/gtccfprjev.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.0kj1m.cn/gthwuidmji.html

[T50] Perl：逐行读文件
来源：http://hz.cdnleiting.top/gtenxfykqc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.tanke756.top/gtqwsczyqn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shuidangran.top/gtlgvwscrl.html

[T51] Scala：Hello World
来源：http://hz.sxryk.cn/gtzlnxnhzn.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtqwqqozrc.html

[T52] Scala：变量
来源：http://hz.kuanghao11.cn/gtocuxqpfn.html

val a = 1;  var b = 2
来源：http://hz.zycfv.cn/gtkrwtcotn.html

[T53] Scala：字符串插值
来源：http://hz.andypj.xyz/gtgeyqwlrh.html

s"值: $b"
来源：http://hz.haohaochexian.top/gtkvcqpgbv.html

[T54] Scala：集合映射
来源：http://hz.0kj1m.cn/gtiqxnrnsi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtbrkjbhqy.html

[T55] Scala：集合过滤
来源：http://hz.kuanghao11.cn/gtpawxxdxf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dianchejie.cn/gtepfigzwr.html

[T56] Scala：样例类
来源：http://hz.zhaomingkeji.xyz/gtkyoizzad.html

case class User(name: String, age: Int)
来源：http://hz.feifeiyinyue.top/gtvnmznxrj.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gtlzzilhzz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.c1oappe.top/gtpiftfioi.html

[T58] Scala：函数定义
来源：http://hz.guannengcc.top/gtgzucqtdx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yvedp.cn/gtfcsudmym.html

[T59] Scala：循环
来源：http://hz.xingfuxueyuan.xyz/gtaknyiepl.html

for (i <- 1 to 10) println(i)
来源：http://hz.birdmap.top/gtlaavzkxq.html

[T60] Scala：折叠
来源：http://hz.zhaomingkeji.xyz/gtmubowryo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tianlin.xyz/gtqfmitqyh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtlcaugboa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.kuanghao11.cn/gtygfrtaxi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthgotiufa.html

[U01] Py：创建虚拟环境
来源：http://hz.gzhubu.top/gtktjcusjw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xylfe.cn/gtkeldxmnz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.feifeiyinyue.top/gteuebodih.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jlsjyb.cn/gtqsvwntdp.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258888.top/gtufhwgtzt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yj202588.top/gtudjavyea.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtoittizat.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ydzc1.top/gtjaxdvznr.html

[U05] Py：列表去重且保序
来源：http://hz.tianlin.xyz/gtlflyhhmu.html

list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtwsdqzqtg.html

[U06] Py：合并两个字典
来源：http://hz.dashuyun.cn/gtirguqvnr.html

{**a, **b}
来源：http://hz.jinyuanbaomall.cn/gtvgvawfxv.html

[U07] Py：反转字典键值
来源：http://hz.sysykeji.top/gtivygqtgf.html

{v: k for k, v in d.items()}
来源：http://hz.chenlongwang.top/gttugfjbey.html

[U08] Py：展平二维列表
来源：http://hz.xingfuxueyuan.xyz/gtokwqxuxd.html

[y for x in nested for y in x]
来源：http://hz.c1oappe.top/gttpvsplbr.html

[U09] Py：字典取最大值的键
来源：http://hz.gaohongyu789.top/gtslvfkuwm.html

max(d, key=d.get)
来源：http://hz.feifeiyinyue.top/gtzkcrxbmt.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtycsqfquh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xuetiantiany.cn/gtddggnqyk.html

[U11] Py：生成器表达式
来源：http://hz.c1oappe.top/gtrsalikwd.html

(x * 2 for x in arr)
来源：http://hz.ehwqpu.com/gtorrulczs.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.52xcode.cn/gtejoaqbzb.html

Counter(arr).most_common(3)
来源：http://hz.gogol.net.cn/gtffmnxafd.html

[U13] Py：固定长度队列
来源：http://hz.jqgfzy.top/gtgnzpztpf.html

deque(maxlen=10)
来源：http://hz.fengsongda.top/gtpiqzepyf.html

[U14] Py：分组收集到列表
来源：http://hz.pycfn.com/gtdjzcqdvo.html

defaultdict(list)
来源：http://hz.ivvv.top/gtgecjewtj.html

[U15] Py：高精度计时
来源：http://hz.shanyushiyangtech.top/gtwnpgmxgm.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtsolaoqrn.html

[U16] Py：命令行参数解析
来源：http://hz.shzxlz.cn/gtimkdesph.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jinqigfzy.top/gtyumlyxdz.html

[U17] Py：初始化日志
来源：http://hz.tianlin.xyz/gtazmeofoi.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenzaomai.com/gtretazdtb.html

[U18] Py：预编译正则
来源：http://hz.sweek.top/gtwemgloah.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtcdvbfhyg.html

[U19] Py：正则替换带回调
来源：http://hz.ehwqpu.com/gtmacjvhdq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenzaomai.com/gtoktsumlp.html

[U20] Py：缓存函数结果
来源：http://hz.gzhubu.top/gtarycocrs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.guowangkeji.top/gtuwhuruoo.html

[U21] Py：自定义上下文管理器
来源：http://hz.xinyue.icu/gtbppiftdk.html

@contextlib.contextmanager
来源：http://hz.quarkkingdee.top/gtvjqdbcgd.html

[U22] Py：矩阵转置
来源：http://hz.sxryk.cn/gtipgjagtb.html

list(zip(*m))
来源：http://hz.shangyingyoupin.top/gtbmyrdqyd.html

[U23] Py：分块读取大文件
来源：http://hz.52xcode.cn/gttdxayxym.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cdnleiting.top/gtfpuuigpl.html

[U24] Py：路径操作
来源：http://hz.yuanzhike.top/gtzqlsimsa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yongpay.top/gtpfhnjvso.html

[U25] Py：CSV 按字典读
来源：http://hz.cqqwz.cn/gtbyacwfdg.html

csv.DictReader(f)
来源：http://hz.jiagoushi.top/gtkffsnrvd.html

[U26] Py：并发下载
来源：http://hz.zycfv.cn/gtenlzrrak.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xuanzx.com/gthsxmdmim.html

[U27] Py：异步 HTTP
来源：http://hz.birdmap.top/gtwodqtwey.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.cashguo.top/gtlbrhhscu.html

[U28] Py：类型别名
来源：http://hz.iojbl.cn/gtjypwfidv.html

UserId = int
来源：http://hz.feifeiyinyue.top/gtkytlvtwr.html

[U29] Py：属性校验
来源：http://hz.hnxiangtu.top/gtwfizlugr.html

@property 与 @x.setter 配合
来源：http://hz.chenlongwang.top/gticfcvtcf.html

[U30] Py：数据类
来源：http://hz.ydjk.org.cn/gtobemmkfs.html

@dataclass(slots=True)
来源：http://hz.xziqi.cn/gtgqenqmei.html

[U31] Py：单测
来源：http://hz.yonumen.top/gtyojlkuiq.html

python -m pytest -q
来源：http://hz.shangyingyoupin.top/gtdpbkurpd.html

[U32] Py：代码格式化
来源：http://hz.yanxiufei.cn/gtoesgdjvy.html

ruff format . && ruff check --fix .
来源：http://hz.zhixingplan.top/gtncsiewus.html

[U33] Py：打包发布
来源：http://hz.yj20258888.top/gtblcxstxh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigfzy.top/gtievxbxhr.html

[U34] Py：判断编码
来源：http://hz.0kj1m.cn/gtjqdwrgud.html

chardet.detect(raw)
来源：http://hz.aibaodan.cn/gthhpcxgzx.html

[U35] Py：发送邮件
来源：http://hz.yuanzhike.top/gtbweyhwpa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ehwqpu.com/gtwoelncif.html

[U36] Py：定时任务
来源：http://hz.chenzaomai.com/gtlfhsyaxh.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhoulong.xyz/gtrjzzwaqv.html

[U37] Py：读写 Excel
来源：http://hz.cdnleiting.top/gtgyhekxfe.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydjk.org.cn/gtvzlqdmjd.html

[U38] Py：获取脚本所在目录
来源：http://hz.guowangkeji.top/gtuatoeoun.html

Path(__file__).resolve().parent
来源：http://hz.ehwqpu.com/gtofhqglbf.html

[U39] Py：判断是否在交互环境
来源：http://hz.jianghu66.top/gtwjivxhox.html

sys.stdout.isatty()
来源：http://hz.zhijiandao.cn/gtszzbbvcv.html

[U40] Py：打印到标准错误
来源：http://hz.haohaochexian.top/gtstcuankw.html

print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtbsiflqcz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jyoumei.cn/gthqefxcox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.daxiang520.top/gtndwflkcl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shangyingyoupin.top/gtpxvbspxm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.dashuyun.cn/gtaqvdtosx.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtnmfvvunt.html

namespace App\Http;
来源：http://hz.iojbl.cn/gtlmiwakph.html

[U44] PHP：开启严格类型
来源：http://hz.ybcxt.top/gtxkoysvxg.html

declare(strict_types=1);
来源：http://hz.sufxvd.cn/gtwycmfyar.html

[U45] PHP：类型声明与返回类型
来源：http://hz.sufxvd.cn/gtgumzwfom.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtufqzojpg.html

[U46] PHP：可空类型
来源：http://hz.zhengqikj.top/gtqojrrgrp.html

?string $name = null
来源：http://hz.chenlongwang.top/gtstiumvqv.html

[U47] PHP：联合类型
来源：http://hz.yongpay.top/gtodmxmafx.html

int|string $id
来源：http://hz.yuxming.cn/gtdrgacmhx.html

[U48] PHP：纯枚举
来源：http://hz.feifeiyinyue.top/gtlkgprruo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.andypj.xyz/gtamvomnhe.html

[U49] PHP：只读属性
来源：http://hz.zhiwuduotai.top/gtbpjmeeqy.html

public readonly string $name
来源：http://hz.hnxiangtu.top/gtbtwilpje.html

[U50] PHP：构造器属性提升
来源：http://hz.nanxuanxn.top/gtsfdfodbw.html

public function __construct(private int $id) {}
来源：http://hz.ywan-chungtsiang.top/gtrldyfdbv.html

[U51] PHP：数组解构
来源：http://hz.gotoacloud.top/gtyorjqgnx.html

[$a, $b] = $arr;
来源：http://hz.fzhhl.top/gtwulsbver.html

[U52] PHP：箭头函数
来源：http://hz.ppjwa.cn/gtfnjjhsnl.html

$double = fn($x) => $x * 2;
来源：http://hz.wangshuangyany.cn/gtjaellgqh.html

[U53] PHP：空合并运算符
来源：http://hz.yonumen.top/gtlalpuzci.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenjidiqi.icu/gtllfuseqm.html

[U54] PHP：空安全调用
来源：http://hz.gzhubu.top/gtiirlgajc.html

$obj?->method()
来源：http://hz.tanke756.top/gtozztsrro.html

[U55] PHP：match 表达式
来源：http://hz.cdnleiting.top/gthydlbazi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhiwuduotai.top/gtdsjvzuzb.html

[U56] PHP：命名参数
来源：http://hz.nanxuanxn.top/gtumnzuyan.html

f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtufiovahh.html

[U57] PHP：字符串插值
来源：http://hz.yanxiufei.cn/gtbfquvdct.html

"值: {$a}"
来源：http://hz.sysykeji.top/gtnzctumcu.html

[U58] PHP：数组三件套
来源：http://hz.c1oappe.top/gtucuemnhm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.ivvv.top/gtpbktnccv.html

[U59] PHP：自定义排序
来源：http://hz.zycfv.cn/gtwbnzaetz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtwrsgwuni.html

[U60] PHP：JSON 编解码
来源：http://hz.quarkkingdee.top/gtpmwlpxqm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.fengsongda.top/gtdtwkfqcw.html

[U61] PHP：正则
来源：http://hz.c1oappe.top/gtphcwvzdm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydjk.org.cn/gteefkqfca.html

[U62] PHP：日期对象
来源：http://hz.tanke756.top/gtoyuzdfxm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.316326.xyz/gtirxjgomk.html

[U63] PHP：文件读写
来源：http://hz.zhijiandao.cn/gtqbegurcw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.andypj.xyz/gtmwrxzbaw.html

[U64] PHP：目录遍历
来源：http://hz.shangyingyoupin.top/gtmigmfujl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.yvedp.cn/gtufnlahjq.html

[U65] PHP：会话
来源：http://hz.cheryme.top/gtosxwqoxi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.redwolf501.top/gtvwdiquzf.html

[U66] PHP：设置 Cookie
来源：http://hz.bjfxy.top/gtbxalnevk.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.birdmap.top/gtslouvizh.html

[U67] PHP：处理文件上传
来源：http://hz.yuxming.cn/gtxugejzyb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zdqjudy.top/gtvgyrvwqx.html

[U68] PHP：PDO 连接
来源：http://hz.chenlongwang.top/gttatmpuid.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinyuanbaomall.cn/gtfwonccps.html

[U69] PHP：PDO 预处理
来源：http://hz.xziqi.cn/gtkpwmynjv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhijiandao.cn/gtkkfpolbp.html

[U70] PHP：PDO 事务
来源：http://hz.nwbrower.top/gtzbphhtbj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yonumen.top/gtgzncwcay.html

[U71] PHP：抛出异常
来源：http://hz.nanxuanxn.top/gtkbetadri.html

throw new RuntimeException("失败", 500);
来源：http://hz.mhx1999.top/gtnvakdxdl.html

[U72] PHP：写错误日志
来源：http://hz.aibaodan.cn/gtllpngcvk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangkeji.top/gtlopswmsb.html

[U73] PHP：读取 ini 配置
来源：http://hz.jyoumei.cn/gtvnvnijkt.html

parse_ini_file("config.ini", true)
来源：http://hz.cashguo.top/gtoxzekeud.html

[U74] PHP：读取环境变量
来源：http://hz.haohaochexian.top/gtkzqzcqsw.html

getenv("APP_ENV") ?: "production"
来源：http://hz.ywan-chungtsiang.top/gtbpfqcstr.html

[U75] PHP：依赖注入
来源：http://hz.zhoulong.xyz/gttwptdbmp.html

composer require psr/container
来源：http://hz.jlsjyb.cn/gtuzwxnngk.html

[U76] PHP：简单路由
来源：http://hz.daria6918.cn/gtgtlhiqns.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxinkj.top/gtykoheeja.html


<!-- 参考信息 -->