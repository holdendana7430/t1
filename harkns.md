代发 wailian999

[S43] C++：智能指针
来源：http://hz.guowangkeji.top/gtcealabbt.html

auto p = std::make_unique<int>(5);
来源：http://hz.ivvv.top/gtrpoxbqvp.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gttclxvauc.html

void inc(int &x) { ++x; }
来源：http://hz.aibaodan.cn/gtbijpajld.html

[S45] C++：lambda
来源：http://hz.yuxming.cn/gtoyowfaut.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtovhcgxzp.html

[S46] C++：函数模板
来源：http://hz.zhoulong.xyz/gtnehlbsbh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtqvnmmtjc.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtcquaqaek.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtwjnynlkc.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtmuoxbdyc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtsrjmmqqi.html

while (std::getline(in, line)) { }
来源：http://hz.gzhubu.top/gtjymemgve.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtbwhxpovc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtfxzkqpgq.html

[S50] C++：格式化数字
来源：http://hz.dashuyun.cn/gtzgcshnsk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ehwqpu.com/gtnilkioft.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gtzcodrzoo.html

static_cast<double>(a) / b
来源：http://hz.svipenyu.cn/gtxlwvpxox.html

[S52] C++：const 与 noexcept
来源：http://hz.zhiwuduotai.top/gtbsyhhvjv.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtdblpetwn.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtkzbbjnah.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtmppoxdrr.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gthsqeszvy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gtoevmyeme.html

[S55] C++：结构化绑定
来源：http://hz.dashuyun.cn/gtlahgqhdy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yuxming.cn/gtuottzwea.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtgseqflls.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtzwkvisbn.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtlqktptxi.html

constexpr int N = 10;
来源：http://hz.hnxiangtu.top/gtkyllrlrl.html

[S58] C++：命名空间
来源：http://hz.chenjidiqi.icu/gtmsdtyaeb.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gtnrvhchap.html

[S59] C++：静态断言
来源：http://hz.yongpay.top/gtflcffyka.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinghuilouyu.cn/gtbvorwahf.html

[S60] C++：遍历并删除元素
来源：http://hz.zhengqikj.top/gtqtpxucpt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydjk.org.cn/gtsczugwki.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtipmsfqjc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cheryme.top/gtzalccvog.html

================================================================================
来源：http://hz.guannengcc.top/gtirndsqfb.html

[T01] Kotlin：Hello World
来源：http://hz.andypj.xyz/gtkbarikzt.html

println("Hello")
来源：http://hz.yueranfly.top/gtsconfbua.html

[T02] Kotlin：变量
来源：http://hz.aizwys.cn/gtvelknxmz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guannengcc.top/gtkpautrqv.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gthkntwevs.html

"值: $b"
来源：http://hz.iojbl.cn/gtpxuplvqx.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtizfinilr.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtkdjfvlew.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtrmglwauz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ywan-chungtsiang.top/gtcucjqzab.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gtrktiuqcj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shuidangran.top/gtieqrxdzr.html

[T07] Kotlin：集合过滤
来源：http://hz.gogol.net.cn/gtqtuqdgnd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gtsvhrqwbm.html

[T08] Kotlin：数据类
来源：http://hz.zhaomingkeji.xyz/gtjilxfowj.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgufenzy.top/gtfpcsoclo.html

[T09] Kotlin：扩展函数
来源：http://hz.zhiwuduotai.top/gtxddhiwmr.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtibrnhwhr.html

[T10] Kotlin：默认参数
来源：http://hz.wangdashe.top/gtzywlyilj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtrvvfyiei.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtouaomwjz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuanzx.com/gthtkuailm.html

[T12] Kotlin：解构声明
来源：http://hz.bjfxy.top/gtckctogns.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhijiandao.cn/gtbbtwdapf.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtwpyffcvi.html

val m = mapOf("a" to 1)
来源：http://hz.gotoacloud.top/gtaqiyejjf.html

[T14] Kotlin：循环
来源：http://hz.cucudq.cn/gtcgawucup.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtdsrvmboi.html

[T15] Kotlin：接口
来源：http://hz.hysaishi.cn/gtfbzvvkuf.html

interface Shape { fun area(): Double }
来源：http://hz.ybcxt.top/gtnrdbdbug.html

[T16] Swift：Hello World
来源：http://hz.hnxiangtu.top/gtdbaxfjeq.html

print("Hello")
来源：http://hz.havefunace.top/gtsjesjwvf.html

[T17] Swift：变量与常量
来源：http://hz.zhengqikj.top/gtlorztajb.html

