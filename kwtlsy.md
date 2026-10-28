代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.yonumen.top/gtuyejjlsc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cheryme.top/gtmxtlfqzy.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gttzdskmsc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xziqi.cn/gtkhfwqijx.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gtlwpszmme.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtkebxsohv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yonumen.top/gtouafwrzp.html

[S50] C++：格式化数字
来源：http://hz.shuidangran.top/gtulgmhvwx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.gzhubu.top/gtqcuqwull.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtemdgpafg.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangkeji.top/gtwkknpcrl.html

[S52] C++：const 与 noexcept
来源：http://hz.quarkkingdee.top/gtrbpayooz.html

int size() const noexcept { return n_; }
来源：http://hz.jlsjyb.cn/gtcrmbfzsd.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gtigiylyfo.html

std::vector<int> w = std::move(v);
来源：http://hz.dianchejie.cn/gtkfypltjx.html

[S54] C++：异常处理
来源：http://hz.hongshengwenyu.top/gtwrxsgxpq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zdqjudy.top/gtfsixslcl.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtbrdmsfrl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.vqdsnc.cn/gtotawzgce.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtwqzsqwpt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.iojbl.cn/gtsytozgvh.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtmtrxekmc.html

constexpr int N = 10;
来源：http://hz.cheryme.top/gtejianepa.html

[S58] C++：命名空间
来源：http://hz.xingfuxueyuan.xyz/gtposxxpaw.html

namespace ns { int f() { return 1; } }
来源：http://hz.gogol.net.cn/gtcexynghy.html

[S59] C++：静态断言
来源：http://hz.xingfuxueyuan.xyz/gtxdgukrqf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yvedp.cn/gtmrhjmwha.html

[S60] C++：遍历并删除元素
来源：http://hz.tanke756.top/gtvtvndogk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gtehxwpsyo.html

================================================================================
来源：http://hz.jlsjyb.cn/gtahrvuetn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtwinblxdg.html

================================================================================
来源：http://hz.ppjwa.cn/gturxqxguq.html

[T01] Kotlin：Hello World
来源：http://hz.hfpthk.cn/gtqvwofuju.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtpgkyeerl.html

[T02] Kotlin：变量
来源：http://hz.fengsongda.top/gtilpcakyi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigufen.top/gtlvntkodk.html

[T03] Kotlin：字符串模板
来源：http://hz.aibaodan.cn/gtwabxobnr.html

"值: $b"
来源：http://hz.cdnleiting.top/gtpohbmixe.html

[T04] Kotlin：空安全
来源：http://hz.meibo888.top/gtghrjdvxs.html

val n: String? = null;  n?.length
来源：http://hz.jqgfzy.top/gtouadnbgr.html

[T05] Kotlin：when 表达式
来源：http://hz.daxiang520.top/gtuzdxnzrl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dianchejie.cn/gtbnjsipap.html

[T06] Kotlin：集合映射
来源：http://hz.ybcxt.top/gtkmmtevjw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtibdxmrqh.html

[T07] Kotlin：集合过滤
来源：http://hz.hfpthk.cn/gtuyfqtlpr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nwbrower.top/gtnmwbldqc.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gtrvnctdnw.html

data class User(val name: String, val age: Int)
来源：http://hz.9152youxi.cn/gtljstmyjs.html

[T09] Kotlin：扩展函数
来源：http://hz.xylfe.cn/gtiwtgbevz.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtrrbyevqr.html

[T10] Kotlin：默认参数
来源：http://hz.shangyingyoupin.top/gtpfokxslm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtfvrnqxpi.html

[T11] Kotlin：协程
来源：http://hz.yj20258.top/gtssmuozxd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yonumen.top/gtusfvlwui.html

[T12] Kotlin：解构声明
来源：http://hz.sweek.top/gtbjlcmkwz.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtyaxulpbx.html

[T13] Kotlin：只读 Map
来源：http://hz.gaohongyu789.top/gtjrapnflj.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtexcwvwfq.html

