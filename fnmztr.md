代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.zhiwuduotai.top/gtgpizahgf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtyolrtmvz.html

[S48] C++：逐行读文件
来源：http://hz.daxiang520.top/gtwhfqxiiw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cashguo.top/gthaffuoxv.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtmszrnvjx.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtqbpgxqaa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangkeji.top/gtgifgonzs.html

[S50] C++：格式化数字
来源：http://hz.wangdashe.top/gtiicdecjq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhoulong.xyz/gtsulyngrd.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtpoecttoj.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtlrfacatq.html

[S52] C++：const 与 noexcept
来源：http://hz.chenjidiqi.icu/gtxzpyinki.html

int size() const noexcept { return n_; }
来源：http://hz.vqdsnc.cn/gtvrnydzsi.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gtrtrbjgpw.html

std::vector<int> w = std::move(v);
来源：http://hz.hysaishi.cn/gtpximyili.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gthxuykpnt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtxtespyto.html

[S55] C++：结构化绑定
来源：http://hz.quarkkingdee.top/gtrgyjfvpm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cashguo.top/gtakrzcrkd.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtocyrkygc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ivvv.top/gtkepvenvg.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtwpuslwff.html

constexpr int N = 10;
来源：http://hz.ywan-chungtsiang.top/gtoqxklfqw.html

[S58] C++：命名空间
来源：http://hz.quarkkingdee.top/gtfeoikeap.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuanzx.com/gtxjhqessw.html

[S59] C++：静态断言
来源：http://hz.aizwys.cn/gtanmezfzy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hfpthk.cn/gtmwrrfquq.html

[S60] C++：遍历并删除元素
来源：http://hz.xziqi.cn/gtxnrtgdxn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.52xcode.cn/gtabyqjdmr.html

================================================================================
来源：http://hz.gzhubu.top/gtxggpzkxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnqzz.top/gtptljmkir.html

================================================================================
来源：http://hz.cheryme.top/gtvrffqnky.html

[T01] Kotlin：Hello World
来源：http://hz.wangdashe.top/gtaghwjwxd.html

println("Hello")
来源：http://hz.andypj.xyz/gtnftqaynt.html

[T02] Kotlin：变量
来源：http://hz.pycfn.com/gtijhiuwhq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nanxuanxn.top/gtvnfzsfak.html

[T03] Kotlin：字符串模板
来源：http://hz.hnxiangtu.top/gtdbduyhwl.html

"值: $b"
来源：http://hz.hywenlv.cn/gtxngldimj.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtjdzihjyl.html

val n: String? = null;  n?.length
来源：http://hz.tian-w.cn/gtgoooeock.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtgimwfqot.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtbicndcdb.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gtylkwmxqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigfzy.top/gtkovskfah.html

[T07] Kotlin：集合过滤
来源：http://hz.hammf.cn/gtelpynfcd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnxiangtu.top/gtvueqdrrq.html

[T08] Kotlin：数据类
来源：http://hz.daria6918.cn/gtimqtfgmr.html

data class User(val name: String, val age: Int)
来源：http://hz.ydzc1.top/gthpswsurq.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtxexvarcp.html

fun String.exclaim() = this + "!"
来源：http://hz.jianghu66.top/gtcdrmfliy.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gtrzldkfkp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pycfn.com/gtporjbrbb.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtjlkililt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cheryme.top/gtdykjsobu.html

[T12] Kotlin：解构声明
来源：http://hz.dashuyun.cn/gtgswegpmv.html

val (a, b) = Pair(1, 2)
来源：http://hz.daxiang520.top/gtzhiejgwu.html

[T13] Kotlin：只读 Map
来源：http://hz.xuanzx.com/gttcqhlzxr.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gtvtybmevu.html

[T14] Kotlin：循环
来源：http://hz.iojbl.cn/gtnrsfppdf.html

for (i in 1..10) println(i)
来源：http://hz.ehwqpu.com/gtwwvigfjl.html

