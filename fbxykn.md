代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtrabrtske.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenzaomai.com/gtenoyhnqj.html

[S40] C++：查找元素
来源：http://hz.xylfe.cn/gtlycymosi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nwbrower.top/gtlmixanri.html

[S41] C++：类与构造函数
来源：http://hz.ydjk.org.cn/gtgwtnxdvj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuanzx.com/gtfyeolubf.html

[S42] C++：继承与虚函数
来源：http://hz.chenzaomai.com/gtniulvhfr.html

class B : public Base { public: void f() override {} };
来源：http://hz.sweek.top/gtbnyfkens.html

[S43] C++：智能指针
来源：http://hz.havefunace.top/gtybganhfh.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhijiandao.cn/gtaoioutlk.html

[S44] C++：引用传参
来源：http://hz.yvedp.cn/gtbhrynbqf.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gthwwwzuic.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtkadtloxn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.9152youxi.cn/gtzlzsgxya.html

[S46] C++：函数模板
来源：http://hz.tianlin.xyz/gtzccuibkc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ywan-chungtsiang.top/gthfgqdiza.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenlongwang.top/gtuqpjwkpr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhengqikj.top/gtuuejrubj.html

[S48] C++：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtcwhzibde.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtjqorxzia.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtbbnibuvc.html

[S49] C++：写文件
来源：http://hz.meibo888.top/gtbcccoqlg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.smart0.xyz/gtrmzftmab.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtjiplelzg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aibaodan.cn/gtkbbfehnf.html

[S51] C++：显式类型转换
来源：http://hz.bjfxy.top/gttaazsyeq.html

static_cast<double>(a) / b
来源：http://hz.yj20258888.top/gtbzrqbvgk.html

[S52] C++：const 与 noexcept
来源：http://hz.cdnleiting.top/gtigbibyrx.html

int size() const noexcept { return n_; }
来源：http://hz.0kj1m.cn/gtfxwvimpi.html

[S53] C++：移动语义
来源：http://hz.snrcjt.cn/gtzboekier.html

std::vector<int> w = std::move(v);
来源：http://hz.cashguo.top/gtptokjydq.html

[S54] C++：异常处理
来源：http://hz.ydzc1.top/gtjihfumje.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuanzx.com/gtwmxmjxqf.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtrnfqhlra.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jyoumei.cn/gtbxwmakea.html

[S56] C++：optional
来源：http://hz.yuxming.cn/gtalqjdttb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.guannengcc.top/gttavdrapa.html

[S57] C++：编译期常量
来源：http://hz.yanxiufei.cn/gtkekcjrop.html

constexpr int N = 10;
来源：http://hz.xziqi.cn/gtbpcznbjb.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtgrnaqmda.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtxrfbxgso.html

[S59] C++：静态断言
来源：http://hz.hfpthk.cn/gtfwayltkx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtvnrwfnbr.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtulmqgsfy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtckitmtnd.html

================================================================================
来源：http://hz.jiagoushi.top/gtpfayjmob.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cucudq.cn/gtchroboag.html

================================================================================
来源：http://hz.xziqi.cn/gtgrahpzru.html

[T01] Kotlin：Hello World
来源：http://hz.tanke756.top/gtjcfpyfle.html

println("Hello")
来源：http://hz.mhx1999.top/gtcndgzbfs.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtxufaayfd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cqqwz.cn/gtqgcsyudt.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gtgevsywaq.html

"值: $b"
来源：http://hz.yuxming.cn/gtmtjvexut.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtobpvhwqf.html

val n: String? = null;  n?.length
来源：http://hz.shzxlz.cn/gtbwhkupnt.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtnhpmmozi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jqgfzy.top/gtqjvaazdb.html

[T06] Kotlin：集合映射
来源：http://hz.guowangkeji.top/gtaoumhzav.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgufenzy.top/gtuyqmrlrj.html