[T14] Kotlin：循环
来源：http://hz.guowangkeji.top/gtqqldcvwa.html

for (i in 1..10) println(i)
来源：http://hz.dashuyun.cn/gtobbbamut.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtvpqkjtkk.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gtxgkdwkvh.html

[T16] Swift：Hello World
来源：http://hz.aizwys.cn/gthchyyurt.html

print("Hello")
来源：http://hz.yj20258888.top/gtrxhkbqlq.html

[T17] Swift：变量与常量
来源：http://hz.nanxinkj.top/gtdizfkwjv.html

var a = 1;  let b = 2
来源：http://hz.xylfe.cn/gtlgiviera.html

[T18] Swift：字符串插值
来源：http://hz.dianchejie.cn/gtxdurjwka.html

"值: \(b)"
来源：http://hz.yonumen.top/gtsmhdfjsr.html

[T19] Swift：可选绑定
来源：http://hz.kuanghao11.cn/gtaljsannq.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtirdiozif.html

[T20] Swift：数组操作
来源：http://hz.dashuyun.cn/gtlpyejcbi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtxefeoznu.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtuxmtvtmk.html

for x in a { print(x) }
来源：http://hz.xylfe.cn/gtnjaoexuc.html

[T22] Swift：字典
来源：http://hz.zdqjudy.top/gtipqbbwui.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.52xcode.cn/gtbipzosjw.html

[T23] Swift：函数
来源：http://hz.wangshuangyany.cn/gtqpyelwst.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ppjwa.cn/gturtsgqzb.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtsvfundiz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.redwolf501.top/gtsfbppemj.html

[T25] Swift：结构体
来源：http://hz.nwbrower.top/gtsqmsmgoq.html

struct P { var x: Int }
来源：http://hz.meibo888.top/gtfpkqzfko.html

[T26] Swift：类与重写
来源：http://hz.xuanzx.com/gttdqvsphk.html

class A: Base { override func f() {} }
来源：http://hz.xuetiantiany.cn/gtppmhturh.html

[T27] Swift：错误处理
来源：http://hz.shanyushiyangkeji.top/gtgovlhaen.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtigpwllhe.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtmwqvygwy.html

enum Color { case red, green }
来源：http://hz.andypj.xyz/gtyeplfhec.html

[T29] Swift：guard 提前返回
来源：http://hz.chenzaomai.com/gtsbocmuuk.html

guard let x = opt else { return }
来源：http://hz.yj20258.top/gtiidpcnsz.html

[T30] Swift：协议
来源：http://hz.quarkkingdee.top/gtdnleqxav.html

protocol Shape { func area() -> Double }
来源：http://hz.bjfxy.top/gtxjqalaqw.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gthuydysmz.html

print("Hello")
来源：http://hz.hnxiangtu.top/gttxqtdbum.html

[T32] Lua：局部变量
来源：http://hz.nanxuanxn.top/gtscgdbscx.html

local a = 1
来源：http://hz.iojbl.cn/gtjhlhvndk.html

[T33] Lua：表（数组）
来源：http://hz.zdqjudy.top/gtqllbupqb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gtnosbbott.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtzexbotgg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yanxiufei.cn/gtofzbnssf.html

[T35] Lua：字典表
来源：http://hz.iojbl.cn/gtqohxjgwy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jinqigfzy.top/gtdtsdeqah.html

[T36] Lua：函数
来源：http://hz.daxiang520.top/gtuxxlvyxi.html

function add(a, b) return a + b end
来源：http://hz.dashuyun.cn/gtbyohiyor.html

[T37] Lua：字符串拼接
来源：http://hz.hywenlv.cn/gtleatskpr.html

"a" .. "b"
来源：http://hz.nwbrower.top/gtbofmyxii.html

[T38] Lua：条件
来源：http://hz.zhengqikj.top/gtbzjjridc.html

if x > 0 then print("正") end
来源：http://hz.ywan-chungtsiang.top/gtcivvrcnx.html

