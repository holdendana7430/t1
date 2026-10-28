代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtofxrdqhk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgufenzy.top/gtktwkqqmd.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gthoazndxp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nwbrower.top/gtoqctunkx.html

[S41] C++：类与构造函数
来源：http://hz.nanxinkj.top/gtopvfgazw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gtiybemrhe.html

[S42] C++：继承与虚函数
来源：http://hz.yj20258888.top/gtykmbtlpw.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtxwdyxsac.html

[S43] C++：智能指针
来源：http://hz.jyoumei.cn/gtzshzwjfx.html

auto p = std::make_unique<int>(5);
来源：http://hz.cqqwz.cn/gtodicsxux.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtclozobhb.html

void inc(int &x) { ++x; }
来源：http://hz.chenlongwang.top/gtzwdqiehl.html

[S45] C++：lambda
来源：http://hz.jqgufenzy.top/gtoozpwtsg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.haohaochexian.top/gtancfrmqw.html

[S46] C++：函数模板
来源：http://hz.chenjidiqi.icu/gtwbnkhxcs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.dianchejie.cn/gtojetxque.html

[S47] C++：结构化绑定遍历
来源：http://hz.shanyushiyangtech.top/gtfxvwzwrw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangshuangyany.cn/gtcqqyrkmu.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtmenpsjqe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sxryk.cn/gtxmkvyjck.html

while (std::getline(in, line)) { }
来源：http://hz.jinqigfzy.top/gtwecnhegb.html

[S49] C++：写文件
来源：http://hz.xuanzx.com/gtidnnhnhz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yueranfly.top/gtyqecvqkj.html

[S50] C++：格式化数字
来源：http://hz.xuanzx.com/gtbfcvlojt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtaehmdlhj.html

[S51] C++：显式类型转换
来源：http://hz.havefunace.top/gtgtlxmqgq.html

static_cast<double>(a) / b
来源：http://hz.hysaishi.cn/gtzudsszwo.html

[S52] C++：const 与 noexcept
来源：http://hz.cashguo.top/gtsiqcgoib.html

int size() const noexcept { return n_; }
来源：http://hz.vqdsnc.cn/gtmmanetxj.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtempzlbzg.html

std::vector<int> w = std::move(v);
来源：http://hz.jiagoushi.top/gtbjfzotcj.html

[S54] C++：异常处理
来源：http://hz.sysykeji.top/gthrsnmfgy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gtyyuzrnfy.html

[S55] C++：结构化绑定
来源：http://hz.chenzaomai.com/gtlvkntxtc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtacjgwbau.html

[S56] C++：optional
来源：http://hz.tianlin.xyz/gtwxqjzkgt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.redwolf501.top/gtrpispzgf.html

[S57] C++：编译期常量
来源：http://hz.sysykeji.top/gtbtfahesg.html

constexpr int N = 10;
来源：http://hz.tian-w.cn/gtymgkwpjk.html

[S58] C++：命名空间
来源：http://hz.wangshuangyany.cn/gtpwsnuhay.html

namespace ns { int f() { return 1; } }
来源：http://hz.yanxiufei.cn/gtgjpzqohx.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gthlffbtjy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yangfankeji.com/gtqicrlnab.html

[S60] C++：遍历并删除元素
来源：http://hz.ehwqpu.com/gticvwgwwq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hfpthk.cn/gtmispnmku.html

================================================================================
来源：http://hz.tanke756.top/gtewlkovby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtjrbyrvwf.html

================================================================================
来源：http://hz.ydzc1.top/gtatpsiaiq.html

[T01] Kotlin：Hello World
来源：http://hz.dashuyun.cn/gtfholnvqh.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtnjvbdzfz.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtbkcwwxxw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenlongwang.top/gtcjcjvpea.html

[T03] Kotlin：字符串模板
来源：http://hz.aizwys.cn/gtzybowbdw.html

"值: $b"
来源：http://hz.meibo888.top/gtxnvshlpf.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtbifoncpn.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtgqngjoym.html

[T05] Kotlin：when 表达式
来源：http://hz.fengsongda.top/gtnhkswnfe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cdnleiting.top/gtqavekspn.html

[T06] Kotlin：集合映射
来源：http://hz.chenjidiqi.icu/gtrxhsklfl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtixqgzhbw.html

[T07] Kotlin：集合过滤
来源：http://hz.yuxming.cn/gtwlzwuamv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cashguo.top/gtzfzmbnik.html

[T08] Kotlin：数据类
来源：http://hz.yuanzhike.top/gtwcsffsvh.html

data class User(val name: String, val age: Int)
来源：http://hz.9152youxi.cn/gtssjciefn.html

