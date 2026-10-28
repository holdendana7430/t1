代发 wailian999

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtpfljdemp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtxppoequj.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtewsmyeme.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtvbvebpap.html

[S37] C++：set
来源：http://hz.yuxming.cn/gtmlhtwdmp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.dashuyun.cn/gtflmtaegl.html

[S38] C++：排序
来源：http://hz.aibaodan.cn/gtywwyefwv.html

std::sort(v.begin(), v.end());
来源：http://hz.yonumen.top/gtcfjymldo.html

[S39] C++：自定义比较器排序
来源：http://hz.zycfv.cn/gtikjcgjap.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnqzz.top/gtlffmlzxw.html

[S40] C++：查找元素
来源：http://hz.yonumen.top/gtkkcvawcc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtpccddjru.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtkprchdzn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gtkzhshiiw.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtxbtfunvs.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtlbfczbqm.html

[S43] C++：智能指针
来源：http://hz.zhongyouzk.top/gtileouvoq.html

auto p = std::make_unique<int>(5);
来源：http://hz.sysykeji.top/gtgtvomjic.html

[S44] C++：引用传参
来源：http://hz.jyoumei.cn/gtyuapahvt.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtqjebrdsu.html

[S45] C++：lambda
来源：http://hz.havefunace.top/gtfrfjzkod.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xziqi.cn/gtdnnonjzq.html

[S46] C++：函数模板
来源：http://hz.redwolf501.top/gtbqjplpem.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtxxsbacau.html

[S47] C++：结构化绑定遍历
来源：http://hz.yanxiufei.cn/gtlfmqjzjz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cqqwz.cn/gtiuekjmve.html

[S48] C++：逐行读文件
来源：http://hz.sweek.top/gtbrkdkeez.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtqwlgsyho.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtcyblxdet.html

[S49] C++：写文件
来源：http://hz.dashuyun.cn/gtubcnzbag.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhijiandao.cn/gtrraarurx.html

[S50] C++：格式化数字
来源：http://hz.svipenyu.cn/gtusslehxn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hywenlv.cn/gtystywmec.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtutdzahtg.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtoailmhdb.html

[S52] C++：const 与 noexcept
来源：http://hz.yvedp.cn/gtkooqfhoc.html

int size() const noexcept { return n_; }
来源：http://hz.bjfxy.top/gteziqtnee.html

[S53] C++：移动语义
来源：http://hz.meibo888.top/gtidbspywo.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtwadayfym.html

[S54] C++：异常处理
来源：http://hz.yangfankeji.com/gtotjzraqj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jlsjyb.cn/gtigcblqyk.html

[S55] C++：结构化绑定
来源：http://hz.cdnleiting.top/gtlqqmvqyd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtirvhqvbx.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gtxsajjqum.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fzhhl.top/gtqtbnutjg.html

[S57] C++：编译期常量
来源：http://hz.dianchejie.cn/gtwtrkccpp.html

constexpr int N = 10;
来源：http://hz.sysykeji.top/gtagxvuyyi.html

[S58] C++：命名空间
来源：http://hz.mhx1999.top/gtxpgijufj.html

namespace ns { int f() { return 1; } }
来源：http://hz.52xcode.cn/gtflluecwa.html

[S59] C++：静态断言
来源：http://hz.0kj1m.cn/gtmdexnjhd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gogol.net.cn/gtsanvmddu.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtwlnhhapi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtyztjuyux.html

================================================================================
来源：http://hz.xinyue.icu/gtkhjtbgku.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gtrfjigcdy.html

================================================================================
来源：http://hz.chenzaomai.com/gtawxmokam.html

[T01] Kotlin：Hello World
来源：http://hz.jinqigfzy.top/gtutwudhwf.html

println("Hello")
来源：http://hz.vqdsnc.cn/gttjjzlrej.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtloupshox.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.feifeiyinyue.top/gtcsujbwuc.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtpgqemvcg.html

"值: $b"
来源：http://hz.mhx1999.top/gtcphoukyk.html

[T04] Kotlin：空安全
来源：http://hz.svipenyu.cn/gtsnjsmiox.html

val n: String? = null;  n?.length
来源：http://hz.tianlin.xyz/gtibzorzwb.html

[T05] Kotlin：when 表达式
来源：http://hz.havefunace.top/gtnyoyxmlo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtejogudkh.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gtrbgkwadf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtuoszctfy.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gtabiuuuqa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sxryk.cn/gthjxlturu.html