[T39] Lua：模式匹配
来源：http://hz.cqqwz.cn/gthxozbacs.html

string.find(s, "%d+")
来源：http://hz.hnxiangtu.top/gtgfdekyni.html

[T40] Lua：元表
来源：http://hz.sweek.top/gthtqrbhwi.html

setmetatable({}, { __index = base })
来源：http://hz.0kj1m.cn/gtbslgnbhs.html

[T41] Perl：Hello World
来源：http://hz.daria6918.cn/gtqsrsshjm.html

print "Hello\n";
来源：http://hz.ivvv.top/gtqcrwrkvn.html

[T42] Perl：变量类型
来源：http://hz.xziqi.cn/gtrcqytnvd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtsuabnudq.html

[T43] Perl：字符串插值
来源：http://hz.wangshuangyany.cn/gtwuprfvhb.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtzxcppxoh.html

[T44] Perl：条件
来源：http://hz.wangshuangyany.cn/gtuttflaam.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtewnpjcwj.html

[T45] Perl：数组遍历
来源：http://hz.yj20258888.top/gtnhhjvhdt.html

for my $x (@arr) { print $x; }
来源：http://hz.sxryk.cn/gtaiomjklu.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gtworyxpkw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.havefunace.top/gtwhrwupzr.html

[T47] Perl：正则捕获
来源：http://hz.jinqigufen.top/gtpzhpkidx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.52xcode.cn/gtlnrhzkgw.html

[T48] Perl：正则替换
来源：http://hz.cqqwz.cn/gttpspeuel.html

$s =~ s/old/new/g;
来源：http://hz.chenjidiqi.icu/gtkxhbybro.html

[T49] Perl：函数
来源：http://hz.tanke756.top/gtwaiuhdxc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.redwolf501.top/gtpcioukdt.html

[T50] Perl：逐行读文件
来源：http://hz.ppjwa.cn/gtxbtmiisg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhoulong.xyz/gtyzyygyox.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cucudq.cn/gtgorlidpl.html

[T51] Scala：Hello World
来源：http://hz.jinqigfzy.top/gtrrewsfgy.html

println("Hello")
来源：http://hz.jinqigfzy.top/gtomasclrw.html

[T52] Scala：变量
来源：http://hz.tanke756.top/gtkldrrbey.html

val a = 1;  var b = 2
来源：http://hz.svipenyu.cn/gtcaspcpap.html

[T53] Scala：字符串插值
来源：http://hz.mhx1999.top/gtvxawcgib.html

s"值: $b"
来源：http://hz.nanxinkj.top/gtqnceanux.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtprmsrhqa.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuanzhike.top/gtmwozxwim.html

[T55] Scala：集合过滤
来源：http://hz.ivvv.top/gtpwqmcbie.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.svipenyu.cn/gtmqnsqawu.html

[T56] Scala：样例类
来源：http://hz.gzhubu.top/gtezzzotau.html

case class User(name: String, age: Int)
来源：http://hz.chenzaomai.com/gtxrehwizc.html

[T57] Scala：模式匹配
来源：http://hz.nanxuanxn.top/gtzxeotfzs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gttgbvzlvy.html

[T58] Scala：函数定义
来源：http://hz.nwbrower.top/gtqfbzupkz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jiagoushi.top/gtbwbqempc.html

[T59] Scala：循环
来源：http://hz.jinqigufen.top/gtakfqpubs.html

for (i <- 1 to 10) println(i)
来源：http://hz.jiagoushi.top/gtnxoocdfa.html

[T60] Scala：折叠
来源：http://hz.tianlin.xyz/gtcmdrbxym.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.gogol.net.cn/gtkqbmbvyl.html

================================================================================
来源：http://hz.ppjwa.cn/gtcdbsnihz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtrrkjvkhg.html

================================================================================
来源：http://hz.daria6918.cn/gtioiwamtu.html

[U01] Py：创建虚拟环境
来源：http://hz.yangfankeji.com/gtuitpbhnv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.pengpengdd.cyou/gtthwjvvlt.html

