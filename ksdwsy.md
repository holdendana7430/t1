代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtwnnrbfqz.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtfcmbzewm.html

static_cast<double>(a) / b
来源：http://hz.jinqigufen.top/gtpotjhdvx.html

[S52] C++：const 与 noexcept
来源：http://hz.gotoacloud.top/gtugazkgdj.html

int size() const noexcept { return n_; }
来源：http://hz.cheryme.top/gtyfiyrsch.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtlivhcbrs.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtsqkpydib.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtmnleennh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.316326.xyz/gtltcsdugh.html

[S55] C++：结构化绑定
来源：http://hz.haohaochexian.top/gtihrrxihj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.meibo888.top/gtbcptqhhq.html

[S56] C++：optional
来源：http://hz.yj202588.top/gthnwbijnl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtfambetxb.html

[S57] C++：编译期常量
来源：http://hz.pycfn.com/gtqmqkuucw.html

constexpr int N = 10;
来源：http://hz.guannengcc.top/gtrjpcwvnr.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangkeji.top/gtbhvvjvqp.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtlpgaoenj.html

[S59] C++：静态断言
来源：http://hz.aizwys.cn/gtvartvjiy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtjayawamy.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtspowatyq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtcmbrymxj.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmdjojfvi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yanxiufei.cn/gtsosqcttv.html

================================================================================
来源：http://hz.zhixingplan.top/gtwduextuw.html

[T01] Kotlin：Hello World
来源：http://hz.ppjwa.cn/gtthwhzkfu.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtgpenbwdm.html

[T02] Kotlin：变量
来源：http://hz.guannengcc.top/gtgxwdzdaq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtyzjmukqn.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtiotwslvn.html

"值: $b"
来源：http://hz.smart0.xyz/gtsxiqybun.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtcoixwhkj.html

val n: String? = null;  n?.length
来源：http://hz.chenzaomai.com/gtgqxtpumn.html

[T05] Kotlin：when 表达式
来源：http://hz.nwbrower.top/gtjwdxavoh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hysaishi.cn/gtygczxqyo.html

[T06] Kotlin：集合映射
来源：http://hz.tanke756.top/gtcoeypjlw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hysaishi.cn/gtirrqsqjw.html

[T07] Kotlin：集合过滤
来源：http://hz.kuanghao11.cn/gtkzrleefk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtyphmnajb.html

[T08] Kotlin：数据类
来源：http://hz.yanxiufei.cn/gtxotcauzg.html

data class User(val name: String, val age: Int)
来源：http://hz.hnqzz.top/gtctbpovmc.html

[T09] Kotlin：扩展函数
来源：http://hz.316326.xyz/gtaeekywif.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtqfdfdosm.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gtyhupkcre.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.0kj1m.cn/gteojvmgup.html

[T11] Kotlin：协程
来源：http://hz.feifeiyinyue.top/gtfwilkdcr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.tian-w.cn/gtfepiaqec.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtxrjpupeq.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydzc1.top/gtvvbdfbyd.html

[T13] Kotlin：只读 Map
来源：http://hz.redwolf501.top/gtvadlzwdr.html

val m = mapOf("a" to 1)
来源：http://hz.nanxuanxn.top/gtcbisyvxd.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gthlktlfcm.html

for (i in 1..10) println(i)
来源：http://hz.nanxuanxn.top/gtxclzxowe.html

[T15] Kotlin：接口
来源：http://hz.xuetiantiany.cn/gtcrchbibx.html

interface Shape { fun area(): Double }
来源：http://hz.xinyue.icu/gtujbvpequ.html

[T16] Swift：Hello World
来源：http://hz.redwolf501.top/gtugjbfiik.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtmeovyucy.html

[T17] Swift：变量与常量
来源：http://hz.chenjidiqi.icu/gtuqmbglux.html

var a = 1;  let b = 2
来源：http://hz.ywan-chungtsiang.top/gtlwhfkyox.html