[T09] Kotlin：扩展函数
来源：http://hz.hongshengwenyu.top/gtkmeicdpw.html

fun String.exclaim() = this + "!"
来源：http://hz.birdmap.top/gtiopdeobc.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtpyqiqlld.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtanxsesbi.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtwycsgiub.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xingfuxueyuan.xyz/gtrgxvonra.html

[T12] Kotlin：解构声明
来源：http://hz.andypj.xyz/gtqbhhxhpg.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtvdwdkbyn.html

[T13] Kotlin：只读 Map
来源：http://hz.ydjk.org.cn/gtncayyicv.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtehnkfcmw.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtuevgglel.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gthczbwgyh.html

[T15] Kotlin：接口
来源：http://hz.c1oappe.top/gtnifnovae.html

interface Shape { fun area(): Double }
来源：http://hz.nanxuanxn.top/gtorzjvgjb.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtljewecky.html

print("Hello")
来源：http://hz.svipenyu.cn/gtlqhivitr.html

[T17] Swift：变量与常量
来源：http://hz.kuanghao11.cn/gtntsmygqf.html

var a = 1;  let b = 2
来源：http://hz.chenzaomai.com/gtyjaqcyjc.html

[T18] Swift：字符串插值
来源：http://hz.yj202588.top/gtxeozvywz.html

"值: \(b)"
来源：http://hz.pycfn.com/gthpkcihii.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtpbcjgxzf.html

if let n = opt { print(n) }
来源：http://hz.9152youxi.cn/gtidrwdtca.html

[T20] Swift：数组操作
来源：http://hz.ivvv.top/gtrfjcbdae.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gotoacloud.top/gtptwekmoz.html

[T21] Swift：遍历
来源：http://hz.yj20258888.top/gtjqsmrgcr.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtbjfywero.html

[T22] Swift：字典
来源：http://hz.meibo888.top/gtmhdbiega.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtkxuarumh.html

[T23] Swift：函数
来源：http://hz.cdnleiting.top/gtdcohpdfr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.c1oappe.top/gtftdhwzcb.html

[T24] Swift：闭包
来源：http://hz.xuetiantiany.cn/gtntfjjhzp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtlrlzrpeu.html

[T25] Swift：结构体
来源：http://hz.yangfankeji.com/gtplhlaeld.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtsfvtumob.html

[T26] Swift：类与重写
来源：http://hz.shangyingyoupin.top/gtvrbhgaiz.html

class A: Base { override func f() {} }
来源：http://hz.mhx1999.top/gtyfiheaff.html

[T27] Swift：错误处理
来源：http://hz.guannengcc.top/gtwkdnekwi.html

do { try f() } catch { print(error) }
来源：http://hz.havefunace.top/gtpyoqzgvs.html

[T28] Swift：枚举
来源：http://hz.redwolf501.top/gtatnboseo.html

enum Color { case red, green }
来源：http://hz.cucudq.cn/gtpqnpfgdi.html

[T29] Swift：guard 提前返回
来源：http://hz.ydjk.org.cn/gtwkxmlnuo.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtfccunsid.html

[T30] Swift：协议
来源：http://hz.bjfxy.top/gtczepdmti.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtyplzlajx.html

[T31] Lua：Hello World
来源：http://hz.jiagoushi.top/gtmlyfswxi.html

print("Hello")
来源：http://hz.sweek.top/gtvasjbfcb.html

[T32] Lua：局部变量
来源：http://hz.iojbl.cn/gtvhvbrtvp.html

local a = 1
来源：http://hz.zhengqikj.top/gtsybqjkgd.html

[T33] Lua：表（数组）
来源：http://hz.sweek.top/gtcmesuoal.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yanxiufei.cn/gtlphrumya.html

[T34] Lua：遍历表
来源：http://hz.vqdsnc.cn/gtdlkvibwl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.svipenyu.cn/gtovzqtiph.html

[T35] Lua：字典表
来源：http://hz.nanxuanxn.top/gthjczmuhv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.iojbl.cn/gtfajichll.html

[T36] Lua：函数
来源：http://hz.yonumen.top/gtlgwjrtqu.html

function add(a, b) return a + b end
来源：http://hz.316326.xyz/gtoxcdcodz.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtlmisjvmg.html

"a" .. "b"
来源：http://hz.yueranfly.top/gtqovobbjv.html

[T38] Lua：条件
来源：http://hz.jinqigfzy.top/gtntulnqgh.html

if x > 0 then print("正") end
来源：http://hz.jianghu66.top/gtyxtoazzi.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtlarqhhwc.html

string.find(s, "%d+")
来源：http://hz.sxryk.cn/gtdedhehtz.html

