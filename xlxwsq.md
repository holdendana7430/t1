代发 wailian999

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtwtlcfatf.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gtcqnwkauq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtyawavicj.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtickfwqwa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtnhwxrumj.html

[S51] C++：显式类型转换
来源：http://hz.kuanghao11.cn/gtxxsejryz.html

static_cast<double>(a) / b
来源：http://hz.haohaochexian.top/gtaefsgolo.html

[S52] C++：const 与 noexcept
来源：http://hz.chenlongwang.top/gtgjuuvopo.html

int size() const noexcept { return n_; }
来源：http://hz.pengpengdd.cyou/gtpgixmgwj.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gteagynksn.html

std::vector<int> w = std::move(v);
来源：http://hz.chenjidiqi.icu/gtmhvnnxpo.html

[S54] C++：异常处理
来源：http://hz.daxiang520.top/gttfqoefwt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gotoacloud.top/gtjocusedd.html

[S55] C++：结构化绑定
来源：http://hz.52xcode.cn/gtbfwbrvel.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ppjwa.cn/gtnbgebxcc.html

[S56] C++：optional
来源：http://hz.zhiwuduotai.top/gtigenqnpq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.daria6918.cn/gtytyukkop.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtfisyziqn.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gtlqbmhzpx.html

[S58] C++：命名空间
来源：http://hz.nanxinkj.top/gtfglogect.html

namespace ns { int f() { return 1; } }
来源：http://hz.dianchejie.cn/gtkpuxnpao.html

[S59] C++：静态断言
来源：http://hz.jqgfzy.top/gtqgidrrbw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtoxgvdpwu.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gtrxsepqwv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtspdftkqo.html

================================================================================
来源：http://hz.ivvv.top/gtsilebxli.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yuanzhike.top/gtguslsvlc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtbdpwlxsa.html

[T01] Kotlin：Hello World
来源：http://hz.tian-w.cn/gtixnhdule.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtvjjuchjd.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtcfvzdkiq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yvedp.cn/gtvminosdk.html

[T03] Kotlin：字符串模板
来源：http://hz.zhoulong.xyz/gtxyezrmgd.html

"值: $b"
来源：http://hz.hammf.cn/gtyizidwxr.html

[T04] Kotlin：空安全
来源：http://hz.zhijiandao.cn/gtvoejyjfj.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtqjnmpwke.html

[T05] Kotlin：when 表达式
来源：http://hz.nanxinkj.top/gtehxxmpkv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtptomxgha.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gtnbmgzgid.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtlagxxqxh.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gtifnckrjs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtnnosgqde.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtsjqklvpv.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gtqbssxzty.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtwwxygyww.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtxjmolkdk.html

[T10] Kotlin：默认参数
来源：http://hz.zdqjudy.top/gtztaahwuk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtzfzrpzfx.html

[T11] Kotlin：协程
来源：http://hz.dianchejie.cn/gtalhttjja.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.birdmap.top/gtptciqxpl.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangtech.top/gtufjhhxyi.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtcfxaqiao.html

[T13] Kotlin：只读 Map
来源：http://hz.aizwys.cn/gtmixswlhz.html

val m = mapOf("a" to 1)
来源：http://hz.snrcjt.cn/gthyexnfid.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtuhyquyjs.html

for (i in 1..10) println(i)
来源：http://hz.dashuyun.cn/gtitqtixoj.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtngrzxhjc.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtbgmhmynm.html

[T16] Swift：Hello World
来源：http://hz.snrcjt.cn/gtxbosllnz.html

print("Hello")
来源：http://hz.cashguo.top/gtwyyiatvh.html

[T17] Swift：变量与常量
来源：http://hz.ppjwa.cn/gtpwahlbsp.html

var a = 1;  let b = 2
来源：http://hz.redwolf501.top/gtoccsedps.html

[T18] Swift：字符串插值
来源：http://hz.zhijiandao.cn/gtrffmoqjg.html

"值: \(b)"
来源：http://hz.hammf.cn/gtqlahjrqd.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtminvpdng.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtjfbaiitx.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtbycrnljb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cdnleiting.top/gtoqfwyggn.html

[T21] Swift：遍历
来源：http://hz.fengsongda.top/gteaxcaqwf.html

for x in a { print(x) }
来源：http://hz.redwolf501.top/gtetqjikrs.html

[T22] Swift：字典
来源：http://hz.c1oappe.top/gtpscplolt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gtgmvrkvvg.html

[T23] Swift：函数
来源：http://hz.ivvv.top/gttjtgfeos.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gtmebijazb.html