[T15] Kotlin：接口
来源：http://hz.xziqi.cn/gtkgmgwlna.html

interface Shape { fun area(): Double }
来源：http://hz.aizwys.cn/gtdhdcsnbp.html

[T16] Swift：Hello World
来源：http://hz.jqgufenzy.top/gthijsuayp.html

print("Hello")
来源：http://hz.xylfe.cn/gttxnosfoh.html

[T17] Swift：变量与常量
来源：http://hz.smart0.xyz/gtguzqhzch.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtarsclmzx.html

[T18] Swift：字符串插值
来源：http://hz.feifeiyinyue.top/gtxaqpsujz.html

"值: \(b)"
来源：http://hz.hfpthk.cn/gtpharfiga.html

[T19] Swift：可选绑定
来源：http://hz.hywenlv.cn/gtbxxsyrqv.html

if let n = opt { print(n) }
来源：http://hz.jyoumei.cn/gtiwxpkupn.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtoxuwkwpc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtjxnjscgt.html

[T21] Swift：遍历
来源：http://hz.ydzc1.top/gtbxjtvdyr.html

for x in a { print(x) }
来源：http://hz.xuetiantiany.cn/gtwgyjwluk.html

[T22] Swift：字典
来源：http://hz.guowangkeji.top/gtlqcwalfg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtpyafvzqr.html

[T23] Swift：函数
来源：http://hz.sysykeji.top/gtgvfhihpx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zdqjudy.top/gtlbhynbwp.html

[T24] Swift：闭包
来源：http://hz.pengpengdd.cyou/gtnvrtyiwb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtyxguhtop.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gtyzjfgoya.html

struct P { var x: Int }
来源：http://hz.smart0.xyz/gtgfeuftij.html

[T26] Swift：类与重写
来源：http://hz.ivvv.top/gtgpgkdqoq.html

class A: Base { override func f() {} }
来源：http://hz.gogol.net.cn/gtqlvepiml.html

[T27] Swift：错误处理
来源：http://hz.jinghuilouyu.cn/gtgchbwoqu.html

do { try f() } catch { print(error) }
来源：http://hz.haohaochexian.top/gtlfqvhzke.html

[T28] Swift：枚举
来源：http://hz.fzhhl.top/gtjjwgctej.html

enum Color { case red, green }
来源：http://hz.xinyue.icu/gtnjjkmmgi.html

[T29] Swift：guard 提前返回
来源：http://hz.c1oappe.top/gtscimyzov.html

guard let x = opt else { return }
来源：http://hz.fzhhl.top/gtvxtpdvaa.html

[T30] Swift：协议
来源：http://hz.tianlin.xyz/gtoxnhszfw.html

protocol Shape { func area() -> Double }
来源：http://hz.guannengcc.top/gteuzujjas.html

[T31] Lua：Hello World
来源：http://hz.wangshuangyany.cn/gtzxccyvac.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtqbnuajjs.html

[T32] Lua：局部变量
来源：http://hz.snrcjt.cn/gtjslrtisv.html

local a = 1
来源：http://hz.quarkkingdee.top/gtvhjruzss.html

[T33] Lua：表（数组）
来源：http://hz.pengpengdd.cyou/gtbskplynq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgufenzy.top/gtjhbqfnrz.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtoviiiwra.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yangfankeji.com/gtcxgvowyb.html

[T35] Lua：字典表
来源：http://hz.jianghu66.top/gtunyfuwoz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guowangkeji.top/gtcbhqellf.html

[T36] Lua：函数
来源：http://hz.smart0.xyz/gtmfsbzubd.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtqtgvnwqs.html

[T37] Lua：字符串拼接
来源：http://hz.zdqjudy.top/gtnhunfxtd.html

"a" .. "b"
来源：http://hz.jinqigfzy.top/gtbvpqmmbn.html

[T38] Lua：条件
来源：http://hz.ppjwa.cn/gtssswwhmo.html

