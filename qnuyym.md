代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gtjqwzkvfy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtavjnaemm.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtlpyslthg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtrvlkwmqz.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gtzgmqsarl.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtzlkbxykz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cqqwz.cn/gtlanmomli.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtlbkycuan.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtkfsgdmkp.html

[S51] C++：显式类型转换
来源：http://hz.aibaodan.cn/gtknrqiafv.html

static_cast<double>(a) / b
来源：http://hz.sufxvd.cn/gtdytrrujm.html

[S52] C++：const 与 noexcept
来源：http://hz.zhiwuduotai.top/gtrguzhoro.html

int size() const noexcept { return n_; }
来源：http://hz.yj20258888.top/gtqmmlausp.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtsrmvewem.html

std::vector<int> w = std::move(v);
来源：http://hz.hywenlv.cn/gtvqaoptyg.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtgdhumist.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fengsongda.top/gtwoavrkwl.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtmvoodjrm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tianlin.xyz/gtdbatycth.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtxwujdjoh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hnxiangtu.top/gtmwcyhkbt.html

[S57] C++：编译期常量
来源：http://hz.xinyue.icu/gttvxpktgc.html

constexpr int N = 10;
来源：http://hz.9152youxi.cn/gtfmyesmvs.html

[S58] C++：命名空间
来源：http://hz.zhijiandao.cn/gtsvwqjqut.html

namespace ns { int f() { return 1; } }
来源：http://hz.jqgufenzy.top/gtpjsshwww.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtfyahekeb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shangyingyoupin.top/gtlvtodhdq.html

[S60] C++：遍历并删除元素
来源：http://hz.yongpay.top/gtlosdvmfx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ywan-chungtsiang.top/gtrkmeznms.html

================================================================================
来源：http://hz.tanke756.top/gtpsiqhkbs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.gotoacloud.top/gtbafwahsw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtyuxilfut.html

[T01] Kotlin：Hello World
来源：http://hz.yanxiufei.cn/gtdswhhlvp.html

println("Hello")
来源：http://hz.nwbrower.top/gteioqexbd.html

[T02] Kotlin：变量
来源：http://hz.zhijiandao.cn/gtofurlnxl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhixingplan.top/gtqcwqlpkm.html

[T03] Kotlin：字符串模板
来源：http://hz.9152youxi.cn/gtvjcalvax.html

"值: $b"
来源：http://hz.xuetiantiany.cn/gtzxkkunwt.html

[T04] Kotlin：空安全
来源：http://hz.gzhubu.top/gtwtdnndtp.html

val n: String? = null;  n?.length
来源：http://hz.meibo888.top/gtfcfmryov.html

[T05] Kotlin：when 表达式
来源：http://hz.jinqigufen.top/gtilbevnns.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.snrcjt.cn/gtkweiebki.html

[T06] Kotlin：集合映射
来源：http://hz.c1oappe.top/gtlmdfsgsm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.kuanghao11.cn/gtwqozycbr.html

[T07] Kotlin：集合过滤
来源：http://hz.xingfuxueyuan.xyz/gtdnmipxzr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.aibaodan.cn/gtirwyeewm.html

[T08] Kotlin：数据类
来源：http://hz.tian-w.cn/gtctchyxzq.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtlqtzxmmn.html

[T09] Kotlin：扩展函数
来源：http://hz.redwolf501.top/gtmtewlvln.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gtpifytwdl.html

[T10] Kotlin：默认参数
来源：http://hz.ydzc1.top/gtrhwwerty.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jianghu66.top/gtboskfwuy.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtlbdoysmj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtrtymxllv.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigfzy.top/gtbhvldyxv.html

val (a, b) = Pair(1, 2)
来源：http://hz.feifeiyinyue.top/gtgokfknhb.html

[T13] Kotlin：只读 Map
来源：http://hz.svipenyu.cn/gtwnivrncn.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gthefzrhcb.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gtpvrheevl.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtmnpoaufn.html

[T15] Kotlin：接口
来源：http://hz.chenlongwang.top/gtlvureeom.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gtpygybddn.html

[T16] Swift：Hello World
来源：http://hz.havefunace.top/gtkoqavffk.html

print("Hello")
来源：http://hz.jlsjyb.cn/gtvdjbaxdr.html

[T17] Swift：变量与常量
来源：http://hz.aibaodan.cn/gttsiqshfh.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtallqrwlw.html

[T18] Swift：字符串插值
来源：http://hz.zhixingplan.top/gtgunzgciz.html

"值: \(b)"
来源：http://hz.yongpay.top/gtfrvrrvto.html