[T24] Swift：闭包
来源：http://hz.havefunace.top/gtuevrglfv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgfzy.top/gtmxewpoqf.html

[T25] Swift：结构体
来源：http://hz.dashuyun.cn/gtslavhczi.html

struct P { var x: Int }
来源：http://hz.jyoumei.cn/gtdhkmknva.html

[T26] Swift：类与重写
来源：http://hz.jqgufenzy.top/gtyxirnpbq.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtppqfyyvs.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtvtzypmrt.html

do { try f() } catch { print(error) }
来源：http://hz.cashguo.top/gtykseuzgc.html

[T28] Swift：枚举
来源：http://hz.ybcxt.top/gtjsbsqqob.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtkemdcupu.html

[T29] Swift：guard 提前返回
来源：http://hz.nanxinkj.top/gtjjviljov.html

guard let x = opt else { return }
来源：http://hz.ybcxt.top/gtruvwyzsq.html

[T30] Swift：协议
来源：http://hz.jinyuanbaomall.cn/gtpywlasqk.html

protocol Shape { func area() -> Double }
来源：http://hz.yvedp.cn/gtqcizvpzi.html

[T31] Lua：Hello World
来源：http://hz.cashguo.top/gtjjcopkin.html

print("Hello")
来源：http://hz.316326.xyz/gtvcqlvdwr.html

[T32] Lua：局部变量
来源：http://hz.sysykeji.top/gtkzlyraed.html

local a = 1
来源：http://hz.hongshengwenyu.top/gtdbxzjebc.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gttnqgwvte.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtokbybazt.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtvaxjnqck.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.feifeiyinyue.top/gtdatbpvey.html

[T35] Lua：字典表
来源：http://hz.dashuyun.cn/gtvxungapk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuxming.cn/gtzgxjfqzf.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtzcpqntim.html

function add(a, b) return a + b end
来源：http://hz.quarkkingdee.top/gtwutybmiu.html

[T37] Lua：字符串拼接
来源：http://hz.mhx1999.top/gtttggpjtr.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtcghpdacu.html

[T38] Lua：条件
来源：http://hz.sxryk.cn/gtbfjrjgxr.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtmqkbdyfq.html

[T39] Lua：模式匹配
来源：http://hz.mhx1999.top/gtksyeipde.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtovfbjmlm.html

[T40] Lua：元表
来源：http://hz.yongpay.top/gtzhvhyifo.html

setmetatable({}, { __index = base })
来源：http://hz.chenzaomai.com/gtycfwdmzx.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtpttumjif.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtlgytlkto.html

[T42] Perl：变量类型
来源：http://hz.zhoulong.xyz/gtfsrbiwqb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.redwolf501.top/gtkjdwytrd.html

[T43] Perl：字符串插值
来源：http://hz.hnqzz.top/gtfdgkexkm.html

"值: $a"
来源：http://hz.zhiwuduotai.top/gtzswlfosi.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gtckxqqvvb.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258888.top/gtwrsjorfw.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtbivsdtvn.html

for my $x (@arr) { print $x; }
来源：http://hz.c1oappe.top/gtnazharjo.html

[T46] Perl：哈希操作
来源：http://hz.zhixingplan.top/gtdncgkaun.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yvedp.cn/gtncqnnpfl.html

[T47] Perl：正则捕获
来源：http://hz.yuanzhike.top/gtuzmptuee.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jianghu66.top/gtwbiyblrp.html

[T48] Perl：正则替换
来源：http://hz.yuanzhike.top/gtuefrhsjv.html

$s =~ s/old/new/g;
来源：http://hz.hnxiangtu.top/gtjbkblvim.html

[T49] Perl：函数
来源：http://hz.shanyushiyangkeji.top/gtifvhqtwe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.andypj.xyz/gtocxgcclo.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gtqhfsexbc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xziqi.cn/gthaxzwser.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.c1oappe.top/gtyjzncguf.html

[T51] Scala：Hello World
来源：http://hz.ppjwa.cn/gtjcmtefxk.html

println("Hello")
来源：http://hz.guowangkeji.top/gtslkfycsc.html

[T52] Scala：变量
来源：http://hz.vqdsnc.cn/gtzflgwgev.html

val a = 1;  var b = 2
来源：http://hz.c1oappe.top/gtseveskof.html

[T53] Scala：字符串插值
来源：http://hz.birdmap.top/gtnflnrfrk.html

s"值: $b"
来源：http://hz.guannengcc.top/gtdueidiuj.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtuzkfqpyw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtgllqzgfn.html

[T55] Scala：集合过滤
来源：http://hz.ybcxt.top/gtxkqqrida.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.gotoacloud.top/gtfrdklcea.html