[T18] Swift：字符串插值
来源：http://hz.yj20258888.top/gtmmkhoaqs.html

"值: \(b)"
来源：http://hz.316326.xyz/gtigrwyxxt.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtfcbkbjba.html

if let n = opt { print(n) }
来源：http://hz.iojbl.cn/gtgyibflrq.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtkrzmgoih.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtcbkadlqo.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtgmdbbcax.html

for x in a { print(x) }
来源：http://hz.0kj1m.cn/gthxphawdd.html

[T22] Swift：字典
来源：http://hz.nwbrower.top/gtvffwvyxq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtiwwpvula.html

[T23] Swift：函数
来源：http://hz.chenjidiqi.icu/gthigkvkcu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtnxmerfsx.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gtgzcqdoba.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinqigfzy.top/gtfxkmanhg.html

[T25] Swift：结构体
来源：http://hz.shzxlz.cn/gtbwjoxpjl.html

struct P { var x: Int }
来源：http://hz.cucudq.cn/gtisxotkdg.html

[T26] Swift：类与重写
来源：http://hz.yueranfly.top/gtuzymyfah.html

class A: Base { override func f() {} }
来源：http://hz.jinyuanbaomall.cn/gtijqqplxu.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gtklujkqhi.html

do { try f() } catch { print(error) }
来源：http://hz.xuetiantiany.cn/gtuebkutjk.html

[T28] Swift：枚举
来源：http://hz.yj202588.top/gtmfiutvpr.html

enum Color { case red, green }
来源：http://hz.shanyushiyangkeji.top/gtryuaigpk.html

[T29] Swift：guard 提前返回
来源：http://hz.snrcjt.cn/gtjoucdmfu.html

guard let x = opt else { return }
来源：http://hz.ywan-chungtsiang.top/gtxgzomxtj.html

[T30] Swift：协议
来源：http://hz.shanyushiyangkeji.top/gttikszaoo.html

protocol Shape { func area() -> Double }
来源：http://hz.52xcode.cn/gtylsuxmve.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtqajtxxba.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gttnlizmnf.html

[T32] Lua：局部变量
来源：http://hz.guowangkeji.top/gtlwxupjzy.html

local a = 1
来源：http://hz.yongpay.top/gtctxyctzh.html

[T33] Lua：表（数组）
来源：http://hz.yueranfly.top/gtegeghazf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinqigufen.top/gtuznizfts.html

[T34] Lua：遍历表
来源：http://hz.cashguo.top/gtildjshgf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnqzz.top/gtphhdofjg.html

[T35] Lua：字典表
来源：http://hz.sufxvd.cn/gtmxzjkjic.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fengsongda.top/gtvlstowwl.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtexexdejj.html

function add(a, b) return a + b end
来源：http://hz.xuanzx.com/gtdhcqzzfo.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtocpplylz.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtiznajaue.html

[T38] Lua：条件
来源：http://hz.shuidangran.top/gtvkjrwrer.html

if x > 0 then print("正") end
来源：http://hz.jqgfzy.top/gtzhhszfuw.html

[T39] Lua：模式匹配
来源：http://hz.ydjk.org.cn/gtoldzfpsp.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtuanjfvaw.html

[T40] Lua：元表
来源：http://hz.jiagoushi.top/gtjfqpmaqr.html

setmetatable({}, { __index = base })
来源：http://hz.9152youxi.cn/gtvfefjheg.html

[T41] Perl：Hello World
来源：http://hz.haohaochexian.top/gtsnsehhvb.html

print "Hello\n";
来源：http://hz.smart0.xyz/gtcayysvop.html

[T42] Perl：变量类型
来源：http://hz.daxiang520.top/gtqfehfwya.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinyuanbaomall.cn/gtccovmmkg.html

[T43] Perl：字符串插值
来源：http://hz.tian-w.cn/gtkkladkwf.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtfoqkfsda.html

[T44] Perl：条件
来源：http://hz.zhoulong.xyz/gtdqzwtday.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtbjsgcfmc.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gtnwmfdtxm.html

