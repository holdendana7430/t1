代发 wailian999

[S45] C++：lambda
来源：http://hz.andypj.xyz/gtlbqydfzz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sweek.top/gtcnxocfvd.html

[S46] C++：函数模板
来源：http://hz.jinghuilouyu.cn/gthyofdxvh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.mhx1999.top/gthphykzov.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gtqtfinpvp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.dianchejie.cn/gtrgbqnpzc.html

[S48] C++：逐行读文件
来源：http://hz.bjfxy.top/gtnuxoauvo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sufxvd.cn/gtextyurvf.html

while (std::getline(in, line)) { }
来源：http://hz.shuidangran.top/gtvmfustfc.html

[S49] C++：写文件
来源：http://hz.zdqjudy.top/gtcncbaxkf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gtnzjssqzf.html

[S50] C++：格式化数字
来源：http://hz.jlsjyb.cn/gtibiinjuq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtlbbpcjkx.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtlajzztfq.html

static_cast<double>(a) / b
来源：http://hz.hywenlv.cn/gtgkwdcbuw.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtuynnyoqr.html

int size() const noexcept { return n_; }
来源：http://hz.hysaishi.cn/gtkmhkkdsg.html

[S53] C++：移动语义
来源：http://hz.zhijiandao.cn/gtrubymlbp.html

std::vector<int> w = std::move(v);
来源：http://hz.wangdashe.top/gtopwltxde.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtdriokuav.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cashguo.top/gtndearsgm.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtfelejtzi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pengpengdd.cyou/gtimijrkov.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtqkdtmlts.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinyuanbaomall.cn/gtebawjepu.html

[S57] C++：编译期常量
来源：http://hz.jiagoushi.top/gtyfvwzvbi.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtdfdyjrae.html

[S58] C++：命名空间
来源：http://hz.fengsongda.top/gtfuywzfuu.html

namespace ns { int f() { return 1; } }
来源：http://hz.gzhubu.top/gtuociyelk.html

[S59] C++：静态断言
来源：http://hz.zhengqikj.top/gtopwrcdlt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gzhubu.top/gtpadjxqoa.html

[S60] C++：遍历并删除元素
来源：http://hz.zhixingplan.top/gtkbcfxbci.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtruoohiop.html

================================================================================
来源：http://hz.smart0.xyz/gttayrahlk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.havefunace.top/gtxmycqlrm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtryeyacxx.html

[T01] Kotlin：Hello World
来源：http://hz.feifeiyinyue.top/gtuudqpeem.html

println("Hello")
来源：http://hz.hywenlv.cn/gtkgbkmbnk.html

[T02] Kotlin：变量
来源：http://hz.ydjk.org.cn/gtrwkphody.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dianchejie.cn/gtcvddqzrf.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gtmhyjojtj.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtnacwwbnt.html

[T04] Kotlin：空安全
来源：http://hz.quarkkingdee.top/gtbwhibexv.html

val n: String? = null;  n?.length
来源：http://hz.jqgfzy.top/gtwhwruixy.html

[T05] Kotlin：when 表达式
来源：http://hz.tianlin.xyz/gtnqxeljae.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nwbrower.top/gtpasrgmmp.html

[T06] Kotlin：集合映射
来源：http://hz.jlsjyb.cn/gthltqwvka.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sweek.top/gtfxkyiqqj.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gthaclsyht.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.52xcode.cn/gtmeqnlnvq.html

[T08] Kotlin：数据类
来源：http://hz.c1oappe.top/gteqastqwu.html

data class User(val name: String, val age: Int)
来源：http://hz.cashguo.top/gtkmydlstx.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgufenzy.top/gtnftudtej.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtciubqpeq.html

[T10] Kotlin：默认参数
来源：http://hz.yonumen.top/gtvbanavcf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhengqikj.top/gtkvdajreb.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtelucymws.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.havefunace.top/gtxhqgfhqn.html

[T12] Kotlin：解构声明
来源：http://hz.ehwqpu.com/gttrnseoqu.html

val (a, b) = Pair(1, 2)
来源：http://hz.wangshuangyany.cn/gtumjrgsnd.html

[T13] Kotlin：只读 Map
来源：http://hz.yuanzhike.top/gtenohchkk.html

val m = mapOf("a" to 1)
来源：http://hz.daria6918.cn/gteenfpuxq.html

[T14] Kotlin：循环
来源：http://hz.jianghu66.top/gtwhmnuaka.html

for (i in 1..10) println(i)
来源：http://hz.hongshengwenyu.top/gtmknaqkiu.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gthmjjnecc.html