[U02] Py：导出 / 安装依赖
来源：http://hz.havefunace.top/gtbjedlcql.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenzaomai.com/gtscobtxmm.html

[U03] Py：加载 .env 配置
来源：http://hz.ehwqpu.com/gttmsweqgt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.svipenyu.cn/gtvlvbapah.html

[U04] Py：变量调试打印
来源：http://hz.svipenyu.cn/gtzypbpkhb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yangfankeji.com/gtgucsdpgd.html

[U05] Py：列表去重且保序
来源：http://hz.andypj.xyz/gtugdsuyyc.html

list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtubhkkseg.html

[U06] Py：合并两个字典
来源：http://hz.0kj1m.cn/gtpnlqtzal.html

{**a, **b}
来源：http://hz.tianlin.xyz/gtodtjjgfv.html

[U07] Py：反转字典键值
来源：http://hz.c1oappe.top/gtrxlzveob.html

{v: k for k, v in d.items()}
来源：http://hz.sxryk.cn/gtkjbjpagj.html

[U08] Py：展平二维列表
来源：http://hz.wangdashe.top/gteaoojxov.html

[y for x in nested for y in x]
来源：http://hz.jinqigfzy.top/gtcykrlzbb.html

[U09] Py：字典取最大值的键
来源：http://hz.zhengqikj.top/gtqixkpwpv.html

max(d, key=d.get)
来源：http://hz.cqqwz.cn/gtsxgowqrn.html

[U10] Py：按值排序字典
来源：http://hz.zhaomingkeji.xyz/gtyrornxtm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nwbrower.top/gtaxfehvni.html

[U11] Py：生成器表达式
来源：http://hz.52xcode.cn/gtlkxtiyhz.html

(x * 2 for x in arr)
来源：http://hz.pengpengdd.cyou/gtjhdxupel.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hongshengwenyu.top/gtchgsmqgt.html

Counter(arr).most_common(3)
来源：http://hz.yj20258888.top/gthrdcajam.html

[U13] Py：固定长度队列
来源：http://hz.dashuyun.cn/gtydhamnei.html

deque(maxlen=10)
来源：http://hz.gaohongyu789.top/gtjbtwqtlu.html

[U14] Py：分组收集到列表
来源：http://hz.yangfankeji.com/gtfhlneign.html

defaultdict(list)
来源：http://hz.tian-w.cn/gtwziccczd.html

[U15] Py：高精度计时
来源：http://hz.cashguo.top/gtnvxmntkk.html

t = time.perf_counter()
来源：http://hz.sweek.top/gtyyfuybyz.html

[U16] Py：命令行参数解析
来源：http://hz.yongpay.top/gtmhefwdgr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.wangdashe.top/gtkaogkspe.html

[U17] Py：初始化日志
来源：http://hz.ybcxt.top/gtaaweiriz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shzxlz.cn/gtxxwjnzez.html

[U18] Py：预编译正则
来源：http://hz.jyoumei.cn/gtaxsqorni.html

pat = re.compile(r"\d+")
来源：http://hz.yj202588.top/gteqvvkjeh.html

[U19] Py：正则替换带回调
来源：http://hz.fengsongda.top/gtiacbspsx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nanxinkj.top/gtczwngvgg.html

[U20] Py：缓存函数结果
来源：http://hz.yongpay.top/gtalwwxwpu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinghuilouyu.cn/gtfprbcyhi.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenjidiqi.icu/gtpdwgitmw.html

@contextlib.contextmanager
来源：http://hz.hnqzz.top/gtrbgzytba.html

[U22] Py：矩阵转置
来源：http://hz.daria6918.cn/gtfanuixbo.html

list(zip(*m))
来源：http://hz.iojbl.cn/gttmendabh.html

[U23] Py：分块读取大文件
来源：http://hz.shuidangran.top/gtrevytewe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xinyue.icu/gtwsiappoh.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtpyndewou.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.dianchejie.cn/gtdcbfpspr.html