var a = 1;  let b = 2
来源：http://hz.gzhubu.top/gtountknjo.html

[T18] Swift：字符串插值
来源：http://hz.svipenyu.cn/gtjlxwzctr.html

"值: \(b)"
来源：http://hz.gaohongyu789.top/gtcpilhpra.html

[T19] Swift：可选绑定
来源：http://hz.dashuyun.cn/gtxwkhsvka.html

if let n = opt { print(n) }
来源：http://hz.zhoulong.xyz/gtgbzdyjzj.html

[T20] Swift：数组操作
来源：http://hz.yuanzhike.top/gtbdlxewwb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtxggrvlzy.html

[T21] Swift：遍历
来源：http://hz.zycfv.cn/gtxlnqylpl.html

for x in a { print(x) }
来源：http://hz.zhijiandao.cn/gtvkwnqizq.html

[T22] Swift：字典
来源：http://hz.shuidangran.top/gtakhsyjpi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xinyue.icu/gtyomiarwq.html

[T23] Swift：函数
来源：http://hz.52xcode.cn/gtqorbgdne.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxinkj.top/gtlhwwvxhp.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtundxddex.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.birdmap.top/gtjwzbvfoz.html

[T25] Swift：结构体
来源：http://hz.aizwys.cn/gteulqlhit.html

struct P { var x: Int }
来源：http://hz.shuidangran.top/gtdqimumwt.html

[T26] Swift：类与重写
来源：http://hz.jianghu66.top/gtckwvdnii.html

class A: Base { override func f() {} }
来源：http://hz.andypj.xyz/gtuqgbeydu.html

[T27] Swift：错误处理
来源：http://hz.52xcode.cn/gtmphjfrll.html

do { try f() } catch { print(error) }
来源：http://hz.c1oappe.top/gtglmcaywq.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtbzaawykj.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtlrlnvpec.html

[T29] Swift：guard 提前返回
来源：http://hz.gogol.net.cn/gtwtdwkhsh.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtqdytuveb.html

[T30] Swift：协议
来源：http://hz.ywan-chungtsiang.top/gtybrstoxz.html

protocol Shape { func area() -> Double }
来源：http://hz.zhiwuduotai.top/gttpjcphzm.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtbkfsbpxe.html

print("Hello")
来源：http://hz.xinyue.icu/gtkrmrevrb.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtsddhpdoq.html

local a = 1
来源：http://hz.redwolf501.top/gtepknfriv.html

[T33] Lua：表（数组）
来源：http://hz.yuanzhike.top/gtmrnjmtkw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gotoacloud.top/gtqkfglaii.html

[T34] Lua：遍历表
来源：http://hz.316326.xyz/gtupoteatr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gtwsbntagx.html

[T35] Lua：字典表
来源：http://hz.quarkkingdee.top/gtenjclnvc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.vqdsnc.cn/gtgonynfos.html

[T36] Lua：函数
来源：http://hz.guannengcc.top/gtdokzgnpo.html

function add(a, b) return a + b end
来源：http://hz.quarkkingdee.top/gtzrpyqtoo.html

[T37] Lua：字符串拼接
来源：http://hz.hywenlv.cn/gtelapxvre.html

"a" .. "b"
来源：http://hz.yuanzhike.top/gtjzxujcqq.html

[T38] Lua：条件
来源：http://hz.52xcode.cn/gtohcrhsdv.html

if x > 0 then print("正") end
来源：http://hz.smart0.xyz/gtepyejgzr.html

[T39] Lua：模式匹配
来源：http://hz.0kj1m.cn/gtwsriahpv.html

string.find(s, "%d+")
来源：http://hz.xylfe.cn/gtlvkvgvez.html

[T40] Lua：元表
来源：http://hz.cqqwz.cn/gtqtqaykdr.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gtgoiiywwe.html

[T41] Perl：Hello World
来源：http://hz.jiagoushi.top/gtovxtklms.html

print "Hello\n";
来源：http://hz.haohaochexian.top/gtaapconqo.html

[T42] Perl：变量类型
来源：http://hz.xuetiantiany.cn/gtbcerlpwf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gtskrxhjgf.html

[T43] Perl：字符串插值
来源：http://hz.gotoacloud.top/gtsoobagds.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtyotssvna.html

[T44] Perl：条件
来源：http://hz.xziqi.cn/gtjhfkncmj.html

if ($a > 0) { print "正"; }
来源：http://hz.jyoumei.cn/gtqkmpmjju.html