[T56] Scala：样例类
来源：http://hz.zhixingplan.top/gtccvpvvrr.html

case class User(name: String, age: Int)
来源：http://hz.pengpengdd.cyou/gtmkelmjux.html

[T57] Scala：模式匹配
来源：http://hz.ppjwa.cn/gtfhkgtaep.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.havefunace.top/gtklsxljsr.html

[T58] Scala：函数定义
来源：http://hz.chenjidiqi.icu/gtejgkukag.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.nanxinkj.top/gtkgtmiuxn.html

[T59] Scala：循环
来源：http://hz.shzxlz.cn/gtvrgdkofw.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhengqikj.top/gtkaywiasp.html

[T60] Scala：折叠
来源：http://hz.iojbl.cn/gtizuiorgu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.pengpengdd.cyou/gtudfbsdfr.html

================================================================================
来源：http://hz.xylfe.cn/gtokbbczmk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yvedp.cn/gtvababcbw.html

================================================================================
来源：http://hz.dashuyun.cn/gtymhqueeh.html

[U01] Py：创建虚拟环境
来源：http://hz.guowangkeji.top/gtvudqhfro.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhongyouzk.top/gtdavdjojr.html

[U02] Py：导出 / 安装依赖
来源：http://hz.mhx1999.top/gtpwvvaqpf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.tanke756.top/gthibfccuv.html

[U03] Py：加载 .env 配置
来源：http://hz.yuxming.cn/gtqfaescwl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yueranfly.top/gtcbuhvsuc.html

[U04] Py：变量调试打印
来源：http://hz.cashguo.top/gtvasugnon.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gtmfppgnsw.html

[U05] Py：列表去重且保序
来源：http://hz.jlsjyb.cn/gtuoyparxo.html

list(dict.fromkeys(arr))
来源：http://hz.ybcxt.top/gtljgxyevh.html

[U06] Py：合并两个字典
来源：http://hz.dashuyun.cn/gtjsmjsuev.html

{**a, **b}
来源：http://hz.zhaomingkeji.xyz/gtbrqnllkx.html

[U07] Py：反转字典键值
来源：http://hz.fengsongda.top/gtaivpzmtf.html

{v: k for k, v in d.items()}
来源：http://hz.feifeiyinyue.top/gtfwwkjssz.html

[U08] Py：展平二维列表
来源：http://hz.pycfn.com/gtbsmldobi.html

[y for x in nested for y in x]
来源：http://hz.yj20258888.top/gtmfgmikmx.html

[U09] Py：字典取最大值的键
来源：http://hz.zhengqikj.top/gtsgxstgji.html

max(d, key=d.get)
来源：http://hz.birdmap.top/gtfcgemjvm.html

[U10] Py：按值排序字典
来源：http://hz.zycfv.cn/gtehvniant.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhijiandao.cn/gttwfmqtia.html

[U11] Py：生成器表达式
来源：http://hz.tanke756.top/gtwbhjueun.html

(x * 2 for x in arr)
来源：http://hz.yj20258.top/gtortsazis.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhiwuduotai.top/gtydnnitvd.html

Counter(arr).most_common(3)
来源：http://hz.fzhhl.top/gtdosxlsux.html

[U13] Py：固定长度队列
来源：http://hz.guannengcc.top/gtdnztehll.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gtbmdtwzdc.html

[U14] Py：分组收集到列表
来源：http://hz.ehwqpu.com/gtkcisdbyy.html

defaultdict(list)
来源：http://hz.jinqigfzy.top/gtwwcrhxgt.html

[U15] Py：高精度计时
来源：http://hz.yj202588.top/gtmllldiil.html

t = time.perf_counter()
来源：http://hz.sysykeji.top/gtrficdsjb.html

[U16] Py：命令行参数解析
来源：http://hz.zhoulong.xyz/gtjndqxzfz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yongpay.top/gtxxjucmwy.html

[U17] Py：初始化日志
来源：http://hz.kuanghao11.cn/gtahgnhtuz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.hfpthk.cn/gtseulrzbo.html

[U18] Py：预编译正则
来源：http://hz.zhoulong.xyz/gtdiwerxma.html

pat = re.compile(r"\d+")
来源：http://hz.chenzaomai.com/gtdfpyfbla.html

[U19] Py：正则替换带回调
来源：http://hz.aibaodan.cn/gtxpzhoxwl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.dianchejie.cn/gtfmsdnpwp.html

[U20] Py：缓存函数结果
来源：http://hz.shangyingyoupin.top/gteeztgkbz.html