[T08] Kotlin：数据类
来源：http://hz.smart0.xyz/gtletecuye.html

data class User(val name: String, val age: Int)
来源：http://hz.zhixingplan.top/gtvxgrpxik.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtlampngrj.html

fun String.exclaim() = this + "!"
来源：http://hz.zhixingplan.top/gtxqzpcjxc.html

[T10] Kotlin：默认参数
来源：http://hz.ybcxt.top/gtjuonoocg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gttebdqttv.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtozwryrwj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daria6918.cn/gtzzgwkfbg.html

[T12] Kotlin：解构声明
来源：http://hz.guowangkeji.top/gtawwiqxqq.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtbuarvxvs.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtzbwnhtkr.html

val m = mapOf("a" to 1)
来源：http://hz.gogol.net.cn/gtaevrnnjd.html

[T14] Kotlin：循环
来源：http://hz.tianlin.xyz/gtobnglznw.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtuvfjnizz.html

[T15] Kotlin：接口
来源：http://hz.tian-w.cn/gtddgmmucq.html

interface Shape { fun area(): Double }
来源：http://hz.fzhhl.top/gtibttdhfa.html

[T16] Swift：Hello World
来源：http://hz.yueranfly.top/gteqgfjgfz.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtplwkhqkc.html

[T17] Swift：变量与常量
来源：http://hz.cheryme.top/gtrcixjyeb.html

var a = 1;  let b = 2
来源：http://hz.cucudq.cn/gtrubfgrna.html

[T18] Swift：字符串插值
来源：http://hz.yuxming.cn/gthjroljsi.html

"值: \(b)"
来源：http://hz.fengsongda.top/gtodrrtahy.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtiskxkkul.html

if let n = opt { print(n) }
来源：http://hz.xuetiantiany.cn/gtibsjfjcr.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtsduafauj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cashguo.top/gtuyxykeft.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gtsjvwcssp.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtdsidzfcd.html

[T22] Swift：字典
来源：http://hz.nanxinkj.top/gtmehalhkv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtvveuempv.html

[T23] Swift：函数
来源：http://hz.ybcxt.top/gtbfhtnrns.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.birdmap.top/gtjodohlch.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtfxzbzaxs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtsdewoqen.html

[T25] Swift：结构体
来源：http://hz.c1oappe.top/gtdqtspuwc.html

struct P { var x: Int }
来源：http://hz.hammf.cn/gtgjhgreue.html

[T26] Swift：类与重写
来源：http://hz.chenlongwang.top/gtgrnmmjlo.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtttllupjs.html

[T27] Swift：错误处理
来源：http://hz.feifeiyinyue.top/gtzrlylcws.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtfwgnifco.html

[T28] Swift：枚举
来源：http://hz.svipenyu.cn/gtczoeoxxe.html

enum Color { case red, green }
来源：http://hz.zdqjudy.top/gtnrcrynxd.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtmtpmjikt.html

guard let x = opt else { return }
来源：http://hz.shanyushiyangkeji.top/gtyaoubbjk.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gtfkklcipu.html

protocol Shape { func area() -> Double }
来源：http://hz.jinyuanbaomall.cn/gtxodvwzpm.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gtqvsbtnrf.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtkmjxpwxe.html

[T32] Lua：局部变量
来源：http://hz.jinqigfzy.top/gtcsifgdmg.html

local a = 1
来源：http://hz.chenjidiqi.icu/gttdpkciuh.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gtjxjndvsi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sufxvd.cn/gteaelhcck.html

[T34] Lua：遍历表
来源：http://hz.zhaomingkeji.xyz/gtjriaxull.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sufxvd.cn/gtqwceioan.html

[T35] Lua：字典表
来源：http://hz.shuidangran.top/gtxfbrlfsa.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daria6918.cn/gteotllsmz.html

[T36] Lua：函数
来源：http://hz.mhx1999.top/gtwncskawd.html

function add(a, b) return a + b end
来源：http://hz.aizwys.cn/gtkuprlnme.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gtiytrsoik.html

"a" .. "b"
来源：http://hz.gzhubu.top/gtfjlcxdey.html

[T38] Lua：条件
来源：http://hz.yanxiufei.cn/gtwtkoadaq.html

if x > 0 then print("正") end
来源：http://hz.zhijiandao.cn/gtzihveqqd.html

[T39] Lua：模式匹配
来源：http://hz.andypj.xyz/gtkzihuzpt.html