[U25] Py：CSV 按字典读
来源：http://hz.quarkkingdee.top/gtrdkljbhs.html

csv.DictReader(f)
来源：http://hz.gogol.net.cn/gtrukoxfwr.html

[U26] Py：并发下载
来源：http://hz.dianchejie.cn/gtzajslsus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fzhhl.top/gteijkqjhn.html

[U27] Py：异步 HTTP
来源：http://hz.iojbl.cn/gtybpwjrbp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gttfawkaxx.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtjhgpdvyn.html

UserId = int
来源：http://hz.daxiang520.top/gtvyknmmin.html

[U29] Py：属性校验
来源：http://hz.shzxlz.cn/gtdidwnyje.html

@property 与 @x.setter 配合
来源：http://hz.ywan-chungtsiang.top/gtrigfimlg.html

[U30] Py：数据类
来源：http://hz.yanxiufei.cn/gtrwazvoyy.html

@dataclass(slots=True)
来源：http://hz.ehwqpu.com/gtvhdbndhn.html

[U31] Py：单测
来源：http://hz.jqgfzy.top/gtbrcubsla.html

python -m pytest -q
来源：http://hz.gzhubu.top/gtzvqpfnas.html

[U32] Py：代码格式化
来源：http://hz.gaohongyu789.top/gtzoeunphg.html

ruff format . && ruff check --fix .
来源：http://hz.xingfuxueyuan.xyz/gtyytsubpa.html

[U33] Py：打包发布
来源：http://hz.hammf.cn/gtwjdvcgjq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.9152youxi.cn/gtjogqlvpk.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtoanudwkk.html

chardet.detect(raw)
来源：http://hz.cheryme.top/gtxwygrkpa.html

[U35] Py：发送邮件
来源：http://hz.shanyushiyangkeji.top/gtxuzoivyc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.52xcode.cn/gthvkowtqo.html

[U36] Py：定时任务
来源：http://hz.316326.xyz/gtmmtqinro.html

schedule.every(10).minutes.do(job)
来源：http://hz.andypj.xyz/gtakfmgnwn.html

[U37] Py：读写 Excel
来源：http://hz.zdqjudy.top/gtumwkrxwq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cashguo.top/gtumgikbbu.html

[U38] Py：获取脚本所在目录
来源：http://hz.fzhhl.top/gticduyhon.html

Path(__file__).resolve().parent
来源：http://hz.hfpthk.cn/gtwzwfofym.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhengqikj.top/gtibdlafux.html

sys.stdout.isatty()
来源：http://hz.hywenlv.cn/gtvlcddefp.html

[U40] Py：打印到标准错误
来源：http://hz.snrcjt.cn/gtqrxezyhd.html

print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtnqdawsoj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.iojbl.cn/gtbixddwne.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xinyue.icu/gtanwgdgep.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangtech.top/gtskmflnlg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tian-w.cn/gtzmtjfncm.html

[U43] PHP：声明命名空间
来源：http://hz.shanyushiyangtech.top/gtpqqkclwq.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gtzcxtgsth.html

[U44] PHP：开启严格类型
来源：http://hz.zycfv.cn/gtqymtbtur.html

declare(strict_types=1);
来源：http://hz.pycfn.com/gtyeimvdtp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.9152youxi.cn/gtrmtxzdkq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gthdbielbf.html

[U46] PHP：可空类型
来源：http://hz.yj20258888.top/gtqncbdmfy.html

?string $name = null
来源：http://hz.cucudq.cn/gtlvdfggfp.html

[U47] PHP：联合类型
来源：http://hz.xylfe.cn/gtzavifejo.html

int|string $id
来源：http://hz.birdmap.top/gtzlnzhblb.html

[U48] PHP：纯枚举
来源：http://hz.daria6918.cn/gtjragisat.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.316326.xyz/gtlvcmacte.html

[U49] PHP：只读属性
来源：http://hz.zhijiandao.cn/gtzzazffyt.html