[T19] Swift：可选绑定
来源：http://hz.aibaodan.cn/gtktirkpuv.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtazzfamjm.html

[T20] Swift：数组操作
来源：http://hz.meibo888.top/gtvcxdqjjz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guowangkeji.top/gtpndmawps.html

[T21] Swift：遍历
来源：http://hz.andypj.xyz/gtcsehwzec.html

for x in a { print(x) }
来源：http://hz.bjfxy.top/gtzgjfelgv.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtxvhbcnru.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shanyushiyangtech.top/gtlipibeys.html

[T23] Swift：函数
来源：http://hz.jyoumei.cn/gtslcpucsd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenjidiqi.icu/gtfuizufif.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtlemlyrjp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnxiangtu.top/gtmjebarru.html

[T25] Swift：结构体
来源：http://hz.bjfxy.top/gtzwxwnupp.html

struct P { var x: Int }
来源：http://hz.cashguo.top/gtsxkrphxq.html

[T26] Swift：类与重写
来源：http://hz.daria6918.cn/gtgufyatre.html

class A: Base { override func f() {} }
来源：http://hz.gotoacloud.top/gtxinypfdb.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtzleaqtre.html

do { try f() } catch { print(error) }
来源：http://hz.mhx1999.top/gtezrkhuej.html

[T28] Swift：枚举
来源：http://hz.jqgfzy.top/gteypjzcsf.html

enum Color { case red, green }
来源：http://hz.aibaodan.cn/gtccquzcvs.html

[T29] Swift：guard 提前返回
来源：http://hz.gzhubu.top/gtszyyazdf.html

guard let x = opt else { return }
来源：http://hz.yueranfly.top/gtifhqbpnf.html

[T30] Swift：协议
来源：http://hz.vqdsnc.cn/gtavhpylef.html

protocol Shape { func area() -> Double }
来源：http://hz.gaohongyu789.top/gtopilepnn.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtfxoihnsc.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtkgkhysry.html

[T32] Lua：局部变量
来源：http://hz.xingfuxueyuan.xyz/gtqnpzpome.html

local a = 1
来源：http://hz.0kj1m.cn/gtpldbimfy.html

[T33] Lua：表（数组）
来源：http://hz.chenlongwang.top/gtjxzmuznn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgfzy.top/gtrcgbltze.html

[T34] Lua：遍历表
来源：http://hz.bjfxy.top/gtlvtmvqcl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hongshengwenyu.top/gtediwwnzs.html

[T35] Lua：字典表
来源：http://hz.cucudq.cn/gtbcmpsyvi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtktxppjnm.html

[T36] Lua：函数
来源：http://hz.yongpay.top/gtfcgllnjk.html

function add(a, b) return a + b end
来源：http://hz.daria6918.cn/gttaswrmsv.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtvxuppvot.html

"a" .. "b"
来源：http://hz.andypj.xyz/gtsgefzxxi.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gticdczshh.html

if x > 0 then print("正") end
来源：http://hz.yangfankeji.com/gtvwxjczcs.html

[T39] Lua：模式匹配
来源：http://hz.shangyingyoupin.top/gtdbqvuddi.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtdlnzgqov.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtkstqrcbx.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258888.top/gtvomuwjhc.html

[T41] Perl：Hello World
来源：http://hz.daxiang520.top/gtslhkkzgl.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtinneblpj.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtuyohtuos.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ywan-chungtsiang.top/gtayjhhowo.html

[T43] Perl：字符串插值
来源：http://hz.aibaodan.cn/gtdknwztkh.html

"值: $a"
来源：http://hz.meibo888.top/gtjenbheqy.html

[T44] Perl：条件
来源：http://hz.guannengcc.top/gtujgqnkvk.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gtrzsyznkt.html

[T45] Perl：数组遍历
来源：http://hz.daria6918.cn/gtfjqqcyua.html

for my $x (@arr) { print $x; }
来源：http://hz.svipenyu.cn/gtdkztxhkx.html

[T46] Perl：哈希操作
来源：http://hz.dianchejie.cn/gtwjliwius.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shangyingyoupin.top/gtrkxroboh.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gttvzzmjfi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cashguo.top/gtulznmock.html

[T48] Perl：正则替换
来源：http://hz.shanyushiyangtech.top/gtqgngrwsu.html

$s =~ s/old/new/g;
来源：http://hz.wangshuangyany.cn/gteracezyp.html

[T49] Perl：函数
来源：http://hz.kuanghao11.cn/gtuzrornrh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtsteesgzk.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtojehcykd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xziqi.cn/gtoqbxumqu.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jinqigufen.top/gtrbtwcfwt.html