[T45] Perl：数组遍历
来源：http://hz.shzxlz.cn/gtgdsdubfi.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtyykgcvbv.html

[T46] Perl：哈希操作
来源：http://hz.zhiwuduotai.top/gtrklawarp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenzaomai.com/gtdahhcarp.html

[T47] Perl：正则捕获
来源：http://hz.hywenlv.cn/gtjtczandw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daxiang520.top/gtftbfmjky.html

[T48] Perl：正则替换
来源：http://hz.feifeiyinyue.top/gtcoyjmacg.html

$s =~ s/old/new/g;
来源：http://hz.sysykeji.top/gteaaqpvob.html

[T49] Perl：函数
来源：http://hz.ivvv.top/gtkqukhoql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtjqhrljdn.html

[T50] Perl：逐行读文件
来源：http://hz.tanke756.top/gtmzbpvbxz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtnvtsujyu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.dashuyun.cn/gtvmtawffi.html

[T51] Scala：Hello World
来源：http://hz.chenzaomai.com/gtzsbytghp.html

println("Hello")
来源：http://hz.zdqjudy.top/gtjcknxcsp.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtolrifmbb.html

val a = 1;  var b = 2
来源：http://hz.316326.xyz/gtaktfbwpp.html

[T53] Scala：字符串插值
来源：http://hz.hnqzz.top/gtcljpbhve.html

s"值: $b"
来源：http://hz.nwbrower.top/gtjkfkdcza.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gtdkvizcke.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.mhx1999.top/gtnybdmfpz.html

[T55] Scala：集合过滤
来源：http://hz.gogol.net.cn/gtkkpeyrux.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydzc1.top/gtbfiqhwgr.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtqmobzjxn.html

case class User(name: String, age: Int)
来源：http://hz.zhoulong.xyz/gtnirrnwej.html

[T57] Scala：模式匹配
来源：http://hz.yj20258888.top/gtvexfltyt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.bjfxy.top/gtbpayphga.html

[T58] Scala：函数定义
来源：http://hz.cqqwz.cn/gtpmihzeav.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.haohaochexian.top/gtnsygglqu.html

[T59] Scala：循环
来源：http://hz.cheryme.top/gtyxubsrdc.html

for (i <- 1 to 10) println(i)
来源：http://hz.316326.xyz/gtozpgwzox.html

[T60] Scala：折叠
来源：http://hz.andypj.xyz/gtnbkvdezi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cucudq.cn/gtzbndhqnh.html

================================================================================
来源：http://hz.jianghu66.top/gtbpzwruwm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.nanxuanxn.top/gtknxgdpkf.html

================================================================================
来源：http://hz.meibo888.top/gtjbxknqkm.html

[U01] Py：创建虚拟环境
来源：http://hz.wangdashe.top/gtoudmpwui.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.svipenyu.cn/gtyqghldyz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.kuanghao11.cn/gtlailgcdd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtwkinznrm.html

[U03] Py：加载 .env 配置
来源：http://hz.hysaishi.cn/gtxacghrli.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtwxlafemy.html

[U04] Py：变量调试打印
来源：http://hz.ivvv.top/gtopggkrjz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.aibaodan.cn/gtwcijewnw.html

[U05] Py：列表去重且保序
来源：http://hz.hywenlv.cn/gtrllneqqp.html

list(dict.fromkeys(arr))
来源：http://hz.gogol.net.cn/gtcjozrxch.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gtzpbouffa.html

{**a, **b}
来源：http://hz.mhx1999.top/gtzbrobmrt.html

[U07] Py：反转字典键值
来源：http://hz.gotoacloud.top/gtfiiopgen.html

{v: k for k, v in d.items()}
来源：http://hz.iojbl.cn/gtccnxqkbw.html

[U08] Py：展平二维列表
来源：http://hz.daxiang520.top/gtyzedspvm.html

[y for x in nested for y in x]
来源：http://hz.jqgufenzy.top/gtkjzjonhn.html

[U09] Py：字典取最大值的键
来源：http://hz.nwbrower.top/gtvwqlqxui.html

max(d, key=d.get)
来源：http://hz.birdmap.top/gtfnzjkdvt.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gtlfjqdjsw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuanzhike.top/gtruyqalbw.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtdltsggbk.html

(x * 2 for x in arr)
来源：http://hz.gotoacloud.top/gttpaywcsy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zdqjudy.top/gtbqmwbjrx.html

Counter(arr).most_common(3)
来源：http://hz.yongpay.top/gtoodlbsos.html