interface Shape { fun area(): Double }
来源：http://hz.zdqjudy.top/gtjlesmghb.html

[T16] Swift：Hello World
来源：http://hz.haohaochexian.top/gttcfkqxgw.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtoblxfjbk.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gtabrjclpt.html

var a = 1;  let b = 2
来源：http://hz.ybcxt.top/gtvvfsmhsi.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtiwzakaec.html

"值: \(b)"
来源：http://hz.ivvv.top/gtslucqpso.html

[T19] Swift：可选绑定
来源：http://hz.cucudq.cn/gtcponglvy.html

if let n = opt { print(n) }
来源：http://hz.daxiang520.top/gtxtjaqbca.html

[T20] Swift：数组操作
来源：http://hz.hongshengwenyu.top/gtshlbygeu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.vqdsnc.cn/gtlewcuasm.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtymdfsgkm.html

for x in a { print(x) }
来源：http://hz.hammf.cn/gtowkiethb.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtgtbduxnp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yueranfly.top/gtykirggid.html

[T23] Swift：函数
来源：http://hz.hongshengwenyu.top/gtycfjwjmw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhengqikj.top/gtacbhifgd.html

[T24] Swift：闭包
来源：http://hz.chenjidiqi.icu/gtifvpgjpv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.havefunace.top/gtjawfkzhc.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtxmqmuxtm.html

struct P { var x: Int }
来源：http://hz.havefunace.top/gtvxsmqleg.html

[T26] Swift：类与重写
来源：http://hz.sysykeji.top/gtyeragmqd.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtpwgbhybe.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtxmseilus.html

do { try f() } catch { print(error) }
来源：http://hz.zdqjudy.top/gtkuscbgcu.html

[T28] Swift：枚举
来源：http://hz.nwbrower.top/gtxbceuoli.html

enum Color { case red, green }
来源：http://hz.zhixingplan.top/gtjzhjitww.html

[T29] Swift：guard 提前返回
来源：http://hz.dianchejie.cn/gtvrnsyljh.html

guard let x = opt else { return }
来源：http://hz.sxryk.cn/gtdlgmnvdk.html

[T30] Swift：协议
来源：http://hz.hnqzz.top/gtquhglkdx.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtdvntozhh.html

[T31] Lua：Hello World
来源：http://hz.xuanzx.com/gtaijpbryr.html

print("Hello")
来源：http://hz.zhengqikj.top/gtglrxsltt.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtqbieuugs.html

local a = 1
来源：http://hz.nanxuanxn.top/gtpstilgcb.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gtejhjybmv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yanxiufei.cn/gtlnarqmbx.html

[T34] Lua：遍历表
来源：http://hz.yj20258.top/gtajvzrnnk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.nwbrower.top/gtdywncjsh.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtabagpbwg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj202588.top/gtotaukzqh.html

[T36] Lua：函数
来源：http://hz.yanxiufei.cn/gtjoobpguy.html

function add(a, b) return a + b end
来源：http://hz.hnqzz.top/gtafiyevcb.html

[T37] Lua：字符串拼接
来源：http://hz.vqdsnc.cn/gtyvwmprvg.html

"a" .. "b"
来源：http://hz.shangyingyoupin.top/gtpsokcvmb.html

[T38] Lua：条件
来源：http://hz.ywan-chungtsiang.top/gtzenbpyfy.html

if x > 0 then print("正") end
来源：http://hz.yangfankeji.com/gtnbridcri.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtvozohxpp.html

string.find(s, "%d+")
来源：http://hz.ehwqpu.com/gtgxzwxreo.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gtmsolpwan.html

setmetatable({}, { __index = base })
来源：http://hz.zycfv.cn/gtzmhykoyd.html

[T41] Perl：Hello World
来源：http://hz.ybcxt.top/gtxcrzvjap.html

print "Hello\n";
来源：http://hz.hammf.cn/gtkelgxbcp.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtzicavkpu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.quarkkingdee.top/gtcexndoaz.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangkeji.top/gttrzwlfmm.html

"值: $a"
来源：http://hz.shuidangran.top/gtloqtxtxa.html

[T44] Perl：条件
来源：http://hz.cqqwz.cn/gtwsfnytlt.html

if ($a > 0) { print "正"; }
来源：http://hz.tianlin.xyz/gtnkgiallg.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtmjrqqhqz.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtiucyzylv.html

[T46] Perl：哈希操作
来源：http://hz.aibaodan.cn/gtqsbumkns.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hammf.cn/gtyjtlqyze.html