if x > 0 then print("正") end
来源：http://hz.smart0.xyz/gtcnaxjvma.html

[T39] Lua：模式匹配
来源：http://hz.jqgfzy.top/gtnkshvtuh.html

string.find(s, "%d+")
来源：http://hz.hnqzz.top/gtnqdxshpi.html

[T40] Lua：元表
来源：http://hz.yongpay.top/gtrcbjsgxh.html

setmetatable({}, { __index = base })
来源：http://hz.hfpthk.cn/gtuwlriwoa.html

[T41] Perl：Hello World
来源：http://hz.sysykeji.top/gtnfwyzmhb.html

print "Hello\n";
来源：http://hz.nanxuanxn.top/gtjiigvgdg.html

[T42] Perl：变量类型
来源：http://hz.iojbl.cn/gtzvdqthjn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cashguo.top/gtlyfxpzym.html

[T43] Perl：字符串插值
来源：http://hz.chenzaomai.com/gtoywgykfd.html

"值: $a"
来源：http://hz.yueranfly.top/gtxvwgwlxl.html

[T44] Perl：条件
来源：http://hz.jqgufenzy.top/gtpdbvdtnr.html

if ($a > 0) { print "正"; }
来源：http://hz.jyoumei.cn/gtgwsdhxay.html

[T45] Perl：数组遍历
来源：http://hz.shzxlz.cn/gtoffxmerf.html

for my $x (@arr) { print $x; }
来源：http://hz.fzhhl.top/gtpscroiic.html

[T46] Perl：哈希操作
来源：http://hz.chenzaomai.com/gttffmywac.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258888.top/gtpagsydmu.html

[T47] Perl：正则捕获
来源：http://hz.xingfuxueyuan.xyz/gtaczksnoa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.tanke756.top/gtnrznflzc.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtzlpsvqcq.html

$s =~ s/old/new/g;
来源：http://hz.jinqigfzy.top/gtsgexpzwo.html

[T49] Perl：函数
来源：http://hz.daria6918.cn/gthwmxrzfa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zycfv.cn/gtejdwnaef.html

[T50] Perl：逐行读文件
来源：http://hz.feifeiyinyue.top/gthayncnlo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xylfe.cn/gtyglxdngc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nanxuanxn.top/gtkrnyarut.html

[T51] Scala：Hello World
来源：http://hz.feifeiyinyue.top/gtadjoujlp.html

println("Hello")
来源：http://hz.zdqjudy.top/gtertgmtpr.html

[T52] Scala：变量
来源：http://hz.gotoacloud.top/gtbsebgxgg.html

val a = 1;  var b = 2
来源：http://hz.pengpengdd.cyou/gtidpgdrro.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gtvdvbznir.html

s"值: $b"
来源：http://hz.ppjwa.cn/gtagezftbf.html

[T54] Scala：集合映射
来源：http://hz.hnxiangtu.top/gtychzrlqg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.wangshuangyany.cn/gtmouinheu.html

[T55] Scala：集合过滤
来源：http://hz.guowangkeji.top/gtnmpdhwqt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.guannengcc.top/gtzezqthol.html

[T56] Scala：样例类
来源：http://hz.aizwys.cn/gtgijgutoq.html

case class User(name: String, age: Int)
来源：http://hz.ivvv.top/gtxpknqccb.html

[T57] Scala：模式匹配
来源：http://hz.hfpthk.cn/gtivuuxpup.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hnxiangtu.top/gthocrosyy.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtfgaezvqx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gteebsoqov.html

[T59] Scala：循环
来源：http://hz.sufxvd.cn/gtnldehvgn.html

for (i <- 1 to 10) println(i)
来源：http://hz.feifeiyinyue.top/gtcxbsvtdp.html

[T60] Scala：折叠
来源：http://hz.hnqzz.top/gtfwumznvp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sysykeji.top/gtksdxarkw.html

================================================================================
来源：http://hz.guowangkeji.top/gtznvkichw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtgfthahng.html