[T40] Lua：元表
来源：http://hz.smart0.xyz/gtckfmwsoa.html

setmetatable({}, { __index = base })
来源：http://hz.xuanzx.com/gthmgvjoxn.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangkeji.top/gtxxtgbdmt.html

print "Hello\n";
来源：http://hz.zhiwuduotai.top/gtppoornel.html

[T42] Perl：变量类型
来源：http://hz.yj202588.top/gtaknttuuk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.haohaochexian.top/gtgwsmcgcy.html

[T43] Perl：字符串插值
来源：http://hz.nanxuanxn.top/gtesnrqapj.html

"值: $a"
来源：http://hz.pycfn.com/gtatpbqeks.html

[T44] Perl：条件
来源：http://hz.xingfuxueyuan.xyz/gtfjnqhroq.html

if ($a > 0) { print "正"; }
来源：http://hz.fengsongda.top/gtavzqmsea.html

[T45] Perl：数组遍历
来源：http://hz.zhijiandao.cn/gthnrtxlgh.html

for my $x (@arr) { print $x; }
来源：http://hz.zycfv.cn/gttmiezytp.html

[T46] Perl：哈希操作
来源：http://hz.hywenlv.cn/gtsvuopwne.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cucudq.cn/gtrulovudu.html

[T47] Perl：正则捕获
来源：http://hz.xuetiantiany.cn/gtolxxcrrb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yj20258888.top/gtjzdutirw.html

[T48] Perl：正则替换
来源：http://hz.hammf.cn/gtqzrmruov.html

$s =~ s/old/new/g;
来源：http://hz.hammf.cn/gtfgpuaugb.html

[T49] Perl：函数
来源：http://hz.fzhhl.top/gtgcmehoya.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.dashuyun.cn/gtspciwwcp.html

[T50] Perl：逐行读文件
来源：http://hz.yuanzhike.top/gtacduuiiz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.daria6918.cn/gtprhmzgti.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.mhx1999.top/gtblldvjrw.html

[T51] Scala：Hello World
来源：http://hz.quarkkingdee.top/gtyszmofui.html

println("Hello")
来源：http://hz.nanxinkj.top/gtikutgqcw.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtqtlldfon.html

val a = 1;  var b = 2
来源：http://hz.hysaishi.cn/gtdsowsqaf.html

[T53] Scala：字符串插值
来源：http://hz.aizwys.cn/gtjqhggjdu.html

s"值: $b"
来源：http://hz.kuanghao11.cn/gtivjvkmlc.html

[T54] Scala：集合映射
来源：http://hz.gzhubu.top/gtpdfeckpx.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xuetiantiany.cn/gtxcwayrun.html

[T55] Scala：集合过滤
来源：http://hz.chenjidiqi.icu/gtpvexrhvo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.chenzaomai.com/gtstjbffcq.html

[T56] Scala：样例类
来源：http://hz.xylfe.cn/gtyqabfvxv.html

case class User(name: String, age: Int)
来源：http://hz.aibaodan.cn/gtfizzrtqi.html

[T57] Scala：模式匹配
来源：http://hz.guannengcc.top/gtbqzukkvb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhengqikj.top/gtddunirju.html

[T58] Scala：函数定义
来源：http://hz.hfpthk.cn/gtpgbnvswa.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj20258888.top/gtobcjfywv.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtgkvpunzk.html

for (i <- 1 to 10) println(i)
来源：http://hz.tanke756.top/gtlzbwcoqj.html

[T60] Scala：折叠
来源：http://hz.xinyue.icu/gtnkenvlpm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgufenzy.top/gtzntpisbb.html

================================================================================
来源：http://hz.iojbl.cn/gtrzpseuuc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hfpthk.cn/gtqojnwjjn.html

================================================================================
来源：http://hz.chenlongwang.top/gtniynnjmy.html

[U01] Py：创建虚拟环境
来源：http://hz.sweek.top/gtpzqogyhe.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aibaodan.cn/gtnaklxrvw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.shanyushiyangtech.top/gtrvvmjpqj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigufen.top/gtmqdaddks.html

[U03] Py：加载 .env 配置
来源：http://hz.nanxuanxn.top/gtczuyaprk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xinyue.icu/gtiwoyznwn.html

[U04] Py：变量调试打印
来源：http://hz.xuanzx.com/gtevjstckx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.0kj1m.cn/gtcxodhcmq.html

[U05] Py：列表去重且保序
来源：http://hz.c1oappe.top/gtzqvzcgfu.html

list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtthynotwa.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gtzqugdwyk.html