[T51] Scala：Hello World
来源：http://hz.meibo888.top/gtnxwbflli.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtkezpdgav.html

[T52] Scala：变量
来源：http://hz.guowangkeji.top/gtkxlrbekj.html

val a = 1;  var b = 2
来源：http://hz.zhijiandao.cn/gtkunhfnfj.html

[T53] Scala：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtwkrwekey.html

s"值: $b"
来源：http://hz.yueranfly.top/gtalvgwoce.html

[T54] Scala：集合映射
来源：http://hz.zdqjudy.top/gtaaetoqih.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.bjfxy.top/gtmjtocayv.html

[T55] Scala：集合过滤
来源：http://hz.kuanghao11.cn/gtttjldgtc.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zycfv.cn/gtlsyujwec.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtgmabsyqv.html

case class User(name: String, age: Int)
来源：http://hz.daria6918.cn/gtamcfjzyw.html

[T57] Scala：模式匹配
来源：http://hz.shangyingyoupin.top/gtgmodpapp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.9152youxi.cn/gtsfxaqeyw.html

[T58] Scala：函数定义
来源：http://hz.xylfe.cn/gttsfglhvk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtdcafjnlu.html

[T59] Scala：循环
来源：http://hz.zhijiandao.cn/gtipmfcuth.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhongyouzk.top/gtaipyhkbj.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtfogabvak.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xziqi.cn/gtcnmcmpit.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtoxolaaxn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtpqtxbqya.html

================================================================================
来源：http://hz.fzhhl.top/gtpsupbakb.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gtrkybmank.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gogol.net.cn/gtmwomyduy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jinghuilouyu.cn/gtahaaecmg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yanxiufei.cn/gtdlduiqvw.html

[U03] Py：加载 .env 配置
来源：http://hz.zhixingplan.top/gtiqutupmb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shuidangran.top/gtbsqxhgcq.html

[U04] Py：变量调试打印
来源：http://hz.ydzc1.top/gtqfqoatza.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cdnleiting.top/gtyojsqbfk.html

[U05] Py：列表去重且保序
来源：http://hz.gzhubu.top/gtptbhxtwi.html

list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtmfjqnkwf.html

[U06] Py：合并两个字典
来源：http://hz.wangdashe.top/gttguexayx.html

{**a, **b}
来源：http://hz.ydjk.org.cn/gtqcmrupdq.html

[U07] Py：反转字典键值
来源：http://hz.tianlin.xyz/gtbqkjyoeh.html

{v: k for k, v in d.items()}
来源：http://hz.gzhubu.top/gtcmsympkk.html

[U08] Py：展平二维列表
来源：http://hz.shzxlz.cn/gtlrwkdgrc.html

[y for x in nested for y in x]
来源：http://hz.hywenlv.cn/gtilejlman.html

[U09] Py：字典取最大值的键
来源：http://hz.zhoulong.xyz/gticyndmuu.html

max(d, key=d.get)
来源：http://hz.iojbl.cn/gtfbggchit.html

[U10] Py：按值排序字典
来源：http://hz.bjfxy.top/gtesikfysr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yangfankeji.com/gtjyiqgqnh.html

[U11] Py：生成器表达式
来源：http://hz.havefunace.top/gtjfpaxuom.html

(x * 2 for x in arr)
来源：http://hz.cucudq.cn/gtfieggfpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jqgfzy.top/gtncblcorf.html

Counter(arr).most_common(3)
来源：http://hz.chenzaomai.com/gtkwtaheox.html

[U13] Py：固定长度队列
来源：http://hz.gaohongyu789.top/gtgplgjssq.html

deque(maxlen=10)
来源：http://hz.mhx1999.top/gtaihqqrei.html

[U14] Py：分组收集到列表
来源：http://hz.birdmap.top/gtbrjnjdnp.html

defaultdict(list)
来源：http://hz.cqqwz.cn/gtpqolhuvh.html

[U15] Py：高精度计时
来源：http://hz.ydjk.org.cn/gtjzzlhgbu.html

t = time.perf_counter()
来源：http://hz.zhaomingkeji.xyz/gtfwaaehix.html

[U16] Py：命令行参数解析
来源：http://hz.ydzc1.top/gtetyypsmc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtzdmwfzsr.html

[U17] Py：初始化日志
来源：http://hz.hammf.cn/gtqvqcpqom.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hnxiangtu.top/gtllkrtpvz.html