================================================================================
来源：http://hz.yvedp.cn/gtaxnhmmfn.html

[U01] Py：创建虚拟环境
来源：http://hz.shzxlz.cn/gteeetyrws.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hysaishi.cn/gtbbuxlnzc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.snrcjt.cn/gtitjmwpar.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtwixzndjv.html

[U03] Py：加载 .env 配置
来源：http://hz.ydzc1.top/gtauawsuch.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.tian-w.cn/gthxsekxtp.html

[U04] Py：变量调试打印
来源：http://hz.0kj1m.cn/gtqyfnnufi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj202588.top/gtjjgzwqqv.html

[U05] Py：列表去重且保序
来源：http://hz.zhongyouzk.top/gtsrbwsjwq.html

list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtgjktxrgl.html

[U06] Py：合并两个字典
来源：http://hz.quarkkingdee.top/gtjxjqjwzn.html

{**a, **b}
来源：http://hz.yvedp.cn/gtvrjjaulk.html

[U07] Py：反转字典键值
来源：http://hz.ydjk.org.cn/gtulfiqgqz.html

{v: k for k, v in d.items()}
来源：http://hz.jyoumei.cn/gtqtatqmwh.html

[U08] Py：展平二维列表
来源：http://hz.jianghu66.top/gtqgvapjqf.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtszslzwvx.html

[U09] Py：字典取最大值的键
来源：http://hz.yanxiufei.cn/gtusyikzji.html

max(d, key=d.get)
来源：http://hz.quarkkingdee.top/gticdbfqfk.html

[U10] Py：按值排序字典
来源：http://hz.jianghu66.top/gtgvntbgyv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hywenlv.cn/gtdkexrhmn.html

[U11] Py：生成器表达式
来源：http://hz.hnqzz.top/gtbdqjpjhu.html

(x * 2 for x in arr)
来源：http://hz.jinghuilouyu.cn/gtkfgiqnqv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.vqdsnc.cn/gtklijxypx.html

Counter(arr).most_common(3)
来源：http://hz.daria6918.cn/gtpuxpzstg.html

[U13] Py：固定长度队列
来源：http://hz.cashguo.top/gtjkvwrzyi.html

deque(maxlen=10)
来源：http://hz.yonumen.top/gtyblnzutl.html

[U14] Py：分组收集到列表
来源：http://hz.chenlongwang.top/gtndecmbqw.html

defaultdict(list)
来源：http://hz.hnxiangtu.top/gtlfmfszyn.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtufhkyreb.html

t = time.perf_counter()
来源：http://hz.cheryme.top/gtqzjyrjqs.html

[U16] Py：命令行参数解析
来源：http://hz.sufxvd.cn/gtlutzkrqq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhixingplan.top/gtyfrrprry.html

[U17] Py：初始化日志
来源：http://hz.xingfuxueyuan.xyz/gtdkydhygf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yanxiufei.cn/gtunqhgihj.html

[U18] Py：预编译正则
来源：http://hz.jianghu66.top/gtptewxyjh.html

pat = re.compile(r"\d+")
来源：http://hz.zhiwuduotai.top/gtjmpgmhgb.html

[U19] Py：正则替换带回调
来源：http://hz.vqdsnc.cn/gtrmxgozuu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sufxvd.cn/gtzomoxioj.html

[U20] Py：缓存函数结果
来源：http://hz.ybcxt.top/gttvhhghwo.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jqgfzy.top/gtdpsouofp.html

[U21] Py：自定义上下文管理器
来源：http://hz.tanke756.top/gtleckgwsy.html

@contextlib.contextmanager
来源：http://hz.yuxming.cn/gtrwfreerg.html

[U22] Py：矩阵转置
来源：http://hz.meibo888.top/gttfmvhdee.html

list(zip(*m))
来源：http://hz.sufxvd.cn/gtcvjqhblr.html