[T07] Kotlin：集合过滤
来源：http://hz.tian-w.cn/gthgmdwalo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shuidangran.top/gtoehyyhme.html

[T08] Kotlin：数据类
来源：http://hz.redwolf501.top/gtlzazfeej.html

data class User(val name: String, val age: Int)
来源：http://hz.jinyuanbaomall.cn/gtnnttmhch.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtwcqmmvep.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgufenzy.top/gtcwwvmlmb.html

[T10] Kotlin：默认参数
来源：http://hz.meibo888.top/gtosojiyqc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shangyingyoupin.top/gtxkhrjzat.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtpsohnutq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.aizwys.cn/gtmiulzlim.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtqafrvpiq.html

val (a, b) = Pair(1, 2)
来源：http://hz.andypj.xyz/gtwrvadreg.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gtaptdqomo.html

val m = mapOf("a" to 1)
来源：http://hz.iojbl.cn/gtfeexlhtu.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtlirmalzp.html

for (i in 1..10) println(i)
来源：http://hz.zhixingplan.top/gtamfqexfw.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtsoqyagoz.html

interface Shape { fun area(): Double }
来源：http://hz.yangfankeji.com/gtcjpmnoud.html

[T16] Swift：Hello World
来源：http://hz.ehwqpu.com/gtbbglskeq.html

print("Hello")
来源：http://hz.cashguo.top/gtnhjldtcl.html

[T17] Swift：变量与常量
来源：http://hz.gzhubu.top/gtxkzjazil.html

var a = 1;  let b = 2
来源：http://hz.zhiwuduotai.top/gtoedptxzh.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangkeji.top/gtrnlvfdwh.html

"值: \(b)"
来源：http://hz.shuidangran.top/gtgpbsovlb.html

[T19] Swift：可选绑定
来源：http://hz.zhengqikj.top/gtolxupibw.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtvkbuvghi.html

[T20] Swift：数组操作
来源：http://hz.zycfv.cn/gtnvqkzpcg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxuanxn.top/gtvycbxpkc.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gtxxftwshv.html

for x in a { print(x) }
来源：http://hz.yuanzhike.top/gttefppaex.html

[T22] Swift：字典
来源：http://hz.hammf.cn/gtozrvxrmq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhixingplan.top/gtqimibnqs.html

[T23] Swift：函数
来源：http://hz.yuanzhike.top/gtwpdummfl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtsltvrmuu.html

[T24] Swift：闭包
来源：http://hz.bjfxy.top/gteobjdymc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtxfzxskoq.html

[T25] Swift：结构体
来源：http://hz.chenlongwang.top/gtkhpeehoj.html

struct P { var x: Int }
来源：http://hz.kuanghao11.cn/gtgzddlzof.html

[T26] Swift：类与重写
来源：http://hz.ybcxt.top/gtrxkfanwi.html

class A: Base { override func f() {} }
来源：http://hz.shzxlz.cn/gtqtgsziuj.html

[T27] Swift：错误处理
来源：http://hz.wangshuangyany.cn/gtrgdxojko.html

do { try f() } catch { print(error) }
来源：http://hz.zdqjudy.top/gteknkyrni.html

[T28] Swift：枚举
来源：http://hz.zycfv.cn/gthnkzafab.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtcebswdef.html

[T29] Swift：guard 提前返回
来源：http://hz.wangdashe.top/gtuxwnmhvg.html

guard let x = opt else { return }
来源：http://hz.gotoacloud.top/gteicirgwo.html

[T30] Swift：协议
来源：http://hz.ywan-chungtsiang.top/gterpbamva.html

protocol Shape { func area() -> Double }
来源：http://hz.dianchejie.cn/gtgbtignug.html

[T31] Lua：Hello World
来源：http://hz.0kj1m.cn/gthtmnfcsh.html

print("Hello")
来源：http://hz.hnqzz.top/gtmdpotceg.html

[T32] Lua：局部变量
来源：http://hz.yuxming.cn/gtresibcxj.html