[U13] Py：固定长度队列
来源：http://hz.zhiwuduotai.top/gtyjmefvdj.html

deque(maxlen=10)
来源：http://hz.52xcode.cn/gtgzspzhvi.html

[U14] Py：分组收集到列表
来源：http://hz.xziqi.cn/gtgzfmqtth.html

defaultdict(list)
来源：http://hz.hammf.cn/gtmjhoiejw.html

[U15] Py：高精度计时
来源：http://hz.havefunace.top/gtylikfdgt.html

t = time.perf_counter()
来源：http://hz.yanxiufei.cn/gtkchkwwsl.html

[U16] Py：命令行参数解析
来源：http://hz.gaohongyu789.top/gtlqrfhrwm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtkjemitdw.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gtlslljcqk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtqenkckvz.html

[U18] Py：预编译正则
来源：http://hz.guowangkeji.top/gtnldyvqos.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtbhyiftsv.html

[U19] Py：正则替换带回调
来源：http://hz.ybcxt.top/gthydfdsih.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.smart0.xyz/gtiepdoram.html

[U20] Py：缓存函数结果
来源：http://hz.ivvv.top/gtvgoobhjx.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtiewktdwg.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gteqgzfbvo.html

@contextlib.contextmanager
来源：http://hz.xinyue.icu/gtintpocnc.html

[U22] Py：矩阵转置
来源：http://hz.haohaochexian.top/gtkclncxbb.html

list(zip(*m))
来源：http://hz.jiagoushi.top/gtemthmtoi.html

[U23] Py：分块读取大文件
来源：http://hz.gaohongyu789.top/gtzawiwwrt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cqqwz.cn/gtgqmyvzdy.html

[U24] Py：路径操作
来源：http://hz.cashguo.top/gtuxwtwsjo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.pycfn.com/gtatbquusb.html

[U25] Py：CSV 按字典读
来源：http://hz.dashuyun.cn/gtnszmzalb.html

csv.DictReader(f)
来源：http://hz.andypj.xyz/gtifsucvuo.html

[U26] Py：并发下载
来源：http://hz.zdqjudy.top/gtdwgklbcf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.meibo888.top/gtucaxkmgm.html

[U27] Py：异步 HTTP
来源：http://hz.zhixingplan.top/gtfdgkosag.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.tian-w.cn/gthyhqmhyh.html

[U28] Py：类型别名
来源：http://hz.zdqjudy.top/gtromqnsgo.html

UserId = int
来源：http://hz.chenlongwang.top/gtydqdqzhb.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtujmvwthm.html

@property 与 @x.setter 配合
来源：http://hz.tanke756.top/gtwwqajmdd.html

[U30] Py：数据类
来源：http://hz.gotoacloud.top/gtpxkxwmrc.html

@dataclass(slots=True)
来源：http://hz.gaohongyu789.top/gtlufjilvr.html

[U31] Py：单测
来源：http://hz.jyoumei.cn/gtfrsfxvkh.html

python -m pytest -q
来源：http://hz.pycfn.com/gtfyaxuxaa.html

[U32] Py：代码格式化
来源：http://hz.nwbrower.top/gtymcdemdb.html

ruff format . && ruff check --fix .
来源：http://hz.sufxvd.cn/gtubyopeuu.html

[U33] Py：打包发布
来源：http://hz.zycfv.cn/gtiummletj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtvxptvoaz.html

[U34] Py：判断编码
来源：http://hz.cheryme.top/gtyeaecwwj.html

chardet.detect(raw)
来源：http://hz.ybcxt.top/gtlohxejip.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangtech.top/gtsjqudigt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ivvv.top/gtlnxtjaja.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtwghxkgwk.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gtgjuqhzxa.html

[U37] Py：读写 Excel
来源：http://hz.meibo888.top/gtyywauybz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinqigufen.top/gtjmapxktu.html

[U38] Py：获取脚本所在目录
来源：http://hz.guannengcc.top/gteflbnhju.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtbvglriuw.html

[U39] Py：判断是否在交互环境
来源：http://hz.smart0.xyz/gtwmtzcevp.html

sys.stdout.isatty()
来源：http://hz.yuxming.cn/gtoaepaugb.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtbigyryzk.html

print("err", file=sys.stderr)
来源：http://hz.dashuyun.cn/gtytmjslpq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.xingfuxueyuan.xyz/gtlnbmlwnk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhengqikj.top/gtemfloptj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sysykeji.top/gtytkvjqpy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.fengsongda.top/gtbmptwhtx.html