[U23] Py：分块读取大文件
来源：http://hz.vqdsnc.cn/gtlsferxwe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hnqzz.top/gtoovnfyds.html

[U24] Py：路径操作
来源：http://hz.iojbl.cn/gtbglmxmzj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sufxvd.cn/gtwrmtalky.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtqpltgvta.html

csv.DictReader(f)
来源：http://hz.snrcjt.cn/gtvkfkfnav.html

[U26] Py：并发下载
来源：http://hz.yuxming.cn/gtvgorjold.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cqqwz.cn/gtyddhibsz.html

[U27] Py：异步 HTTP
来源：http://hz.fengsongda.top/gtalhosmfw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hammf.cn/gtawhjeylz.html

[U28] Py：类型别名
来源：http://hz.cdnleiting.top/gtbcyzcpet.html

UserId = int
来源：http://hz.xuanzx.com/gtgltaaafj.html

[U29] Py：属性校验
来源：http://hz.guowangkeji.top/gtexjnaxbw.html

@property 与 @x.setter 配合
来源：http://hz.nanxinkj.top/gtftjwyzda.html

[U30] Py：数据类
来源：http://hz.meibo888.top/gtykyllgix.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtqadbztuu.html

[U31] Py：单测
来源：http://hz.9152youxi.cn/gtyovvrnuy.html

python -m pytest -q
来源：http://hz.fengsongda.top/gtyhsswtlv.html

[U32] Py：代码格式化
来源：http://hz.shanyushiyangkeji.top/gteajlolib.html

ruff format . && ruff check --fix .
来源：http://hz.tianlin.xyz/gtliyhjxex.html

[U33] Py：打包发布
来源：http://hz.hnxiangtu.top/gtobuksbzo.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gthxpsazzy.html

[U34] Py：判断编码
来源：http://hz.tian-w.cn/gtqjfrslpq.html

chardet.detect(raw)
来源：http://hz.meibo888.top/gtpcszqded.html

[U35] Py：发送邮件
来源：http://hz.zhixingplan.top/gtdcculcaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yanxiufei.cn/gtczhbhvno.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gttmxucums.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgufenzy.top/gtardombrr.html

[U37] Py：读写 Excel
来源：http://hz.hnqzz.top/gtjlwwposa.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hnqzz.top/gttwtssgmu.html

[U38] Py：获取脚本所在目录
来源：http://hz.haohaochexian.top/gtjyoaxqfa.html

Path(__file__).resolve().parent
来源：http://hz.yanxiufei.cn/gtmyzirzje.html

[U39] Py：判断是否在交互环境
来源：http://hz.dashuyun.cn/gthgoupyjb.html

sys.stdout.isatty()
来源：http://hz.aizwys.cn/gtoucpftjo.html

[U40] Py：打印到标准错误
来源：http://hz.yj202588.top/gtaolzkway.html

print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gtacfmrjtz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.gotoacloud.top/gtnmreavqw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gotoacloud.top/gtvpggqiyd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sufxvd.cn/gtlclfqodz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sufxvd.cn/gtbvoszecy.html

[U43] PHP：声明命名空间
来源：http://hz.yueranfly.top/gttkxxxajv.html

namespace App\Http;
来源：http://hz.52xcode.cn/gtsvejncxf.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtiqsxqkyd.html

declare(strict_types=1);
来源：http://hz.chenzaomai.com/gtkdiwhyzz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yangfankeji.com/gtdaurkaxb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gtyzecgtsb.html

[U46] PHP：可空类型
来源：http://hz.wangshuangyany.cn/gtruiojrun.html

?string $name = null
来源：http://hz.quarkkingdee.top/gtnqqsmpef.html

[U47] PHP：联合类型
来源：http://hz.mhx1999.top/gtnahwuxqj.html

int|string $id
来源：http://hz.yj20258.top/gtsfyndvnj.html

[U48] PHP：纯枚举
来源：http://hz.ywan-chungtsiang.top/gtrgnugdki.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj202588.top/gtfafagggu.html