[U18] Py：预编译正则
来源：http://hz.yj20258.top/gtziwndoyc.html

pat = re.compile(r"\d+")
来源：http://hz.havefunace.top/gtjvxolpbv.html

[U19] Py：正则替换带回调
来源：http://hz.havefunace.top/gtxqmsuzkn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.fzhhl.top/gtcqmhxcah.html

[U20] Py：缓存函数结果
来源：http://hz.fzhhl.top/gtjbbktiiq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj202588.top/gtjydxhulj.html

[U21] Py：自定义上下文管理器
来源：http://hz.daria6918.cn/gtyzwpqsun.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gtospbxgxv.html

[U22] Py：矩阵转置
来源：http://hz.sufxvd.cn/gtscqfhpjn.html

list(zip(*m))
来源：http://hz.hongshengwenyu.top/gtsgkxpqin.html

[U23] Py：分块读取大文件
来源：http://hz.daria6918.cn/gtlxnvuvxu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtkhdbhuvj.html

[U24] Py：路径操作
来源：http://hz.fzhhl.top/gtejbcxbdb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.havefunace.top/gtnrpofcil.html

[U25] Py：CSV 按字典读
来源：http://hz.xingfuxueyuan.xyz/gtbesmgipu.html

csv.DictReader(f)
来源：http://hz.snrcjt.cn/gtvssalsye.html

[U26] Py：并发下载
来源：http://hz.redwolf501.top/gtvrfdfpjp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.hywenlv.cn/gtzbgqlows.html

[U27] Py：异步 HTTP
来源：http://hz.sweek.top/gtsruighqe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ywan-chungtsiang.top/gtdvqqgmwo.html

[U28] Py：类型别名
来源：http://hz.c1oappe.top/gtwxunjsko.html

UserId = int
来源：http://hz.yuxming.cn/gtyqaxbqgk.html

[U29] Py：属性校验
来源：http://hz.sxryk.cn/gtfippottf.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gtkmfatzrq.html

[U30] Py：数据类
来源：http://hz.jlsjyb.cn/gtjxqmkdfc.html

@dataclass(slots=True)
来源：http://hz.jinghuilouyu.cn/gtfyihqixu.html

[U31] Py：单测
来源：http://hz.ppjwa.cn/gtbrqrgdhs.html

python -m pytest -q
来源：http://hz.dianchejie.cn/gtmtfznydt.html

[U32] Py：代码格式化
来源：http://hz.hysaishi.cn/gtyyrfpfwq.html

ruff format . && ruff check --fix .
来源：http://hz.pycfn.com/gtbsrurxik.html

[U33] Py：打包发布
来源：http://hz.jyoumei.cn/gtgeeyjwqs.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hammf.cn/gtszdsvmjg.html

[U34] Py：判断编码
来源：http://hz.chenlongwang.top/gtygafckyx.html

chardet.detect(raw)
来源：http://hz.mhx1999.top/gtyelgukmn.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gteabszoaa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.havefunace.top/gtxxchdxwd.html

[U36] Py：定时任务
来源：http://hz.jinqigfzy.top/gtekzqapuw.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinqigufen.top/gttnlrzoka.html

[U37] Py：读写 Excel
来源：http://hz.aibaodan.cn/gtzeylyrtq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.chenjidiqi.icu/gtwrtdblcp.html

[U38] Py：获取脚本所在目录
来源：http://hz.ydzc1.top/gtvlkkdlyo.html

Path(__file__).resolve().parent
来源：http://hz.zycfv.cn/gtjhnyseni.html

[U39] Py：判断是否在交互环境
来源：http://hz.tanke756.top/gtaifyqlba.html

sys.stdout.isatty()
来源：http://hz.aizwys.cn/gterplybnh.html

[U40] Py：打印到标准错误
来源：http://hz.meibo888.top/gtbwikvtlo.html

print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtpzjjybiv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.birdmap.top/gtqdhlwvjp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.feifeiyinyue.top/gtrkqzmlbf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.316326.xyz/gtimbuowba.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.0kj1m.cn/gttfzhqepr.html

[U43] PHP：声明命名空间
来源：http://hz.fengsongda.top/gtduvweqmr.html

namespace App\Http;
来源：http://hz.yueranfly.top/gtijuaqigc.html

[U44] PHP：开启严格类型
来源：http://hz.jinqigfzy.top/gtmpazplrz.html

declare(strict_types=1);
来源：http://hz.zhengqikj.top/gtbgrxbjuw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuxming.cn/gtfcxfqbxx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtiitqxaix.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtshehblnr.html