string.find(s, "%d+")
来源：http://hz.xylfe.cn/gtkutjrxwk.html

[T40] Lua：元表
来源：http://hz.jinyuanbaomall.cn/gthbomqbvt.html

setmetatable({}, { __index = base })
来源：http://hz.ywan-chungtsiang.top/gtvroylaxu.html

[T41] Perl：Hello World
来源：http://hz.sxryk.cn/gtywymrduy.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gtgudwvwld.html

[T42] Perl：变量类型
来源：http://hz.birdmap.top/gtkdqvyfjt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenzaomai.com/gtpojngibn.html

[T43] Perl：字符串插值
来源：http://hz.chenjidiqi.icu/gtjhidypmz.html

"值: $a"
来源：http://hz.xingfuxueyuan.xyz/gtfpbvtfnw.html

[T44] Perl：条件
来源：http://hz.smart0.xyz/gtxpnxxezg.html

if ($a > 0) { print "正"; }
来源：http://hz.zhixingplan.top/gtwbiuoegk.html

[T45] Perl：数组遍历
来源：http://hz.jyoumei.cn/gtdkjepsiy.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtcszjzesi.html

[T46] Perl：哈希操作
来源：http://hz.hywenlv.cn/gtfxikqosf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yonumen.top/gttainzhfd.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtuqhxyhqk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.havefunace.top/gtaazelsxe.html

[T48] Perl：正则替换
来源：http://hz.gogol.net.cn/gtqqnuzeil.html

$s =~ s/old/new/g;
来源：http://hz.yj20258888.top/gtkdvenlwu.html

[T49] Perl：函数
来源：http://hz.hammf.cn/gttphxwjqc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhongyouzk.top/gtxppriido.html

[T50] Perl：逐行读文件
来源：http://hz.xylfe.cn/gtndhiagmv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jlsjyb.cn/gtgwsorahc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.kuanghao11.cn/gtswhynmhd.html

[T51] Scala：Hello World
来源：http://hz.fengsongda.top/gtbsqybyuy.html

println("Hello")
来源：http://hz.xinyue.icu/gtphhzjrhr.html

[T52] Scala：变量
来源：http://hz.jinqigufen.top/gtlzdjwxvg.html

val a = 1;  var b = 2
来源：http://hz.jinqigfzy.top/gtwrognbvg.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gtcdjjutew.html

s"值: $b"
来源：http://hz.c1oappe.top/gteztzfdte.html

[T54] Scala：集合映射
来源：http://hz.jinqigfzy.top/gtnouhjmzx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtagtklqij.html

[T55] Scala：集合过滤
来源：http://hz.yj202588.top/gtrfajxpyd.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shuidangran.top/gtrsjswopg.html

[T56] Scala：样例类
来源：http://hz.zhongyouzk.top/gtlyzopggp.html

case class User(name: String, age: Int)
来源：http://hz.xuanzx.com/gtwcnmzqft.html

[T57] Scala：模式匹配
来源：http://hz.quarkkingdee.top/gtdixqdmva.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fzhhl.top/gtmfyibxfz.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtrhvqscot.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cqqwz.cn/gtsuoyabaq.html

[T59] Scala：循环
来源：http://hz.ydjk.org.cn/gtmekznios.html

for (i <- 1 to 10) println(i)
来源：http://hz.xinyue.icu/gtxfgbotjw.html

[T60] Scala：折叠
来源：http://hz.zhongyouzk.top/gtfscttfel.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.tian-w.cn/gtkvkktzcr.html

================================================================================
来源：http://hz.xziqi.cn/gtumalnxqd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtufxhflnn.html

================================================================================
来源：http://hz.yonumen.top/gtzodlwoyh.html

[U01] Py：创建虚拟环境
来源：http://hz.xuetiantiany.cn/gtqmqkbxau.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.kuanghao11.cn/gtkxgqhalp.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtuqmvabnj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhiwuduotai.top/gtdjfhxtyf.html

[U03] Py：加载 .env 配置
来源：http://hz.hongshengwenyu.top/gtvboporeg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuanzx.com/gtmlxmwdqy.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gtrqedrrfj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gttatprwjh.html

[U05] Py：列表去重且保序
来源：http://hz.xylfe.cn/gtrdwrqpmr.html

list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtadaxtbvv.html

[U06] Py：合并两个字典
来源：http://hz.sweek.top/gtmzrhcrse.html

{**a, **b}
来源：http://hz.ydzc1.top/gtvituddqm.html