local a = 1
来源：http://hz.smart0.xyz/gtomzhgpol.html

[T33] Lua：表（数组）
来源：http://hz.dianchejie.cn/gtjwrylcgm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cdnleiting.top/gtxellmzwe.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangtech.top/gtcbtwasxr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nanxuanxn.top/gtatlsqcuc.html

[T35] Lua：字典表
来源：http://hz.tanke756.top/gtpdbewuum.html

local d = { a = 1 };  d.b = 2
来源：http://hz.mhx1999.top/gtpmbjfaeg.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtbwlkzcma.html

function add(a, b) return a + b end
来源：http://hz.ivvv.top/gtcgpzokcq.html

[T37] Lua：字符串拼接
来源：http://hz.yonumen.top/gtogozmweq.html

"a" .. "b"
来源：http://hz.dashuyun.cn/gtwjlwhqsw.html

[T38] Lua：条件
来源：http://hz.jiagoushi.top/gtspxoihzk.html

if x > 0 then print("正") end
来源：http://hz.zhaomingkeji.xyz/gtunxpdpbv.html

[T39] Lua：模式匹配
来源：http://hz.9152youxi.cn/gtjmeexxgu.html

string.find(s, "%d+")
来源：http://hz.jiagoushi.top/gtvozvmzsv.html

[T40] Lua：元表
来源：http://hz.hysaishi.cn/gtquabgmnc.html

setmetatable({}, { __index = base })
来源：http://hz.shanyushiyangkeji.top/gtnxfrtjlc.html

[T41] Perl：Hello World
来源：http://hz.nwbrower.top/gtqugxiptl.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtsjwfmfex.html

[T42] Perl：变量类型
来源：http://hz.ydjk.org.cn/gtzlytltry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cheryme.top/gtcsbvvpny.html

[T43] Perl：字符串插值
来源：http://hz.zhoulong.xyz/gtbupzbtst.html

"值: $a"
来源：http://hz.quarkkingdee.top/gtisjsddxb.html

[T44] Perl：条件
来源：http://hz.zhixingplan.top/gtxcyvkfvf.html

if ($a > 0) { print "正"; }
来源：http://hz.aibaodan.cn/gtjmevgatz.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtxozgzyqn.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtjgzopvkk.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gtxrfzkvlq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zdqjudy.top/gthwenrnrr.html

[T47] Perl：正则捕获
来源：http://hz.tianlin.xyz/gtfzeaaglz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gthhoyskeh.html

[T48] Perl：正则替换
来源：http://hz.jiagoushi.top/gtgxenledm.html

$s =~ s/old/new/g;
来源：http://hz.jqgfzy.top/gtfxsjycgh.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtwvsjetwd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yj202588.top/gtxrxxvtjl.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtzkvnztmv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.meibo888.top/gtqpqukixy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.316326.xyz/gthihabxtg.html

[T51] Scala：Hello World
来源：http://hz.cashguo.top/gthecctwrb.html

println("Hello")
来源：http://hz.jiagoushi.top/gtsvvebtfk.html

[T52] Scala：变量
来源：http://hz.zycfv.cn/gtdjjnnncj.html

val a = 1;  var b = 2
来源：http://hz.pengpengdd.cyou/gtpmqmseer.html

[T53] Scala：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtwrtddqxd.html

s"值: $b"
来源：http://hz.ppjwa.cn/gtmaxsgkpz.html

[T54] Scala：集合映射
来源：http://hz.andypj.xyz/gtjuuiwmih.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.meibo888.top/gtawihsmsz.html

[T55] Scala：集合过滤
来源：http://hz.yvedp.cn/gtqfqouruv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.andypj.xyz/gtbfitesks.html

[T56] Scala：样例类
来源：http://hz.pycfn.com/gtertpozra.html

case class User(name: String, age: Int)
来源：http://hz.guowangkeji.top/gtzlqpcfgt.html