public readonly string $name
来源：http://hz.shuidangran.top/gtndrdcfbe.html

[U50] PHP：构造器属性提升
来源：http://hz.316326.xyz/gtawrijnot.html

public function __construct(private int $id) {}
来源：http://hz.tianlin.xyz/gtnqvfcngz.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gttsvuidms.html

[$a, $b] = $arr;
来源：http://hz.jinqigufen.top/gtlutauhha.html

[U52] PHP：箭头函数
来源：http://hz.ydzc1.top/gtibcbblls.html

$double = fn($x) => $x * 2;
来源：http://hz.tianlin.xyz/gtcmluhgbn.html

[U53] PHP：空合并运算符
来源：http://hz.zhiwuduotai.top/gtghusnqvg.html

$v = $a ?? $b ?? "default";
来源：http://hz.pengpengdd.cyou/gtpdlbhlxh.html

[U54] PHP：空安全调用
来源：http://hz.jinghuilouyu.cn/gtmzdjqfse.html

$obj?->method()
来源：http://hz.birdmap.top/gtwqgohvjh.html

[U55] PHP：match 表达式
来源：http://hz.zhongyouzk.top/gtlemwpafl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.haohaochexian.top/gtoavnudzf.html

[U56] PHP：命名参数
来源：http://hz.tanke756.top/gtlmgtduwx.html

f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtqovznzkb.html

[U57] PHP：字符串插值
来源：http://hz.ydzc1.top/gtdfvlfdkr.html

"值: {$a}"
来源：http://hz.jqgfzy.top/gtkgskvidt.html

[U58] PHP：数组三件套
来源：http://hz.ivvv.top/gttxjwllrm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtfbjxemsb.html

[U59] PHP：自定义排序
来源：http://hz.tian-w.cn/gtpxmibesi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.havefunace.top/gtkesprcan.html

[U60] PHP：JSON 编解码
来源：http://hz.jinyuanbaomall.cn/gtjueozujh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xylfe.cn/gtrnfmxrgq.html

[U61] PHP：正则
来源：http://hz.smart0.xyz/gtvtsponcf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtsudpmvqe.html

[U62] PHP：日期对象
来源：http://hz.ydzc1.top/gtvdrtaekw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.daria6918.cn/gtuvazxwih.html

[U63] PHP：文件读写
来源：http://hz.yuxming.cn/gtfaxbvhxe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yj20258888.top/gtixmsuynu.html

[U64] PHP：目录遍历
来源：http://hz.ehwqpu.com/gtgkgiufzo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.xziqi.cn/gtdwidnmsc.html

[U65] PHP：会话
来源：http://hz.xziqi.cn/gtuepvqpib.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.vqdsnc.cn/gtkmlmzwyo.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtabjllbpj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zycfv.cn/gtbygyzpqk.html

[U67] PHP：处理文件上传
来源：http://hz.ybcxt.top/gtcskjzvhr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.9152youxi.cn/gtygpvganm.html

[U68] PHP：PDO 连接
来源：http://hz.kuanghao11.cn/gtsbbgxvls.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yvedp.cn/gtvdqkodvl.html

[U69] PHP：PDO 预处理
来源：http://hz.shzxlz.cn/gtkrqiyref.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhaomingkeji.xyz/gtdiubwzlc.html

[U70] PHP：PDO 事务
来源：http://hz.bjfxy.top/gtfgtvkcvr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.shuidangran.top/gtnqjnwrkl.html

[U71] PHP：抛出异常
来源：http://hz.shzxlz.cn/gtkzmuagep.html

throw new RuntimeException("失败", 500);
来源：http://hz.yueranfly.top/gtpzikauoc.html

[U72] PHP：写错误日志
来源：http://hz.jlsjyb.cn/gtsaaisycz.html

error_log("失败: " . $e->getMessage());
来源：http://hz.9152youxi.cn/gtkbqksszb.html


<!-- 参考信息 -->