?string $name = null
来源：http://hz.andypj.xyz/gtjsgonopb.html

[U47] PHP：联合类型
来源：http://hz.xuanzx.com/gtyozdzuqt.html

int|string $id
来源：http://hz.cheryme.top/gtwdcfuzyn.html

[U48] PHP：纯枚举
来源：http://hz.sweek.top/gtshfmmypw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhaomingkeji.xyz/gtffkggltl.html

[U49] PHP：只读属性
来源：http://hz.shangyingyoupin.top/gtxltntnti.html

public readonly string $name
来源：http://hz.zhoulong.xyz/gtflrsygyi.html

[U50] PHP：构造器属性提升
来源：http://hz.shuidangran.top/gtmmjlbwzq.html

public function __construct(private int $id) {}
来源：http://hz.xingfuxueyuan.xyz/gtbysnbzog.html

[U51] PHP：数组解构
来源：http://hz.zhixingplan.top/gtymscbwhz.html

[$a, $b] = $arr;
来源：http://hz.hammf.cn/gtchdtjamm.html

[U52] PHP：箭头函数
来源：http://hz.gaohongyu789.top/gtrsfpqruq.html

$double = fn($x) => $x * 2;
来源：http://hz.pengpengdd.cyou/gtoxvpaegx.html

[U53] PHP：空合并运算符
来源：http://hz.smart0.xyz/gtrxrzasjw.html

$v = $a ?? $b ?? "default";
来源：http://hz.cheryme.top/gtixluxdwn.html

[U54] PHP：空安全调用
来源：http://hz.xylfe.cn/gtnagvibab.html

$obj?->method()
来源：http://hz.zhixingplan.top/gtyjqlmhas.html

[U55] PHP：match 表达式
来源：http://hz.hongshengwenyu.top/gtsbvfmpwu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.feifeiyinyue.top/gtolklddif.html

[U56] PHP：命名参数
来源：http://hz.jinqigufen.top/gtslhuojck.html

f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtwpezmrgp.html

[U57] PHP：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtrmkcpvqr.html

"值: {$a}"
来源：http://hz.jqgufenzy.top/gtlsqbpizp.html

[U58] PHP：数组三件套
来源：http://hz.chenzaomai.com/gtlyblsdam.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.shanyushiyangtech.top/gtrckcpbgf.html

[U59] PHP：自定义排序
来源：http://hz.guannengcc.top/gtbfdwfnvz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.andypj.xyz/gtgnfwhotl.html

[U60] PHP：JSON 编解码
来源：http://hz.nwbrower.top/gtupnaqdqn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.vqdsnc.cn/gtekwfiodd.html

[U61] PHP：正则
来源：http://hz.ivvv.top/gtjvyeebgf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtmgsvugir.html

[U62] PHP：日期对象
来源：http://hz.yongpay.top/gtmsfsgrvn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.cdnleiting.top/gtxteiqruj.html

[U63] PHP：文件读写
来源：http://hz.ehwqpu.com/gtizvqnmrv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.kuanghao11.cn/gtzxeitpoq.html

[U64] PHP：目录遍历
来源：http://hz.52xcode.cn/gtdvfcrhvy.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.ppjwa.cn/gtljtzlkny.html

[U65] PHP：会话
来源：http://hz.pengpengdd.cyou/gtnrqlhqsc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.snrcjt.cn/gtyhbtoycv.html

[U66] PHP：设置 Cookie
来源：http://hz.jqgfzy.top/gttocasjqi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yangfankeji.com/gtmevykqgq.html

[U67] PHP：处理文件上传
来源：http://hz.daria6918.cn/gtpzsazrvu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jianghu66.top/gttobcymen.html

[U68] PHP：PDO 连接
来源：http://hz.gogol.net.cn/gtbqhdsneo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aizwys.cn/gtdoituewr.html

[U69] PHP：PDO 预处理
来源：http://hz.ppjwa.cn/gtdzfmzdoy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.meibo888.top/gtdqtnxudr.html

[U70] PHP：PDO 事务
来源：http://hz.aibaodan.cn/gtxnxihtit.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.cheryme.top/gtvopadpai.html

[U71] PHP：抛出异常
来源：http://hz.cheryme.top/gtkaqjawjp.html

throw new RuntimeException("失败", 500);
来源：http://hz.hysaishi.cn/gtucmdgztm.html

[U72] PHP：写错误日志
来源：http://hz.yuxming.cn/gtbidjdywk.html

error_log("失败: " . $e->getMessage());
来源：http://hz.aizwys.cn/gtogketqpd.html


<!-- 参考信息 -->