[T57] Scala：模式匹配
来源：http://hz.316326.xyz/gtindaqgqy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jyoumei.cn/gtsemhwsmz.html

[T58] Scala：函数定义
来源：http://hz.kuanghao11.cn/gtapmrjqyg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.feifeiyinyue.top/gtmnkqjedf.html

[T59] Scala：循环
来源：http://hz.yj20258888.top/gtkatdbunl.html

for (i <- 1 to 10) println(i)
来源：http://hz.ppjwa.cn/gtuwpggiij.html

[T60] Scala：折叠
来源：http://hz.mhx1999.top/gtfzfhnini.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.snrcjt.cn/gtqfgceeua.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtydobzobm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtthgxcnhf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtvoljlcai.html

[U01] Py：创建虚拟环境
来源：http://hz.birdmap.top/gtiazptoeh.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.kuanghao11.cn/gtslhgdhvk.html

[U02] Py：导出 / 安装依赖
来源：http://hz.andypj.xyz/gtljooijlv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.shzxlz.cn/gtmmxkfdsy.html

[U03] Py：加载 .env 配置
来源：http://hz.fengsongda.top/gtilrtiuny.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gtoapyodyk.html

[U04] Py：变量调试打印
来源：http://hz.gotoacloud.top/gtbzbyflkg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.meibo888.top/gtfruenupd.html

[U05] Py：列表去重且保序
来源：http://hz.sufxvd.cn/gtonzxehpg.html

list(dict.fromkeys(arr))
来源：http://hz.svipenyu.cn/gtrtnweodf.html

[U06] Py：合并两个字典
来源：http://hz.zhaomingkeji.xyz/gtmtztjpmr.html

{**a, **b}
来源：http://hz.sweek.top/gtvhxwxvpw.html

[U07] Py：反转字典键值
来源：http://hz.kuanghao11.cn/gtcjivifwx.html

{v: k for k, v in d.items()}
来源：http://hz.guowangkeji.top/gtztxutsgc.html

[U08] Py：展平二维列表
来源：http://hz.guowangkeji.top/gtbuxfbunb.html

[y for x in nested for y in x]
来源：http://hz.feifeiyinyue.top/gtxpyvhdex.html

[U09] Py：字典取最大值的键
来源：http://hz.guannengcc.top/gtvyilycpw.html

max(d, key=d.get)
来源：http://hz.xuetiantiany.cn/gtbjzpzkkw.html

[U10] Py：按值排序字典
来源：http://hz.guannengcc.top/gtymdvouom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jyoumei.cn/gtkvivmoxq.html

[U11] Py：生成器表达式
来源：http://hz.aibaodan.cn/gtxobrkeyw.html

(x * 2 for x in arr)
来源：http://hz.zhongyouzk.top/gtvgjeusnt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hywenlv.cn/gtlyefoekq.html

Counter(arr).most_common(3)
来源：http://hz.jqgufenzy.top/gtevoiijlr.html

[U13] Py：固定长度队列
来源：http://hz.52xcode.cn/gtnpgklfev.html

deque(maxlen=10)
来源：http://hz.xinyue.icu/gtjtslzcvn.html

[U14] Py：分组收集到列表
来源：http://hz.zhongyouzk.top/gtcllprwtq.html

defaultdict(list)
来源：http://hz.tianlin.xyz/gtcwmsdwbt.html

[U15] Py：高精度计时
来源：http://hz.chenlongwang.top/gtefdkrlpd.html

t = time.perf_counter()
来源：http://hz.nanxuanxn.top/gtudjtlpwc.html

[U16] Py：命令行参数解析
来源：http://hz.snrcjt.cn/gtcosgwrrc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhengqikj.top/gtngczbhlz.html

[U17] Py：初始化日志
来源：http://hz.chenzaomai.com/gtmrtsmglr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.gotoacloud.top/gtyrtlweso.html

[U18] Py：预编译正则
来源：http://hz.chenlongwang.top/gtfwzuwnpi.html