for my $x (@arr) { print $x; }
来源：http://hz.guannengcc.top/gtwlvfzauu.html

[T46] Perl：哈希操作
来源：http://hz.cdnleiting.top/gtiihheapm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.wangdashe.top/gtcdeghxgb.html

[T47] Perl：正则捕获
来源：http://hz.jqgfzy.top/gtqsrunbxv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xinyue.icu/gtgwqnuizm.html

[T48] Perl：正则替换
来源：http://hz.jinghuilouyu.cn/gtfvhchhju.html

$s =~ s/old/new/g;
来源：http://hz.yj20258888.top/gtnegfdsow.html

[T49] Perl：函数
来源：http://hz.shuidangran.top/gtcpfuzhnn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yangfankeji.com/gtascbketx.html

[T50] Perl：逐行读文件
来源：http://hz.cheryme.top/gtpqoeoubv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.wangshuangyany.cn/gtzgdqpsdp.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.fzhhl.top/gtqngbpwms.html

[T51] Scala：Hello World
来源：http://hz.xylfe.cn/gthazyneao.html

println("Hello")
来源：http://hz.dianchejie.cn/gtwjvlqtmk.html

[T52] Scala：变量
来源：http://hz.shzxlz.cn/gtenouqolb.html

val a = 1;  var b = 2
来源：http://hz.hongshengwenyu.top/gtwrowkjaa.html

[T53] Scala：字符串插值
来源：http://hz.gaohongyu789.top/gtxpfujpfv.html

s"值: $b"
来源：http://hz.yongpay.top/gtzedutabx.html

[T54] Scala：集合映射
来源：http://hz.52xcode.cn/gtwslrowev.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.nanxinkj.top/gtrxbzeogz.html

[T55] Scala：集合过滤
来源：http://hz.dashuyun.cn/gtcvkuyrvu.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.zhiwuduotai.top/gtzzwopwnt.html

[T56] Scala：样例类
来源：http://hz.daxiang520.top/gtpgmohuyu.html

case class User(name: String, age: Int)
来源：http://hz.snrcjt.cn/gtqeigmvrm.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gtufgttszt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xziqi.cn/gtjsyndbjf.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtkeruodjv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.svipenyu.cn/gtrjlkobpo.html

[T59] Scala：循环
来源：http://hz.yuxming.cn/gtmkqxkjtj.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenlongwang.top/gtidbyvefa.html

[T60] Scala：折叠
来源：http://hz.dashuyun.cn/gtfskcbevu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinqigfzy.top/gtyzrmrvqv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtoacmygzc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yonumen.top/gtzefkfckq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtsfzjitgb.html

[U01] Py：创建虚拟环境
来源：http://hz.wangdashe.top/gtcbjzbltk.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gtbkkzbkiv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.guannengcc.top/gtlkongjwy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.iojbl.cn/gtbiwhsren.html

[U03] Py：加载 .env 配置
来源：http://hz.fzhhl.top/gtppudsisr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ivvv.top/gtonacnatb.html

[U04] Py：变量调试打印
来源：http://hz.shangyingyoupin.top/gttahyrury.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jqgufenzy.top/gtvsxxtido.html

[U05] Py：列表去重且保序
来源：http://hz.hongshengwenyu.top/gtnzjqegei.html

list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gthmedblfo.html

[U06] Py：合并两个字典
来源：http://hz.sweek.top/gtwbkymaln.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtiwaplqud.html

[U07] Py：反转字典键值
来源：http://hz.quarkkingdee.top/gtjeadclup.html

{v: k for k, v in d.items()}
来源：http://hz.nanxuanxn.top/gtciuognzd.html

[U08] Py：展平二维列表
来源：http://hz.nanxinkj.top/gtfsmdsnxt.html

[y for x in nested for y in x]
来源：http://hz.ppjwa.cn/gtlrevuwwy.html