[U49] PHP：只读属性
来源：http://hz.zhixingplan.top/gtenanrgrv.html

public readonly string $name
来源：http://hz.ybcxt.top/gtkiwoqtmq.html

[U50] PHP：构造器属性提升
来源：http://hz.cqqwz.cn/gtuqznfdnr.html

public function __construct(private int $id) {}
来源：http://hz.iojbl.cn/gtycttdjut.html

[U51] PHP：数组解构
来源：http://hz.jinghuilouyu.cn/gtgldtugwj.html

[$a, $b] = $arr;
来源：http://hz.hnxiangtu.top/gtanqasrlk.html

[U52] PHP：箭头函数
来源：http://hz.cdnleiting.top/gtlifpysmd.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtsdeldflz.html

[U53] PHP：空合并运算符
来源：http://hz.sysykeji.top/gtlrhgcofo.html

$v = $a ?? $b ?? "default";
来源：http://hz.xinyue.icu/gtjyjzvioi.html

[U54] PHP：空安全调用
来源：http://hz.fengsongda.top/gtczvxpuoh.html

$obj?->method()
来源：http://hz.wangdashe.top/gtnamomdhk.html

[U55] PHP：match 表达式
来源：http://hz.zycfv.cn/gtvuqazpxp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ywan-chungtsiang.top/gtrrkwfgbt.html

[U56] PHP：命名参数
来源：http://hz.ydzc1.top/gtwncblwjw.html

f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtjyxqormh.html

[U57] PHP：字符串插值
来源：http://hz.birdmap.top/gtanvhftws.html

"值: {$a}"
来源：http://hz.daxiang520.top/gtejuracqc.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtkuzutdds.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtpwnlgpuj.html

[U59] PHP：自定义排序
来源：http://hz.0kj1m.cn/gtljuxkpfz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dashuyun.cn/gtsdawjuhi.html

[U60] PHP：JSON 编解码
来源：http://hz.quarkkingdee.top/gtrezqubip.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shangyingyoupin.top/gtzlrdibhu.html

[U61] PHP：正则
来源：http://hz.ywan-chungtsiang.top/gtwpmkqsbj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtvmyedmpz.html

[U62] PHP：日期对象
来源：http://hz.tianlin.xyz/gtqzvppuvz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yj202588.top/gttgqxhuqr.html

[U63] PHP：文件读写
来源：http://hz.zhiwuduotai.top/gtcvrgozls.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gotoacloud.top/gtuzqaqwzd.html

[U64] PHP：目录遍历
来源：http://hz.yongpay.top/gtpetqzzmm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.zhengqikj.top/gthkhfbcxr.html

[U65] PHP：会话
来源：http://hz.bjfxy.top/gtvkmevrbc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.pengpengdd.cyou/gtravnipdr.html

[U66] PHP：设置 Cookie
来源：http://hz.hongshengwenyu.top/gtrujdqnuu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zycfv.cn/gtspopmfnz.html

[U67] PHP：处理文件上传
来源：http://hz.hnqzz.top/gtclommmtp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cqqwz.cn/gtvddyoatj.html

[U68] PHP：PDO 连接
来源：http://hz.c1oappe.top/gtloqsqmoy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.pengpengdd.cyou/gtaqqcjqpo.html

[U69] PHP：PDO 预处理
来源：http://hz.xingfuxueyuan.xyz/gtykgyyece.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ybcxt.top/gtrvdvxznu.html

[U70] PHP：PDO 事务
来源：http://hz.yanxiufei.cn/gtzamrxpum.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yj20258.top/gtyhnhgprr.html

[U71] PHP：抛出异常
来源：http://hz.jinyuanbaomall.cn/gtydayyxzk.html

throw new RuntimeException("失败", 500);
来源：http://hz.316326.xyz/gtddumvunt.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangkeji.top/gtezgotbev.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zhengqikj.top/gtraeknyvi.html


<!-- 参考信息 -->