pat = re.compile(r"\d+")
来源：http://hz.yanxiufei.cn/gtxbnjhtvj.html

[U19] Py：正则替换带回调
来源：http://hz.ivvv.top/gtcldxdwlz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.andypj.xyz/gtejuelonr.html

[U20] Py：缓存函数结果
来源：http://hz.yongpay.top/gtlctpocsb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.feifeiyinyue.top/gtlchixtox.html

[U21] Py：自定义上下文管理器
来源：http://hz.cheryme.top/gtihicggbv.html

@contextlib.contextmanager
来源：http://hz.ywan-chungtsiang.top/gtfimkvwau.html

[U22] Py：矩阵转置
来源：http://hz.bjfxy.top/gtvcjywzng.html

list(zip(*m))
来源：http://hz.wangshuangyany.cn/gtxxmvyabh.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gtmkecygle.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.meibo888.top/gtoficikvg.html

[U24] Py：路径操作
来源：http://hz.chenlongwang.top/gtbuibbibk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.tian-w.cn/gtmmkyonsy.html

[U25] Py：CSV 按字典读
来源：http://hz.xuetiantiany.cn/gtyrhbrpyz.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtewxvzhed.html

[U26] Py：并发下载
来源：http://hz.shangyingyoupin.top/gtbigxspfh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenjidiqi.icu/gtrksiziid.html

[U27] Py：异步 HTTP
来源：http://hz.hongshengwenyu.top/gtvyhuesfn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xuanzx.com/gtabsebims.html

[U28] Py：类型别名
来源：http://hz.hnqzz.top/gtsmmodgej.html

UserId = int
来源：http://hz.yj20258888.top/gtetspvizv.html

[U29] Py：属性校验
来源：http://hz.gotoacloud.top/gtudunrwqf.html

@property 与 @x.setter 配合
来源：http://hz.kuanghao11.cn/gtoscejqga.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtcelsinls.html

@dataclass(slots=True)
来源：http://hz.havefunace.top/gtcgtsuppi.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtjszreone.html

python -m pytest -q
来源：http://hz.birdmap.top/gtavyzehxm.html

[U32] Py：代码格式化
来源：http://hz.yvedp.cn/gtemyikrcm.html

ruff format . && ruff check --fix .
来源：http://hz.zhongyouzk.top/gtufckgohm.html

[U33] Py：打包发布
来源：http://hz.sysykeji.top/gtoycncdms.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.nwbrower.top/gtlnfkdbwn.html

[U34] Py：判断编码
来源：http://hz.zdqjudy.top/gtvkjdqvad.html

chardet.detect(raw)
来源：http://hz.guowangkeji.top/gtpzemgmny.html

[U35] Py：发送邮件
来源：http://hz.zhaomingkeji.xyz/gtwcmrklly.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gotoacloud.top/gtemwivtrv.html

[U36] Py：定时任务
来源：http://hz.gaohongyu789.top/gtvzpfejhw.html

schedule.every(10).minutes.do(job)
来源：http://hz.fengsongda.top/gtwonpvsrj.html

[U37] Py：读写 Excel
来源：http://hz.cqqwz.cn/gtsyvvwxln.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.fzhhl.top/gtpkkmycpe.html

[U38] Py：获取脚本所在目录
来源：http://hz.xylfe.cn/gtohxsbuqk.html

Path(__file__).resolve().parent
来源：http://hz.svipenyu.cn/gtsejqyqyz.html

[U39] Py：判断是否在交互环境
来源：http://hz.yuanzhike.top/gtjhymfcao.html

sys.stdout.isatty()
来源：http://hz.zhixingplan.top/gturwxewms.html

[U40] Py：打印到标准错误
来源：http://hz.cucudq.cn/gtmxovgajc.html

print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtnwttexls.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tianlin.xyz/gtorwpgnkp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sufxvd.cn/gtwxgokxwu.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.mhx1999.top/gtdqnuxrbe.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangkeji.top/gtkvukrqxi.html