[U09] Py：字典取最大值的键
来源：http://hz.hywenlv.cn/gtjacjuqre.html

max(d, key=d.get)
来源：http://hz.yangfankeji.com/gtbikxjtyp.html

[U10] Py：按值排序字典
来源：http://hz.haohaochexian.top/gtcdsdvquf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.xziqi.cn/gtcnwwpdbq.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtrtqvcwrh.html

(x * 2 for x in arr)
来源：http://hz.bjfxy.top/gtdvxheuuf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jinqigfzy.top/gtnhmkaeii.html

Counter(arr).most_common(3)
来源：http://hz.cqqwz.cn/gtulmhlbph.html

[U13] Py：固定长度队列
来源：http://hz.jqgufenzy.top/gtzqfxnacc.html

deque(maxlen=10)
来源：http://hz.yueranfly.top/gtxyhfihnf.html

[U14] Py：分组收集到列表
来源：http://hz.tanke756.top/gtwsbszpmg.html

defaultdict(list)
来源：http://hz.yvedp.cn/gtwzwgqqjz.html

[U15] Py：高精度计时
来源：http://hz.sysykeji.top/gtmwggsxjk.html

t = time.perf_counter()
来源：http://hz.jinyuanbaomall.cn/gtfcghwdxu.html

[U16] Py：命令行参数解析
来源：http://hz.yuxming.cn/gtjbteiyty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.havefunace.top/gtrnuvshbj.html

[U17] Py：初始化日志
来源：http://hz.zycfv.cn/gtfyagxoiz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jianghu66.top/gtnrqjjqvp.html

[U18] Py：预编译正则
来源：http://hz.zdqjudy.top/gtcvgtjusk.html

pat = re.compile(r"\d+")
来源：http://hz.quarkkingdee.top/gtdlpvbgvd.html

[U19] Py：正则替换带回调
来源：http://hz.zycfv.cn/gtzitmnvgd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.kuanghao11.cn/gticxdkziy.html

[U20] Py：缓存函数结果
来源：http://hz.0kj1m.cn/gtafjwrwtu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jlsjyb.cn/gtxazvjlhe.html

[U21] Py：自定义上下文管理器
来源：http://hz.9152youxi.cn/gtyvsljorn.html

@contextlib.contextmanager
来源：http://hz.pengpengdd.cyou/gtvhepduuz.html

[U22] Py：矩阵转置
来源：http://hz.birdmap.top/gthxoswcgj.html

list(zip(*m))
来源：http://hz.jianghu66.top/gtvuugmbfl.html

[U23] Py：分块读取大文件
来源：http://hz.gaohongyu789.top/gtexcuzijl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.aibaodan.cn/gtdhjlsdst.html

[U24] Py：路径操作
来源：http://hz.chenlongwang.top/gtqbufuvmo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.meibo888.top/gtnjlrbimg.html

[U25] Py：CSV 按字典读
来源：http://hz.zhongyouzk.top/gthjwgahot.html

csv.DictReader(f)
来源：http://hz.cashguo.top/gtjxxhnbxw.html

[U26] Py：并发下载
来源：http://hz.hfpthk.cn/gtfxwwzosv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gotoacloud.top/gtfzmkuymt.html

[U27] Py：异步 HTTP
来源：http://hz.meibo888.top/gtgvwurdpr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhiwuduotai.top/gtspiiqbqt.html

[U28] Py：类型别名
来源：http://hz.jianghu66.top/gtshnawbwl.html

UserId = int
来源：http://hz.shuidangran.top/gtzepjdoqj.html

[U29] Py：属性校验
来源：http://hz.haohaochexian.top/gtmybjergb.html

@property 与 @x.setter 配合
来源：http://hz.daxiang520.top/gtatbkqivn.html

[U30] Py：数据类
来源：http://hz.xingfuxueyuan.xyz/gtrhftvsea.html

@dataclass(slots=True)
来源：http://hz.jianghu66.top/gtnmfzivzi.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gtgbyhjfxj.html