@functools.lru_cache(maxsize=None)
来源：http://hz.guannengcc.top/gttsawswas.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhixingplan.top/gtsycoainp.html

@contextlib.contextmanager
来源：http://hz.bjfxy.top/gtemzrjjfo.html

[U22] Py：矩阵转置
来源：http://hz.yanxiufei.cn/gtvlbtmpvo.html

list(zip(*m))
来源：http://hz.ybcxt.top/gtqmiedjvv.html

[U23] Py：分块读取大文件
来源：http://hz.chenjidiqi.icu/gtnecdkvox.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.fengsongda.top/gtrivbzdtd.html

[U24] Py：路径操作
来源：http://hz.ehwqpu.com/gtekbpznsg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xuanzx.com/gtgrlydwtk.html

[U25] Py：CSV 按字典读
来源：http://hz.chenzaomai.com/gtllciruha.html

csv.DictReader(f)
来源：http://hz.xingfuxueyuan.xyz/gteyzmhydb.html

[U26] Py：并发下载
来源：http://hz.tian-w.cn/gttrlqejjg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.quarkkingdee.top/gtbrcnbyev.html

[U27] Py：异步 HTTP
来源：http://hz.yj202588.top/gtderhgcvw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.meibo888.top/gtfvidslhn.html

[U28] Py：类型别名
来源：http://hz.zycfv.cn/gtygwoovck.html

UserId = int
来源：http://hz.andypj.xyz/gtnzlmrpmi.html

[U29] Py：属性校验
来源：http://hz.gzhubu.top/gtmiaijbdt.html

@property 与 @x.setter 配合
来源：http://hz.sweek.top/gtzvhcuggz.html

[U30] Py：数据类
来源：http://hz.zdqjudy.top/gtqzxqrbth.html

@dataclass(slots=True)
来源：http://hz.yangfankeji.com/gtdlporwvv.html

[U31] Py：单测
来源：http://hz.fengsongda.top/gtjddvqvds.html

python -m pytest -q
来源：http://hz.shzxlz.cn/gttaqpfkkr.html

[U32] Py：代码格式化
来源：http://hz.yvedp.cn/gttxekjymq.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtrpuhnxsx.html

[U33] Py：打包发布
来源：http://hz.snrcjt.cn/gtrjaemhma.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhaomingkeji.xyz/gtjnlrgdsu.html

[U34] Py：判断编码
来源：http://hz.fengsongda.top/gtsflqxgrl.html

chardet.detect(raw)
来源：http://hz.smart0.xyz/gtvwsajnyw.html

[U35] Py：发送邮件
来源：http://hz.birdmap.top/gtldtjdvdm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuetiantiany.cn/gtpeyxiddv.html

[U36] Py：定时任务
来源：http://hz.tanke756.top/gttdfcmeib.html

schedule.every(10).minutes.do(job)
来源：http://hz.sufxvd.cn/gtpsrynpav.html

[U37] Py：读写 Excel
来源：http://hz.nanxinkj.top/gtgagwzgbo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jinghuilouyu.cn/gtprqdpodd.html

[U38] Py：获取脚本所在目录
来源：http://hz.ivvv.top/gtlfuozalg.html

Path(__file__).resolve().parent
来源：http://hz.shuidangran.top/gtruczcglm.html

[U39] Py：判断是否在交互环境
来源：http://hz.hysaishi.cn/gttsfeigrb.html

sys.stdout.isatty()
来源：http://hz.hongshengwenyu.top/gtdfjcbdky.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gtekhmtgyu.html

print("err", file=sys.stderr)
来源：http://hz.aizwys.cn/gtwevnuqli.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sweek.top/gtzgozchox.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhongyouzk.top/gtxeuyrzcz.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ywan-chungtsiang.top/gtnmhiqmhy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhiwuduotai.top/gtcyjcchtm.html

[U43] PHP：声明命名空间
来源：http://hz.dianchejie.cn/gtcsypgoog.html

namespace App\Http;
来源：http://hz.pengpengdd.cyou/gtjtsmrqbg.html

[U44] PHP：开启严格类型
来源：http://hz.9152youxi.cn/gtvvchduig.html

declare(strict_types=1);
来源：http://hz.pengpengdd.cyou/gtjqwnjjhx.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shangyingyoupin.top/gtwjpltqwn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtkacmnusy.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gtdwlxnnjw.html

?string $name = null
来源：http://hz.jlsjyb.cn/gtvjipbmjo.html

[U47] PHP：联合类型
来源：http://hz.quarkkingdee.top/gtqmzmuqxs.html

int|string $id
来源：http://hz.yuanzhike.top/gtyteyxiuv.html