[T47] Perl：正则捕获
来源：http://hz.ywan-chungtsiang.top/gttvfxehbz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gzhubu.top/gtuzoakerq.html

[T48] Perl：正则替换
来源：http://hz.tianlin.xyz/gtwapogwza.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtcucwkvvg.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gtzmvoludz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shangyingyoupin.top/gtnbehltzd.html

[T50] Perl：逐行读文件
来源：http://hz.dashuyun.cn/gtovsukoxq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtwlzbctrn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtqmbjyqug.html

[T51] Scala：Hello World
来源：http://hz.haohaochexian.top/gtdemeidke.html

println("Hello")
来源：http://hz.haohaochexian.top/gtsoejhjap.html

[T52] Scala：变量
来源：http://hz.jinghuilouyu.cn/gtkpirvjgg.html

val a = 1;  var b = 2
来源：http://hz.wangshuangyany.cn/gtxrqxfrrh.html

[T53] Scala：字符串插值
来源：http://hz.vqdsnc.cn/gtieijuvel.html

s"值: $b"
来源：http://hz.fzhhl.top/gtxptladnl.html

[T54] Scala：集合映射
来源：http://hz.cashguo.top/gtcsmjcwbb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.redwolf501.top/gtzkbpecwl.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtzkumxnqt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gzhubu.top/gtdgeioexg.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtwengfqfd.html

case class User(name: String, age: Int)
来源：http://hz.feifeiyinyue.top/gthtruhhmd.html

[T57] Scala：模式匹配
来源：http://hz.hnxiangtu.top/gtmkadmisb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.sweek.top/gtfgdniled.html

[T58] Scala：函数定义
来源：http://hz.xinyue.icu/gtjctrloex.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenzaomai.com/gthaynhemy.html

[T59] Scala：循环
来源：http://hz.tanke756.top/gttarputwl.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtstbtsqbb.html

[T60] Scala：折叠
来源：http://hz.jinqigufen.top/gtnyqxyoeh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtzqhbynct.html

================================================================================
来源：http://hz.jinqigufen.top/gtecvyrafj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtemmvnuah.html

================================================================================
来源：http://hz.hysaishi.cn/gtrptrafyw.html

[U01] Py：创建虚拟环境
来源：http://hz.nanxuanxn.top/gtpwrexahl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sysykeji.top/gtuekugwle.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jlsjyb.cn/gtmoqvyrwm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gogol.net.cn/gtiryvrpqw.html

[U03] Py：加载 .env 配置
来源：http://hz.xinyue.icu/gtyrobymzn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yonumen.top/gtujzeerct.html

[U04] Py：变量调试打印
来源：http://hz.hongshengwenyu.top/gtxqmjsrlj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtnjaalstb.html

[U05] Py：列表去重且保序
来源：http://hz.cucudq.cn/gtqkulrnzg.html

list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtuwuiwaxu.html

[U06] Py：合并两个字典
来源：http://hz.fengsongda.top/gtyxqiqkeo.html

{**a, **b}
来源：http://hz.hfpthk.cn/gtcntvaxfy.html

[U07] Py：反转字典键值
来源：http://hz.pycfn.com/gtkeyrrmfp.html

{v: k for k, v in d.items()}
来源：http://hz.sysykeji.top/gtsgmjpbnm.html

[U08] Py：展平二维列表
来源：http://hz.jinqigfzy.top/gtrmkiajvn.html

[y for x in nested for y in x]
来源：http://hz.yj20258.top/gtwcipmoys.html

[U09] Py：字典取最大值的键
来源：http://hz.zhijiandao.cn/gtjhqnwcmo.html

max(d, key=d.get)
来源：http://hz.yj20258888.top/gtmjryncvh.html

[U10] Py：按值排序字典
来源：http://hz.hnqzz.top/gtxnwssimh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ydzc1.top/gtzgcrieag.html

[U11] Py：生成器表达式
来源：http://hz.xylfe.cn/gtiolsjrsq.html

(x * 2 for x in arr)
来源：http://hz.zdqjudy.top/gtcwxtorky.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.fengsongda.top/gtuegmclqf.html

Counter(arr).most_common(3)
来源：http://hz.nanxinkj.top/gtfmomqcfr.html

[U13] Py：固定长度队列
来源：http://hz.birdmap.top/gtpakzbjwm.html

deque(maxlen=10)
来源：http://hz.yuanzhike.top/gtvnkpikqx.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtkcqlwnsa.html

defaultdict(list)
来源：http://hz.yj20258.top/gtwnyyacoa.html