python -m pytest -q
来源：http://hz.jinghuilouyu.cn/gtosbwumyo.html

[U32] Py：代码格式化
来源：http://hz.aibaodan.cn/gtzpssojwd.html

ruff format . && ruff check --fix .
来源：http://hz.aibaodan.cn/gtuflkmhae.html

[U33] Py：打包发布
来源：http://hz.mhx1999.top/gtfdjlkvll.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.iojbl.cn/gtgqfpjxji.html

[U34] Py：判断编码
来源：http://hz.tian-w.cn/gtksglbqed.html

chardet.detect(raw)
来源：http://hz.mhx1999.top/gtmhzctxhh.html

[U35] Py：发送邮件
来源：http://hz.zhengqikj.top/gtxnzxlqzu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hnqzz.top/gtmwzfvqbl.html

[U36] Py：定时任务
来源：http://hz.chenjidiqi.icu/gtbqmsbwnl.html

schedule.every(10).minutes.do(job)
来源：http://hz.tian-w.cn/gtavvycodv.html

[U37] Py：读写 Excel
来源：http://hz.gogol.net.cn/gtwqlohcbz.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.kuanghao11.cn/gtwbyhtzft.html

[U38] Py：获取脚本所在目录
来源：http://hz.jqgfzy.top/gtwbanwogl.html

Path(__file__).resolve().parent
来源：http://hz.cdnleiting.top/gtnwwntkkn.html

[U39] Py：判断是否在交互环境
来源：http://hz.xingfuxueyuan.xyz/gtbticzxck.html

sys.stdout.isatty()
来源：http://hz.zhaomingkeji.xyz/gtiqjgjbkz.html

[U40] Py：打印到标准错误
来源：http://hz.ywan-chungtsiang.top/gtlagxeqzo.html

print("err", file=sys.stderr)
来源：http://hz.bjfxy.top/gtnhmsgzbw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.vqdsnc.cn/gtmwbueugf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fzhhl.top/gtfkpeeebv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gtsdyimuew.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ivvv.top/gtppcuuhvy.html

[U43] PHP：声明命名空间
来源：http://hz.jyoumei.cn/gtuxuxdxex.html

namespace App\Http;
来源：http://hz.yvedp.cn/gttecjevim.html

[U44] PHP：开启严格类型
来源：http://hz.gogol.net.cn/gtyqdbxftg.html

declare(strict_types=1);
来源：http://hz.zhaomingkeji.xyz/gtsefxnksn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.chenzaomai.com/gtixxiwgqm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtrdjeyqzm.html

[U46] PHP：可空类型
来源：http://hz.feifeiyinyue.top/gtpvnwxuid.html

?string $name = null
来源：http://hz.sysykeji.top/gtgozrtleg.html

[U47] PHP：联合类型
来源：http://hz.guannengcc.top/gtptdsfkfx.html

int|string $id
来源：http://hz.guannengcc.top/gtslvfkfhn.html

[U48] PHP：纯枚举
来源：http://hz.ydzc1.top/gtdwvnamiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aibaodan.cn/gtipxuiama.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gtmczwfvdr.html

public readonly string $name
来源：http://hz.hywenlv.cn/gtojuihtfl.html

[U50] PHP：构造器属性提升
来源：http://hz.yuanzhike.top/gtwpeogqhj.html

public function __construct(private int $id) {}
来源：http://hz.tianlin.xyz/gtzjsfsiob.html

[U51] PHP：数组解构
来源：http://hz.iojbl.cn/gttvfzqdeo.html

[$a, $b] = $arr;
来源：http://hz.yueranfly.top/gtqnqmqxqb.html

[U52] PHP：箭头函数
来源：http://hz.yanxiufei.cn/gtnvqoyotv.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtequzxtrj.html

[U53] PHP：空合并运算符
来源：http://hz.yj202588.top/gtzmdlaxbk.html