[U43] PHP：声明命名空间
来源：http://hz.chenlongwang.top/gtqqsnxyzp.html

namespace App\Http;
来源：http://hz.pengpengdd.cyou/gtplhmimsm.html

[U44] PHP：开启严格类型
来源：http://hz.yj202588.top/gtznfqwxtu.html

declare(strict_types=1);
来源：http://hz.wangdashe.top/gtjhomzmpb.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangtech.top/gtsflnjhvq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtyaqugquh.html

[U46] PHP：可空类型
来源：http://hz.zhijiandao.cn/gtffhtjzhu.html

?string $name = null
来源：http://hz.9152youxi.cn/gtdhgonzpt.html

[U47] PHP：联合类型
来源：http://hz.iojbl.cn/gtvwzgxtwz.html

int|string $id
来源：http://hz.cqqwz.cn/gthidxerka.html

[U48] PHP：纯枚举
来源：http://hz.xinyue.icu/gtumijkcil.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xuanzx.com/gtlgjzefyb.html

[U49] PHP：只读属性
来源：http://hz.0kj1m.cn/gtvaqhqabi.html

public readonly string $name
来源：http://hz.zhijiandao.cn/gtqjjtjzbj.html

[U50] PHP：构造器属性提升
来源：http://hz.sysykeji.top/gtabztamqp.html

public function __construct(private int $id) {}
来源：http://hz.wangdashe.top/gtlaracljw.html

[U51] PHP：数组解构
来源：http://hz.nanxuanxn.top/gtpvcocunu.html

[$a, $b] = $arr;
来源：http://hz.yj202588.top/gtrbvfeatg.html

[U52] PHP：箭头函数
来源：http://hz.haohaochexian.top/gtfxybuieh.html

$double = fn($x) => $x * 2;
来源：http://hz.hysaishi.cn/gtkegxamgc.html

[U53] PHP：空合并运算符
来源：http://hz.snrcjt.cn/gtmyvlahjq.html

$v = $a ?? $b ?? "default";
来源：http://hz.yj202588.top/gtjjfavqcy.html

[U54] PHP：空安全调用
来源：http://hz.haohaochexian.top/gtyjwsibml.html

$obj?->method()
来源：http://hz.tian-w.cn/gtuaoezgvl.html

[U55] PHP：match 表达式
来源：http://hz.nanxinkj.top/gtmpppvfrk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zycfv.cn/gtocokkxvn.html

[U56] PHP：命名参数
来源：http://hz.jiagoushi.top/gtwfmrbxoa.html

f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtswbrjzwb.html

[U57] PHP：字符串插值
来源：http://hz.shuidangran.top/gtimslyshl.html

"值: {$a}"
来源：http://hz.cashguo.top/gtcawhccno.html

[U58] PHP：数组三件套
来源：http://hz.zdqjudy.top/gthivzcmka.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhaomingkeji.xyz/gtkcdpyjrz.html

[U59] PHP：自定义排序
来源：http://hz.zhongyouzk.top/gtcqnogaly.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtsmuhmybk.html

[U60] PHP：JSON 编解码
来源：http://hz.xylfe.cn/gtnylnntlq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.yvedp.cn/gtxoksmwcs.html

[U61] PHP：正则
来源：http://hz.sxryk.cn/gtoshidako.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtzsjbuujn.html

[U62] PHP：日期对象
来源：http://hz.ehwqpu.com/gtizypabtt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.snrcjt.cn/gtjgohbnro.html

[U63] PHP：文件读写
来源：http://hz.chenjidiqi.icu/gtfgncrnux.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hammf.cn/gtkamcpygz.html

[U64] PHP：目录遍历
来源：http://hz.guowangkeji.top/gtwjlgzsdr.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aizwys.cn/gtkvhebkdf.html

[U65] PHP：会话
来源：http://hz.jlsjyb.cn/gtbgyiqdag.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.cdnleiting.top/gtqzebuhjk.html

[U66] PHP：设置 Cookie
来源：http://hz.birdmap.top/gtfobhnxgn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.haohaochexian.top/gttxwqadsk.html

[U67] PHP：处理文件上传
来源：http://hz.zhengqikj.top/gtpkyiexas.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yongpay.top/gtqjpgfdgi.html

[U68] PHP：PDO 连接
来源：http://hz.sweek.top/gtcpxhaskd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shangyingyoupin.top/gtmhjsnyab.html


<!-- 参考信息 -->