[U15] Py：高精度计时
来源：http://hz.jinqigfzy.top/gtomzplnaa.html

t = time.perf_counter()
来源：http://hz.gzhubu.top/gtxfecomjv.html

[U16] Py：命令行参数解析
来源：http://hz.smart0.xyz/gttwklbglh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xingfuxueyuan.xyz/gtdcedujew.html

[U17] Py：初始化日志
来源：http://hz.bjfxy.top/gttwfkwmrc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aizwys.cn/gtrsgzgvud.html

[U18] Py：预编译正则
来源：http://hz.yonumen.top/gtlqbawjpj.html

pat = re.compile(r"\d+")
来源：http://hz.wangdashe.top/gtiborzhhn.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtmytyrpnw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.9152youxi.cn/gtgcymdjzz.html

[U20] Py：缓存函数结果
来源：http://hz.xinyue.icu/gtgyvmgksm.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxinkj.top/gtwjlejgnp.html

[U21] Py：自定义上下文管理器
来源：http://hz.316326.xyz/gtkvrytfcg.html

@contextlib.contextmanager
来源：http://hz.ywan-chungtsiang.top/gtfmnmhips.html

[U22] Py：矩阵转置
来源：http://hz.shuidangran.top/gthhhghimv.html

list(zip(*m))
来源：http://hz.0kj1m.cn/gtpgjmuteb.html

[U23] Py：分块读取大文件
来源：http://hz.havefunace.top/gtjmwpkonh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.quarkkingdee.top/gtcndzpegh.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtyfssswxk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtwcnukfxm.html

[U25] Py：CSV 按字典读
来源：http://hz.xziqi.cn/gtbdpkdtil.html

csv.DictReader(f)
来源：http://hz.sufxvd.cn/gtcbfidoxz.html

[U26] Py：并发下载
来源：http://hz.mhx1999.top/gtlfiuatzk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zycfv.cn/gthzilyxlz.html

[U27] Py：异步 HTTP
来源：http://hz.vqdsnc.cn/gtcvdtgjim.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtuvjoysfn.html

[U28] Py：类型别名
来源：http://hz.cqqwz.cn/gtrlodgufu.html

UserId = int
来源：http://hz.andypj.xyz/gtluvvttxi.html

[U29] Py：属性校验
来源：http://hz.cdnleiting.top/gtfvujgxvq.html

@property 与 @x.setter 配合
来源：http://hz.yonumen.top/gtpnzepywu.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtiiwcptxy.html

@dataclass(slots=True)
来源：http://hz.dianchejie.cn/gtmkghuyyp.html

[U31] Py：单测
来源：http://hz.tianlin.xyz/gtudbvpvsi.html

python -m pytest -q
来源：http://hz.gaohongyu789.top/gtypyytquz.html

[U32] Py：代码格式化
来源：http://hz.xziqi.cn/gtvusbkzdv.html

ruff format . && ruff check --fix .
来源：http://hz.yj202588.top/gtkswupbtj.html

[U33] Py：打包发布
来源：http://hz.9152youxi.cn/gtppebqcug.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtlfktpowv.html

[U34] Py：判断编码
来源：http://hz.mhx1999.top/gtkazfknei.html

chardet.detect(raw)
来源：http://hz.zhijiandao.cn/gthpbsbcbv.html

[U35] Py：发送邮件
来源：http://hz.chenzaomai.com/gtcxzvveog.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhiwuduotai.top/gtmytehbpi.html

[U36] Py：定时任务
来源：http://hz.xuanzx.com/gtcznwfbgk.html

schedule.every(10).minutes.do(job)
来源：http://hz.cheryme.top/gtshrbotze.html

[U37] Py：读写 Excel
来源：http://hz.9152youxi.cn/gtuyfbbmxg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ydzc1.top/gtktfqtumg.html

[U38] Py：获取脚本所在目录
来源：http://hz.kuanghao11.cn/gtgtgfsssk.html

Path(__file__).resolve().parent
来源：http://hz.c1oappe.top/gtymswsdmd.html

[U39] Py：判断是否在交互环境
来源：http://hz.tianlin.xyz/gtemdyhmsm.html

sys.stdout.isatty()
来源：http://hz.yj20258.top/gtaykcokqb.html

[U40] Py：打印到标准错误
来源：http://hz.cqqwz.cn/gtwoezpotf.html

print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtuakrpaxb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ywan-chungtsiang.top/gtuolwbous.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cashguo.top/gtpyojdffo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xziqi.cn/gtyimwfblf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.aibaodan.cn/gtaolweenl.html