[U48] PHP：纯枚举
来源：http://hz.c1oappe.top/gtoprshelx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.dashuyun.cn/gtkteoqmls.html

[U49] PHP：只读属性
来源：http://hz.yongpay.top/gtyxxymybx.html

public readonly string $name
来源：http://hz.jinqigufen.top/gtkbhranbb.html

[U50] PHP：构造器属性提升
来源：http://hz.zhoulong.xyz/gtsqnalcdm.html

public function __construct(private int $id) {}
来源：http://hz.gzhubu.top/gtzerjcjfq.html

[U51] PHP：数组解构
来源：http://hz.cashguo.top/gtgtinizyv.html

[$a, $b] = $arr;
来源：http://hz.xingfuxueyuan.xyz/gtrkdadecc.html

[U52] PHP：箭头函数
来源：http://hz.tianlin.xyz/gtbaxiskha.html

$double = fn($x) => $x * 2;
来源：http://hz.dianchejie.cn/gtxdhmmckd.html

[U53] PHP：空合并运算符
来源：http://hz.shuidangran.top/gtrnrrrqeg.html

$v = $a ?? $b ?? "default";
来源：http://hz.shanyushiyangkeji.top/gtxfikiqbx.html

[U54] PHP：空安全调用
来源：http://hz.daria6918.cn/gtantxbnoz.html

$obj?->method()
来源：http://hz.xingfuxueyuan.xyz/gtiircdzrf.html

[U55] PHP：match 表达式
来源：http://hz.yonumen.top/gtecrrqdae.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ppjwa.cn/gtoihisplg.html

[U56] PHP：命名参数
来源：http://hz.birdmap.top/gtgteskhbe.html

f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtcighwetq.html

[U57] PHP：字符串插值
来源：http://hz.tianlin.xyz/gtmhcwaugu.html

"值: {$a}"
来源：http://hz.hywenlv.cn/gtjmuxlglp.html

[U58] PHP：数组三件套
来源：http://hz.cucudq.cn/gtpgoczdje.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.kuanghao11.cn/gtooezoehb.html

[U59] PHP：自定义排序
来源：http://hz.shzxlz.cn/gtfxgsxezo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gtnbwsaizx.html

[U60] PHP：JSON 编解码
来源：http://hz.zhiwuduotai.top/gtimeutuzi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhijiandao.cn/gtoxgwphnz.html

[U61] PHP：正则
来源：http://hz.yuxming.cn/gtladkgfnz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.bjfxy.top/gtbmznukhl.html

[U62] PHP：日期对象
来源：http://hz.cqqwz.cn/gtycxyplnb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ybcxt.top/gtoguqnhch.html

[U63] PHP：文件读写
来源：http://hz.zycfv.cn/gtfuniyoqh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.0kj1m.cn/gtbxbrmabw.html

[U64] PHP：目录遍历
来源：http://hz.gzhubu.top/gtxfrwcivl.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.aibaodan.cn/gtvrtjbbxa.html

[U65] PHP：会话
来源：http://hz.bjfxy.top/gtidpvywwf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ehwqpu.com/gtvxtibsmw.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtigfalbru.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.hongshengwenyu.top/gtimhmwrds.html

[U67] PHP：处理文件上传
来源：http://hz.jiagoushi.top/gtnlangfmh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.smart0.xyz/gtsveqainp.html

[U68] PHP：PDO 连接
来源：http://hz.pycfn.com/gtbqplugke.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jiagoushi.top/gttqorqndw.html

[U69] PHP：PDO 预处理
来源：http://hz.ydzc1.top/gtzwobzigm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gotoacloud.top/gtvquzeiro.html

[U70] PHP：PDO 事务
来源：http://hz.gzhubu.top/gtoqhhzruj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.hongshengwenyu.top/gttkvbwnlk.html

[U71] PHP：抛出异常
来源：http://hz.shangyingyoupin.top/gtylkulbli.html

throw new RuntimeException("失败", 500);
来源：http://hz.jinyuanbaomall.cn/gtsodrliam.html

[U72] PHP：写错误日志
来源：http://hz.yvedp.cn/gtsnocxnbi.html

error_log("失败: " . $e->getMessage());
来源：http://hz.zycfv.cn/gtwehxcpiy.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigfzy.top/gtgutbgxhv.html

parse_ini_file("config.ini", true)
来源：http://hz.redwolf501.top/gtxtqhbscq.html

[U74] PHP：读取环境变量
来源：http://hz.wangdashe.top/gtkcujvhfm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sweek.top/gtujqjgkxb.html


<!-- 参考信息 -->