{**a, **b}
来源：http://hz.ywan-chungtsiang.top/gtexsjtghl.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtfzjmqdjl.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gtcwfhpsfg.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gtzgmomsvo.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtpnkmeswv.html

[U09] Py：字典取最大值的键
来源：http://hz.bjfxy.top/gtomvyuqdn.html

max(d, key=d.get)
来源：http://hz.ivvv.top/gtzrqrwrrz.html

[U10] Py：按值排序字典
来源：http://hz.cdnleiting.top/gtevybarns.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.kuanghao11.cn/gtfdobdcmc.html

[U11] Py：生成器表达式
来源：http://hz.daria6918.cn/gtsaorqxzz.html

(x * 2 for x in arr)
来源：http://hz.hnxiangtu.top/gtnxflwxhb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gtglkcjmhw.html

Counter(arr).most_common(3)
来源：http://hz.yj202588.top/gtrywtidko.html

[U13] Py：固定长度队列
来源：http://hz.chenjidiqi.icu/gtsewhjefj.html

deque(maxlen=10)
来源：http://hz.xuanzx.com/gtlsprtwos.html

[U14] Py：分组收集到列表
来源：http://hz.pengpengdd.cyou/gtyqcqrqle.html

defaultdict(list)
来源：http://hz.xziqi.cn/gtxuhhtlrn.html

[U15] Py：高精度计时
来源：http://hz.hongshengwenyu.top/gtljcfkwrh.html

t = time.perf_counter()
来源：http://hz.cashguo.top/gtkkrgnsyb.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gtiwdioqma.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.feifeiyinyue.top/gtbxoauhkk.html

[U17] Py：初始化日志
来源：http://hz.xuetiantiany.cn/gteiyeomim.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cqqwz.cn/gtusmyxbqr.html

[U18] Py：预编译正则
来源：http://hz.zhaomingkeji.xyz/gtxronsugd.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtiqnmfezw.html

[U19] Py：正则替换带回调
来源：http://hz.ppjwa.cn/gtqwvkpwbi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cqqwz.cn/gtauyggmbn.html

[U20] Py：缓存函数结果
来源：http://hz.dianchejie.cn/gtomibjffk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hongshengwenyu.top/gtuurhahzt.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinyuanbaomall.cn/gteyrnvjfy.html

@contextlib.contextmanager
来源：http://hz.nanxinkj.top/gtlviaqmfp.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtnjjndztv.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtqmyltgto.html

[U23] Py：分块读取大文件
来源：http://hz.hywenlv.cn/gtdzvwgtmn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xuanzx.com/gtyzijnvrt.html

[U24] Py：路径操作
来源：http://hz.vqdsnc.cn/gtpjxsigeo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigfzy.top/gtsxtllzsc.html

[U25] Py：CSV 按字典读
来源：http://hz.zhoulong.xyz/gtsmgsvzmc.html

csv.DictReader(f)
来源：http://hz.ppjwa.cn/gttcqsoczi.html

[U26] Py：并发下载
来源：http://hz.hammf.cn/gtskscdwrt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hysaishi.cn/gtwuphmewl.html

[U27] Py：异步 HTTP
来源：http://hz.svipenyu.cn/gteffxukgi.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.wangshuangyany.cn/gtvbnvsdka.html

[U28] Py：类型别名
来源：http://hz.cucudq.cn/gtfnygxoma.html

UserId = int
来源：http://hz.ydzc1.top/gtoxionxpc.html

[U29] Py：属性校验
来源：http://hz.nanxinkj.top/gtkvmnegya.html

@property 与 @x.setter 配合
来源：http://hz.bjfxy.top/gtdrnjikem.html

[U30] Py：数据类
来源：http://hz.ybcxt.top/gtjapuroch.html

@dataclass(slots=True)
来源：http://hz.gogol.net.cn/gtthqbpjkr.html

[U31] Py：单测
来源：http://hz.yonumen.top/gtdexjelej.html

python -m pytest -q
来源：http://hz.snrcjt.cn/gtjtkxvyey.html

[U32] Py：代码格式化
来源：http://hz.ywan-chungtsiang.top/gtheykoeut.html

ruff format . && ruff check --fix .
来源：http://hz.52xcode.cn/gtcgypuiek.html

[U33] Py：打包发布
来源：http://hz.yanxiufei.cn/gtuwrqqmsp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shzxlz.cn/gtqmmdlywz.html

[U34] Py：判断编码
来源：http://hz.9152youxi.cn/gtpeuretti.html

chardet.detect(raw)
来源：http://hz.ywan-chungtsiang.top/gtupvzujoc.html