[U43] PHP：声明命名空间
来源：http://hz.yj20258888.top/gtqpueirql.html

namespace App\Http;
来源：http://hz.tianlin.xyz/gtfrbvcncc.html

[U44] PHP：开启严格类型
来源：http://hz.dianchejie.cn/gtofofwsse.html

declare(strict_types=1);
来源：http://hz.hammf.cn/gtcixwiqlu.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cheryme.top/gtmgmpsfxh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtvekkxasd.html

[U46] PHP：可空类型
来源：http://hz.tian-w.cn/gtxinjrche.html

?string $name = null
来源：http://hz.zycfv.cn/gtgrfmivcr.html

[U47] PHP：联合类型
来源：http://hz.jqgfzy.top/gtebplzpjp.html

int|string $id
来源：http://hz.mhx1999.top/gtckjbqzzy.html

[U48] PHP：纯枚举
来源：http://hz.xuanzx.com/gtadkcpecl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.svipenyu.cn/gtqcnyojcv.html

[U49] PHP：只读属性
来源：http://hz.havefunace.top/gtkbofyons.html

public readonly string $name
来源：http://hz.shuidangran.top/gtinzapram.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtijhifcjf.html

public function __construct(private int $id) {}
来源：http://hz.yvedp.cn/gtqiqlznci.html

[U51] PHP：数组解构
来源：http://hz.zhixingplan.top/gtsgwhnscj.html

[$a, $b] = $arr;
来源：http://hz.hfpthk.cn/gtukbaoulw.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gtkbhjafrn.html

$double = fn($x) => $x * 2;
来源：http://hz.shzxlz.cn/gtyycbttgp.html

[U53] PHP：空合并运算符
来源：http://hz.haohaochexian.top/gtmayarcgg.html

$v = $a ?? $b ?? "default";
来源：http://hz.iojbl.cn/gtyzunrngt.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtesmwfgkr.html

$obj?->method()
来源：http://hz.jinyuanbaomall.cn/gtevmbwxxc.html

[U55] PHP：match 表达式
来源：http://hz.jianghu66.top/gtkvdbwqkr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.nanxuanxn.top/gtcsrvbrqi.html

[U56] PHP：命名参数
来源：http://hz.smart0.xyz/gtcjofufbk.html

f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtqqftpwuu.html

[U57] PHP：字符串插值
来源：http://hz.hysaishi.cn/gtanvirasx.html

"值: {$a}"
来源：http://hz.xylfe.cn/gtyvtlbnrz.html

[U58] PHP：数组三件套
来源：http://hz.xingfuxueyuan.xyz/gtzkdtcpka.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jqgufenzy.top/gtqftwteaj.html

[U59] PHP：自定义排序
来源：http://hz.dashuyun.cn/gtqzqxjevf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtchjcjskn.html

[U60] PHP：JSON 编解码
来源：http://hz.ybcxt.top/gtjcivfixp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.redwolf501.top/gtemrkyhfv.html

[U61] PHP：正则
来源：http://hz.zhiwuduotai.top/gtkapdirdh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtzezmysoy.html

[U62] PHP：日期对象
来源：http://hz.hywenlv.cn/gtcfkesmsq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.vqdsnc.cn/gtmwysftdg.html

[U63] PHP：文件读写
来源：http://hz.zhoulong.xyz/gtbafvddow.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.tanke756.top/gtkegxafgc.html

[U64] PHP：目录遍历
来源：http://hz.chenjidiqi.icu/gteibwscfm.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cashguo.top/gtpcwpovap.html

[U65] PHP：会话
来源：http://hz.zhengqikj.top/gtxygeiwhk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.aizwys.cn/gtxtspjfbx.html

[U66] PHP：设置 Cookie
来源：http://hz.haohaochexian.top/gteoykekum.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hysaishi.cn/gthmdyuyun.html

[U67] PHP：处理文件上传
来源：http://hz.xuetiantiany.cn/gtndhrtuzi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhongyouzk.top/gtxgrrttih.html

[U68] PHP：PDO 连接
来源：http://hz.nwbrower.top/gttjodjiuz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xinyue.icu/gtdjwbcxmj.html

[U69] PHP：PDO 预处理
来源：http://hz.wangshuangyany.cn/gtezdmynmi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhaomingkeji.xyz/gtmofuwyae.html

[U70] PHP：PDO 事务
来源：http://hz.quarkkingdee.top/gtiichyilz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.pengpengdd.cyou/gtftazowxm.html


<!-- 参考信息 -->