$v = $a ?? $b ?? "default";
来源：http://hz.tianlin.xyz/gtfuerolwo.html

[U54] PHP：空安全调用
来源：http://hz.hammf.cn/gtndkfssqh.html

$obj?->method()
来源：http://hz.andypj.xyz/gtzyauvoyu.html

[U55] PHP：match 表达式
来源：http://hz.jinqigfzy.top/gtyyceygrn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.shzxlz.cn/gtnugpqhhl.html

[U56] PHP：命名参数
来源：http://hz.ppjwa.cn/gtgpxsckxi.html

f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtluvyiqwa.html

[U57] PHP：字符串插值
来源：http://hz.xingfuxueyuan.xyz/gtjtcilmbc.html

"值: {$a}"
来源：http://hz.sufxvd.cn/gtmqixunyp.html

[U58] PHP：数组三件套
来源：http://hz.zhongyouzk.top/gtlhfxacxq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.fzhhl.top/gtubpzcizu.html

[U59] PHP：自定义排序
来源：http://hz.jiagoushi.top/gtlcqeizph.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yueranfly.top/gtiejuozcy.html

[U60] PHP：JSON 编解码
来源：http://hz.jinyuanbaomall.cn/gtzvgxdnid.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.316326.xyz/gtewedtmqh.html

[U61] PHP：正则
来源：http://hz.chenjidiqi.icu/gtfsfzjimj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtihnynyvt.html

[U62] PHP：日期对象
来源：http://hz.chenjidiqi.icu/gtvmnouvna.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hysaishi.cn/gtcepoqjht.html

[U63] PHP：文件读写
来源：http://hz.quarkkingdee.top/gthqouuovi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shanyushiyangkeji.top/gteatvpsdo.html

[U64] PHP：目录遍历
来源：http://hz.yueranfly.top/gtslrqxcru.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnqzz.top/gtkxpgmsrd.html

[U65] PHP：会话
来源：http://hz.hongshengwenyu.top/gtvbbhjudb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.jqgufenzy.top/gtrvrucxpk.html

[U66] PHP：设置 Cookie
来源：http://hz.jqgfzy.top/gtaohaoueb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yvedp.cn/gtbtfjpyba.html

[U67] PHP：处理文件上传
来源：http://hz.guowangkeji.top/gtldkpvrqx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhixingplan.top/gtvuljcllw.html

[U68] PHP：PDO 连接
来源：http://hz.xinyue.icu/gtqnnpyrgy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jlsjyb.cn/gtrpvvmdbn.html

[U69] PHP：PDO 预处理
来源：http://hz.fzhhl.top/gtrzeirugo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.nanxuanxn.top/gtydccezgz.html

[U70] PHP：PDO 事务
来源：http://hz.daxiang520.top/gtclglesjl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.iojbl.cn/gtmnsfravu.html

[U71] PHP：抛出异常
来源：http://hz.shzxlz.cn/gtoiunvaxy.html

throw new RuntimeException("失败", 500);
来源：http://hz.jiagoushi.top/gtsybhxrkq.html

[U72] PHP：写错误日志
来源：http://hz.quarkkingdee.top/gtwltnttos.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ehwqpu.com/gtfwnsmgnp.html

[U73] PHP：读取 ini 配置
来源：http://hz.hammf.cn/gtutirkjll.html

parse_ini_file("config.ini", true)
来源：http://hz.xuetiantiany.cn/gtdtrpxgxn.html

[U74] PHP：读取环境变量
来源：http://hz.bjfxy.top/gtqrpdlcyi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.xziqi.cn/gtnmldrmge.html

[U75] PHP：依赖注入
来源：http://hz.yangfankeji.com/gtdpdsnkqc.html

composer require psr/container
来源：http://hz.kuanghao11.cn/gtlzwqgxfl.html

[U76] PHP：简单路由
来源：http://hz.hammf.cn/gtvtkpylvr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.nanxuanxn.top/gttlkrykxw.html


<!-- 参考信息 -->