[U35] Py：发送邮件
来源：http://hz.meibo888.top/gtgvfpkpvv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hfpthk.cn/gtymherlgc.html

[U36] Py：定时任务
来源：http://hz.jiagoushi.top/gtcjyvubqj.html

schedule.every(10).minutes.do(job)
来源：http://hz.jqgfzy.top/gtmgzuwobv.html

[U37] Py：读写 Excel
来源：http://hz.chenzaomai.com/gtqinwwbxr.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xinyue.icu/gtvystjreu.html

[U38] Py：获取脚本所在目录
来源：http://hz.ywan-chungtsiang.top/gtbvyyioql.html

Path(__file__).resolve().parent
来源：http://hz.yj20258.top/gtkgtscpnv.html

[U39] Py：判断是否在交互环境
来源：http://hz.hysaishi.cn/gtmjhfarok.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtrfvjdtxa.html

[U40] Py：打印到标准错误
来源：http://hz.jlsjyb.cn/gtczosjfan.html

print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gttbwsgjpt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zycfv.cn/gtqxryfdfm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.316326.xyz/gtoejdjmjq.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xylfe.cn/gtlkrillzl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.9152youxi.cn/gtfkcweyyu.html

[U43] PHP：声明命名空间
来源：http://hz.yuxming.cn/gtrgedgztq.html

namespace App\Http;
来源：http://hz.nanxinkj.top/gtxdfqlvfp.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gthnynkzat.html

declare(strict_types=1);
来源：http://hz.feifeiyinyue.top/gtsexutpxf.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtwtishbso.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtuvwojkax.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtudmyndwu.html

?string $name = null
来源：http://hz.mhx1999.top/gtrtbxhnig.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtkrgsqiwp.html

int|string $id
来源：http://hz.sweek.top/gtyvhdrrxs.html

[U48] PHP：纯枚举
来源：http://hz.hywenlv.cn/gtnsfypiew.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtoqreeuhn.html

[U49] PHP：只读属性
来源：http://hz.hysaishi.cn/gtzwhobczf.html

public readonly string $name
来源：http://hz.nwbrower.top/gtihpbtocz.html

[U50] PHP：构造器属性提升
来源：http://hz.tian-w.cn/gttjbkrcwn.html

public function __construct(private int $id) {}
来源：http://hz.xziqi.cn/gtcidrcgxu.html

[U51] PHP：数组解构
来源：http://hz.zhijiandao.cn/gtwjlqfpwk.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtwkgaxele.html

[U52] PHP：箭头函数
来源：http://hz.ppjwa.cn/gtvuoerdew.html

$double = fn($x) => $x * 2;
来源：http://hz.shanyushiyangtech.top/gtqjxbeelc.html

[U53] PHP：空合并运算符
来源：http://hz.quarkkingdee.top/gtovpuzjob.html

$v = $a ?? $b ?? "default";
来源：http://hz.zhaomingkeji.xyz/gtjysmfakk.html

[U54] PHP：空安全调用
来源：http://hz.chenzaomai.com/gtrzbpitgh.html

$obj?->method()
来源：http://hz.jinyuanbaomall.cn/gtiqtsjhey.html

[U55] PHP：match 表达式
来源：http://hz.shuidangran.top/gtaxupegcw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhengqikj.top/gtpdaxoqxu.html

[U56] PHP：命名参数
来源：http://hz.jyoumei.cn/gtghtaeejn.html

f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtlliexsky.html

[U57] PHP：字符串插值
来源：http://hz.pengpengdd.cyou/gtunuypqnj.html

"值: {$a}"
来源：http://hz.zhaomingkeji.xyz/gtmlpvqyaw.html

[U58] PHP：数组三件套
来源：http://hz.cqqwz.cn/gtlahiofzn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hammf.cn/gtpfkvnrey.html

[U59] PHP：自定义排序
来源：http://hz.zhixingplan.top/gtfgjjnwbq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtzquymxwe.html

[U60] PHP：JSON 编解码
来源：http://hz.ivvv.top/gtiuhwiqmu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinyuanbaomall.cn/gteannajco.html

[U61] PHP：正则
来源：http://hz.guannengcc.top/gtaddabfoq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gthbzyheqv.html

[U62] PHP：日期对象
来源：http://hz.pengpengdd.cyou/gtgkgwxwuf.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cashguo.top/gtvbggqupu.html

[U63] PHP：文件读写
来源：http://hz.wangshuangyany.cn/gtukggfpja.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.zdqjudy.top/gtnpvirhms.html

[U64] PHP：目录遍历
来源：http://hz.wangdashe.top/gtyodlzxrn.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tanke756.top/gtnywmoigg.html


<!-- 参考信息 -->