[U07] Py：反转字典键值
来源：http://hz.chenlongwang.top/gtcikqwsue.html

{v: k for k, v in d.items()}
来源：http://hz.fzhhl.top/gtfzbcakfc.html

[U08] Py：展平二维列表
来源：http://hz.fzhhl.top/gtprhjkziy.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtcjazzdro.html

[U09] Py：字典取最大值的键
来源：http://hz.haohaochexian.top/gtwczdtobg.html

max(d, key=d.get)
来源：http://hz.zhiwuduotai.top/gtgurlocfm.html

[U10] Py：按值排序字典
来源：http://hz.meibo888.top/gthddrabqs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xylfe.cn/gtlzwkfejc.html

[U11] Py：生成器表达式
来源：http://hz.xylfe.cn/gtykemoqif.html

(x * 2 for x in arr)
来源：http://hz.zhiwuduotai.top/gtnjylehsk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shangyingyoupin.top/gtkveirmvc.html

Counter(arr).most_common(3)
来源：http://hz.ydzc1.top/gtgifxmeoj.html

[U13] Py：固定长度队列
来源：http://hz.yonumen.top/gtrpayrgnr.html

deque(maxlen=10)
来源：http://hz.nanxinkj.top/gtjmdgzuki.html

[U14] Py：分组收集到列表
来源：http://hz.cdnleiting.top/gtgzggxuti.html

defaultdict(list)
来源：http://hz.hywenlv.cn/gtlfmmxdve.html

[U15] Py：高精度计时
来源：http://hz.yonumen.top/gtaeddxmcl.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtitxfddeq.html

[U16] Py：命令行参数解析
来源：http://hz.wangshuangyany.cn/gtxwnbvtlu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xuanzx.com/gtpterbiww.html

[U17] Py：初始化日志
来源：http://hz.yuxming.cn/gtydcqdbrg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.svipenyu.cn/gtnzfutgew.html

[U18] Py：预编译正则
来源：http://hz.zhijiandao.cn/gturbxywyw.html

pat = re.compile(r"\d+")
来源：http://hz.vqdsnc.cn/gtooppkcca.html

[U19] Py：正则替换带回调
来源：http://hz.yvedp.cn/gtbahyltwf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gthrsfsxjj.html

[U20] Py：缓存函数结果
来源：http://hz.smart0.xyz/gtinjwenyb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xziqi.cn/gtptceziuc.html

[U21] Py：自定义上下文管理器
来源：http://hz.xziqi.cn/gtcyxopbsg.html

@contextlib.contextmanager
来源：http://hz.sweek.top/gtaahhhiju.html

[U22] Py：矩阵转置
来源：http://hz.jyoumei.cn/gthbddjhvl.html

list(zip(*m))
来源：http://hz.shzxlz.cn/gttlmjvecv.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtslltymfc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtszgblaqh.html

[U24] Py：路径操作
来源：http://hz.dashuyun.cn/gtbsccgsok.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtjwvzgzby.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258888.top/gtmtiuobzx.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gttoiaksjk.html

[U26] Py：并发下载
来源：http://hz.daxiang520.top/gtdivxpkxi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.bjfxy.top/gtnqhyniuz.html

[U27] Py：异步 HTTP
来源：http://hz.xziqi.cn/gtalqclbyt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yongpay.top/gtyhohjewg.html

[U28] Py：类型别名
来源：http://hz.zhiwuduotai.top/gtcewawyyx.html

UserId = int
来源：http://hz.jyoumei.cn/gtutlsleed.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gtcskjabqz.html

@property 与 @x.setter 配合
来源：http://hz.yuanzhike.top/gteuvcxddu.html

[U30] Py：数据类
来源：http://hz.hysaishi.cn/gtolwrpwzt.html

@dataclass(slots=True)
来源：http://hz.yj202588.top/gtgaattopn.html

[U31] Py：单测
来源：http://hz.jinghuilouyu.cn/gtzstwtexs.html

python -m pytest -q
来源：http://hz.wangshuangyany.cn/gtmjbzfcsq.html

[U32] Py：代码格式化
来源：http://hz.hnqzz.top/gtowjumewx.html

ruff format . && ruff check --fix .
来源：http://hz.ywan-chungtsiang.top/gthdsrdaxc.html

[U33] Py：打包发布
来源：http://hz.guannengcc.top/gttxbyfyyd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.gotoacloud.top/gtnusgwfxw.html