[U43] PHP：声明命名空间
来源：http://hz.zhijiandao.cn/gtxjtqgbxh.html

namespace App\Http;
来源：http://hz.shanyushiyangtech.top/gtsxgnwtga.html

[U44] PHP：开启严格类型
来源：http://hz.cdnleiting.top/gtdyhcdgqn.html

declare(strict_types=1);
来源：http://hz.aibaodan.cn/gtitxbzdly.html

[U45] PHP：类型声明与返回类型
来源：http://hz.svipenyu.cn/gttpyaeiop.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtfaxgdgyc.html

[U46] PHP：可空类型
来源：http://hz.yuxming.cn/gtjrajgugm.html

?string $name = null
来源：http://hz.zhengqikj.top/gtcngxnhkv.html

[U47] PHP：联合类型
来源：http://hz.kuanghao11.cn/gtftiorrrd.html

int|string $id
来源：http://hz.yonumen.top/gtqvaryuvo.html

[U48] PHP：纯枚举
来源：http://hz.cqqwz.cn/gtgqlfcmlk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhaomingkeji.xyz/gttwoynaok.html

[U49] PHP：只读属性
来源：http://hz.sxryk.cn/gtmtmypcwh.html

public readonly string $name
来源：http://hz.yj20258.top/gtdbbuhlre.html

[U50] PHP：构造器属性提升
来源：http://hz.cqqwz.cn/gtxiblggkp.html

public function __construct(private int $id) {}
来源：http://hz.xylfe.cn/gtlielmibs.html

[U51] PHP：数组解构
来源：http://hz.snrcjt.cn/gtdyetmxgf.html

[$a, $b] = $arr;
来源：http://hz.chenlongwang.top/gtxfhvpctz.html

[U52] PHP：箭头函数
来源：http://hz.cqqwz.cn/gtquqpexct.html

$double = fn($x) => $x * 2;
来源：http://hz.zhijiandao.cn/gtbfwpwitw.html

[U53] PHP：空合并运算符
来源：http://hz.zhijiandao.cn/gtyxzwivyo.html

$v = $a ?? $b ?? "default";
来源：http://hz.xuanzx.com/gtivuagzne.html

[U54] PHP：空安全调用
来源：http://hz.hnxiangtu.top/gtconfrbeo.html

$obj?->method()
来源：http://hz.hfpthk.cn/gtvcxcmjdv.html

[U55] PHP：match 表达式
来源：http://hz.gogol.net.cn/gtfnfmmfry.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.aizwys.cn/gtwonmdubn.html

[U56] PHP：命名参数
来源：http://hz.birdmap.top/gtmuichyah.html

f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gthajfdvoz.html

[U57] PHP：字符串插值
来源：http://hz.daria6918.cn/gttzxfzexa.html

"值: {$a}"
来源：http://hz.fzhhl.top/gtfujythwq.html

[U58] PHP：数组三件套
来源：http://hz.nanxuanxn.top/gttyjztawo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.0kj1m.cn/gtechlfelj.html

[U59] PHP：自定义排序
来源：http://hz.yueranfly.top/gtvwjmmlqj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtundadawv.html

[U60] PHP：JSON 编解码
来源：http://hz.fengsongda.top/gtgaqacpwy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.andypj.xyz/gtxyubxjph.html

[U61] PHP：正则
来源：http://hz.mhx1999.top/gtbjrkojqs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtnideqqsc.html

[U62] PHP：日期对象
来源：http://hz.jqgfzy.top/gtpxzlinrz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghu66.top/gttayujkmk.html

[U63] PHP：文件读写
来源：http://hz.ydjk.org.cn/gtszhwvpkr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jinyuanbaomall.cn/gtrigdmloy.html

[U64] PHP：目录遍历
来源：http://hz.sxryk.cn/gtfutlpcjd.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hysaishi.cn/gtxmhvzfjo.html


<!-- 参考信息 -->