[U34] Py：判断编码
来源：http://hz.snrcjt.cn/gtgkinplwe.html

chardet.detect(raw)
来源：http://hz.gaohongyu789.top/gtsowfqhri.html

[U35] Py：发送邮件
来源：http://hz.bjfxy.top/gtexbmfngz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ydjk.org.cn/gtiyxmejzc.html

[U36] Py：定时任务
来源：http://hz.chenjidiqi.icu/gterzaemrz.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhengqikj.top/gtslvncqyr.html

[U37] Py：读写 Excel
来源：http://hz.gogol.net.cn/gtyqtraklu.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtxrviynfr.html

[U38] Py：获取脚本所在目录
来源：http://hz.jlsjyb.cn/gtjmrfbrho.html

Path(__file__).resolve().parent
来源：http://hz.yuxming.cn/gtlpoxsqwy.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtvqgnmtgg.html

sys.stdout.isatty()
来源：http://hz.chenlongwang.top/gtvhoyztch.html

[U40] Py：打印到标准错误
来源：http://hz.cashguo.top/gtlbeienfm.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtghufoiwb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigufen.top/gtgwboayrv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yj20258.top/gtqsdhvaed.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jyoumei.cn/gtfzohtoez.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.haohaochexian.top/gtvcyupbov.html

[U43] PHP：声明命名空间
来源：http://hz.gotoacloud.top/gtbqaakkcj.html

namespace App\Http;
来源：http://hz.andypj.xyz/gtudhszhyo.html

[U44] PHP：开启严格类型
来源：http://hz.yj202588.top/gtojikwspy.html

declare(strict_types=1);
来源：http://hz.52xcode.cn/gtkewqshbl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.gaohongyu789.top/gtjamqegfg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtlrympfsz.html

[U46] PHP：可空类型
来源：http://hz.fengsongda.top/gtecjbqwbk.html

?string $name = null
来源：http://hz.fzhhl.top/gtsbxvehzh.html

[U47] PHP：联合类型
来源：http://hz.yanxiufei.cn/gtpehzexkm.html

int|string $id
来源：http://hz.iojbl.cn/gtglypltwq.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gtgtzgahjf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.daxiang520.top/gtbjexbpww.html

[U49] PHP：只读属性
来源：http://hz.yj20258.top/gtxlcblnnu.html

public readonly string $name
来源：http://hz.ydjk.org.cn/gtghkfhrwn.html

[U50] PHP：构造器属性提升
来源：http://hz.hammf.cn/gtysruvoas.html

public function __construct(private int $id) {}
来源：http://hz.chenzaomai.com/gttdanctlj.html

[U51] PHP：数组解构
来源：http://hz.xinyue.icu/gtdurtyhbn.html

[$a, $b] = $arr;
来源：http://hz.dashuyun.cn/gtztgegbea.html

[U52] PHP：箭头函数
来源：http://hz.jinqigufen.top/gtyfgetrqy.html

$double = fn($x) => $x * 2;
来源：http://hz.feifeiyinyue.top/gtnrwvdqek.html

[U53] PHP：空合并运算符
来源：http://hz.zhijiandao.cn/gturqrxmjw.html

$v = $a ?? $b ?? "default";
来源：http://hz.quarkkingdee.top/gtdoldomke.html

[U54] PHP：空安全调用
来源：http://hz.vqdsnc.cn/gtreoeqnyh.html

$obj?->method()
来源：http://hz.jinqigfzy.top/gtdjoddnry.html

[U55] PHP：match 表达式
来源：http://hz.hnxiangtu.top/gtbxmemdes.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.xziqi.cn/gtodabqbit.html

[U56] PHP：命名参数
来源：http://hz.ydzc1.top/gtyopjwyck.html

f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtdmtcvmzv.html

[U57] PHP：字符串插值
来源：http://hz.xuanzx.com/gtyelldziw.html

"值: {$a}"
来源：http://hz.zhoulong.xyz/gtnzctwslw.html

[U58] PHP：数组三件套
来源：http://hz.wangshuangyany.cn/gthrxydbcz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.aibaodan.cn/gtwgigjtjs.html

[U59] PHP：自定义排序
来源：http://hz.gzhubu.top/gtngiekduv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtjzselxcz.html

[U60] PHP：JSON 编解码
来源：http://hz.ivvv.top/gtnvctgdhj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.gaohongyu789.top/gtwrvlevrh.html


<!-- 参考信息 -->