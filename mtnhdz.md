代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sysykeji.top/gtzwfqgyhg.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtofyfifjk.html

static_cast<double>(a) / b
来源：http://hz.hysaishi.cn/gtmqfkhoio.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gtxttudswm.html

int size() const noexcept { return n_; }
来源：http://hz.feifeiyinyue.top/gtepygsdxc.html

[S53] C++：移动语义
来源：http://hz.ydzc1.top/gtztsatrzy.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtfzduycff.html

[S54] C++：异常处理
来源：http://hz.snrcjt.cn/gtzdsjzsvd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenzaomai.com/gtkqofnnhj.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtsexhrspq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hfpthk.cn/gtvahatacs.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtxjbfduxx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xingfuxueyuan.xyz/gteztgkxgp.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gtqqxootak.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtkwpplwqj.html

[S58] C++：命名空间
来源：http://hz.zhoulong.xyz/gtrywzgxqf.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtpatsndbj.html

[S59] C++：静态断言
来源：http://hz.yongpay.top/gtpevlvpdn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hysaishi.cn/gtlviemmxg.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtolvrkjqs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hongshengwenyu.top/gtfcxtipin.html

================================================================================
来源：http://hz.redwolf501.top/gtlvgmhcdp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtnjosimig.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqzgteunm.html

[T01] Kotlin：Hello World
来源：http://hz.yuanzhike.top/gtjbkmrkri.html

println("Hello")
来源：http://hz.jiagoushi.top/gttqfjamqv.html

[T02] Kotlin：变量
来源：http://hz.xylfe.cn/gtciiodwxz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gaohongyu789.top/gtcndyqitt.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gtmlzunlqi.html

"值: $b"
来源：http://hz.yj202588.top/gtrgyqyesv.html

[T04] Kotlin：空安全
来源：http://hz.jinyuanbaomall.cn/gthvznxbrz.html

val n: String? = null;  n?.length
来源：http://hz.hnqzz.top/gtuyuuyhda.html

[T05] Kotlin：when 表达式
来源：http://hz.xinyue.icu/gtxbfrhfru.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnxiangtu.top/gtfzyzvlix.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtlirqfwoq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fzhhl.top/gtgofisuph.html

[T07] Kotlin：集合过滤
来源：http://hz.redwolf501.top/gthtqlkjmb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.snrcjt.cn/gtzxxtsqky.html

[T08] Kotlin：数据类
来源：http://hz.yonumen.top/gtdxzeryap.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtblkpotkj.html

[T09] Kotlin：扩展函数
来源：http://hz.chenjidiqi.icu/gtufrbenyq.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtnannzpyj.html

[T10] Kotlin：默认参数
来源：http://hz.gzhubu.top/gtkfijubrf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258888.top/gtdbkehewc.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gtyzzztdsi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gteqgruopf.html

[T12] Kotlin：解构声明
来源：http://hz.cheryme.top/gtpsudvklm.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenjidiqi.icu/gtksprgtkv.html

[T13] Kotlin：只读 Map
来源：http://hz.cdnleiting.top/gtgunzvgjb.html

val m = mapOf("a" to 1)
来源：http://hz.shzxlz.cn/gtksjskczd.html

[T14] Kotlin：循环
来源：http://hz.meibo888.top/gtlwrpqfal.html

for (i in 1..10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtpzuvacyq.html

[T15] Kotlin：接口
来源：http://hz.gzhubu.top/gtqdtdldsw.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtsjfvgppa.html

[T16] Swift：Hello World
来源：http://hz.cdnleiting.top/gtkgpbwykf.html

print("Hello")
来源：http://hz.aibaodan.cn/gtkbnaxvjg.html

[T17] Swift：变量与常量
来源：http://hz.9152youxi.cn/gtocrvugic.html

var a = 1;  let b = 2
来源：http://hz.c1oappe.top/gtucgovvyb.html

[T18] Swift：字符串插值
来源：http://hz.zdqjudy.top/gtlpjytabh.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gtodoslofw.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtrkmzhmwi.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtadbbwowa.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtxkftefud.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtlrqptpeq.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gtszlayvim.html

for x in a { print(x) }
来源：http://hz.daria6918.cn/gtkxhijzjo.html

[T22] Swift：字典
来源：http://hz.yuxming.cn/gtmkekjtsu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ivvv.top/gtfpajsxtn.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtncoeztgh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenlongwang.top/gtzbcbamcv.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtbfuxnsvc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xylfe.cn/gtvphjbnzp.html

[T25] Swift：结构体
来源：http://hz.ppjwa.cn/gtlsemuvvw.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtxsollwzq.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gthsgqxvwa.html

class A: Base { override func f() {} }
来源：http://hz.guannengcc.top/gtlmtmlhvv.html

[T27] Swift：错误处理
来源：http://hz.chenlongwang.top/gtqdcnjkls.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtpgwfvfkt.html

[T28] Swift：枚举
来源：http://hz.chenzaomai.com/gtgfxiupve.html

enum Color { case red, green }
来源：http://hz.chenjidiqi.icu/gtgralgend.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigufen.top/gtnnphvaje.html

guard let x = opt else { return }
来源：http://hz.xuanzx.com/gttivsglif.html

[T30] Swift：协议
来源：http://hz.zhixingplan.top/gtyxmkovcm.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gthurzjmra.html

[T31] Lua：Hello World
来源：http://hz.gzhubu.top/gtqrzsouxg.html

print("Hello")
来源：http://hz.yonumen.top/gtmwuwbdjm.html

[T32] Lua：局部变量
来源：http://hz.zdqjudy.top/gtuxofftwj.html

local a = 1
来源：http://hz.hammf.cn/gtpyagfsqe.html

[T33] Lua：表（数组）
来源：http://hz.kuanghao11.cn/gtvrgwcumc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guannengcc.top/gtsxsutzqk.html

[T34] Lua：遍历表
来源：http://hz.nwbrower.top/gtvcpndloa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jiagoushi.top/gtpacbfqct.html

[T35] Lua：字典表
来源：http://hz.gogol.net.cn/gtdzmhxnfb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ybcxt.top/gtilmuopeg.html

[T36] Lua：函数
来源：http://hz.daria6918.cn/gtsddlluuf.html

function add(a, b) return a + b end
来源：http://hz.yonumen.top/gtalwclvkz.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gtlbcwmgll.html

"a" .. "b"
来源：http://hz.yongpay.top/gtclxzaxmi.html

[T38] Lua：条件
来源：http://hz.jlsjyb.cn/gttusvmoym.html

if x > 0 then print("正") end
来源：http://hz.cqqwz.cn/gtrzrmrfnu.html

[T39] Lua：模式匹配
来源：http://hz.shuidangran.top/gtjhuzkupu.html

string.find(s, "%d+")
来源：http://hz.yonumen.top/gtlddvooho.html

[T40] Lua：元表
来源：http://hz.zhengqikj.top/gtqglxlsjc.html

setmetatable({}, { __index = base })
来源：http://hz.iojbl.cn/gtpyxcjtch.html

[T41] Perl：Hello World
来源：http://hz.xuetiantiany.cn/gtcgbgmmaq.html

print "Hello\n";
来源：http://hz.9152youxi.cn/gtzxrsxexf.html

[T42] Perl：变量类型
来源：http://hz.cashguo.top/gtlovwbccy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ybcxt.top/gtwwthmwvj.html

[T43] Perl：字符串插值
来源：http://hz.havefunace.top/gtahdoumfu.html

"值: $a"
来源：http://hz.shanyushiyangkeji.top/gtxvennrbt.html

[T44] Perl：条件
来源：http://hz.kuanghao11.cn/gtjsckiizs.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gtsdssedxp.html

[T45] Perl：数组遍历
来源：http://hz.zhengqikj.top/gtcrsyaxam.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtoqyfjtwe.html

[T46] Perl：哈希操作
来源：http://hz.svipenyu.cn/gtjgxcsocu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.nanxinkj.top/gtpxetibpx.html

[T47] Perl：正则捕获
来源：http://hz.jinqigufen.top/gtyglztwog.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gzhubu.top/gtynzljonb.html

[T48] Perl：正则替换
来源：http://hz.haohaochexian.top/gtkfkwhqxm.html

$s =~ s/old/new/g;
来源：http://hz.hongshengwenyu.top/gtnhkuudwu.html

[T49] Perl：函数
来源：http://hz.yj20258888.top/gtbchcmykr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sufxvd.cn/gtwcvknzeo.html

[T50] Perl：逐行读文件
来源：http://hz.xinyue.icu/gtdprktlxe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xuetiantiany.cn/gtcogjadmi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ivvv.top/gtrmvhpdek.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gtukfdglbt.html

println("Hello")
来源：http://hz.daria6918.cn/gtgitomvuk.html

[T52] Scala：变量
来源：http://hz.wangshuangyany.cn/gtfulauwvu.html

val a = 1;  var b = 2
来源：http://hz.havefunace.top/gtznjvvtsj.html

[T53] Scala：字符串插值
来源：http://hz.9152youxi.cn/gthaycgowz.html

s"值: $b"
来源：http://hz.cdnleiting.top/gtqwmnpdyd.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtxcvrjftg.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhijiandao.cn/gtxnsnbmgf.html

[T55] Scala：集合过滤
来源：http://hz.cdnleiting.top/gtlqejxkkp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.cheryme.top/gtlpxjurkk.html

[T56] Scala：样例类
来源：http://hz.yuanzhike.top/gtpxiedrju.html

case class User(name: String, age: Int)
来源：http://hz.jlsjyb.cn/gthbyeafbv.html

[T57] Scala：模式匹配
来源：http://hz.guowangkeji.top/gthtwpcfyl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.guannengcc.top/gtxgtoymlk.html

[T58] Scala：函数定义
来源：http://hz.pengpengdd.cyou/gtabhrjlnx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.vqdsnc.cn/gtsiccibuk.html

[T59] Scala：循环
来源：http://hz.smart0.xyz/gtscwdjaor.html

for (i <- 1 to 10) println(i)
来源：http://hz.jlsjyb.cn/gtqtrhflji.html

[T60] Scala：折叠
来源：http://hz.9152youxi.cn/gtxvracapu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jinyuanbaomall.cn/gtxmunmpgk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrorxsxcd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gttwnkdieh.html

================================================================================
来源：http://hz.haohaochexian.top/gtifbpmlqf.html

[U01] Py：创建虚拟环境
来源：http://hz.ydzc1.top/gthaqzuent.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jqgfzy.top/gtqcoeeccw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhongyouzk.top/gtgmsnxzbw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gogol.net.cn/gtulewqgin.html

[U03] Py：加载 .env 配置
来源：http://hz.jiagoushi.top/gtzjzhtsmb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yvedp.cn/gttseerado.html

[U04] Py：变量调试打印
来源：http://hz.ppjwa.cn/gtjjrqhnjc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yonumen.top/gthivizxvj.html

[U05] Py：列表去重且保序
来源：http://hz.yueranfly.top/gtlxqsfgxl.html

list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtbwnxdmxw.html

[U06] Py：合并两个字典
来源：http://hz.jianghu66.top/gtqgipqjlo.html

{**a, **b}
来源：http://hz.jianghu66.top/gtfrzyofdz.html

[U07] Py：反转字典键值
来源：http://hz.shanyushiyangtech.top/gteiixqbcd.html

{v: k for k, v in d.items()}
来源：http://hz.bjfxy.top/gtjmlphjsj.html

[U08] Py：展平二维列表
来源：http://hz.svipenyu.cn/gtrxaagtkk.html

[y for x in nested for y in x]
来源：http://hz.kuanghao11.cn/gtsksrbdtd.html

[U09] Py：字典取最大值的键
来源：http://hz.hnxiangtu.top/gtngyipjjs.html

max(d, key=d.get)
来源：http://hz.jinghuilouyu.cn/gtvgkeyeds.html

[U10] Py：按值排序字典
来源：http://hz.xuanzx.com/gtfqjpfbaa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.pengpengdd.cyou/gtmcvzbjgk.html

[U11] Py：生成器表达式
来源：http://hz.sxryk.cn/gtjnjwzxtl.html

(x * 2 for x in arr)
来源：http://hz.feifeiyinyue.top/gtzafapien.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hysaishi.cn/gtjxtpervu.html

Counter(arr).most_common(3)
来源：http://hz.haohaochexian.top/gtfntbkaml.html

[U13] Py：固定长度队列
来源：http://hz.cqqwz.cn/gtncncaefc.html

deque(maxlen=10)
来源：http://hz.daxiang520.top/gtvbcnzlsd.html

[U14] Py：分组收集到列表
来源：http://hz.chenlongwang.top/gtsncndjza.html

defaultdict(list)
来源：http://hz.gzhubu.top/gtvdvwlzkz.html

[U15] Py：高精度计时
来源：http://hz.chenzaomai.com/gtvsbgwzoe.html

t = time.perf_counter()
来源：http://hz.dianchejie.cn/gtbujfdcmp.html

[U16] Py：命令行参数解析
来源：http://hz.c1oappe.top/gtrlufmwpj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hysaishi.cn/gtctvmqrqa.html

[U17] Py：初始化日志
来源：http://hz.chenlongwang.top/gtomrawqsf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtaevddder.html

[U18] Py：预编译正则
来源：http://hz.zhongyouzk.top/gtlzkdcsic.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gtcrldgsaz.html

[U19] Py：正则替换带回调
来源：http://hz.jinghuilouyu.cn/gtietdgwtg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.pycfn.com/gtccqqsuxv.html

[U20] Py：缓存函数结果
来源：http://hz.daxiang520.top/gttmbnsoll.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhixingplan.top/gtynrrgmkh.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinyuanbaomall.cn/gtjzjfohft.html

@contextlib.contextmanager
来源：http://hz.yueranfly.top/gtegbdfxab.html

[U22] Py：矩阵转置
来源：http://hz.gotoacloud.top/gtnfpdfnrp.html

list(zip(*m))
来源：http://hz.birdmap.top/gtbafsosol.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtnmmijnqm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.c1oappe.top/gtbthgwpre.html

[U24] Py：路径操作
来源：http://hz.bjfxy.top/gtmgfhkgsw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtnnfgtgpp.html

[U25] Py：CSV 按字典读
来源：http://hz.yonumen.top/gtwhfkzmcd.html

csv.DictReader(f)
来源：http://hz.xinyue.icu/gtejphimmz.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtlffgnwwn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jyoumei.cn/gtntoevotz.html

[U27] Py：异步 HTTP
来源：http://hz.aibaodan.cn/gtlbmlhvmp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dashuyun.cn/gtoibahqka.html

[U28] Py：类型别名
来源：http://hz.wangshuangyany.cn/gttyvefpbe.html

UserId = int
来源：http://hz.jiagoushi.top/gtfdokdcry.html

[U29] Py：属性校验
来源：http://hz.pengpengdd.cyou/gtfdwygaxk.html

@property 与 @x.setter 配合
来源：http://hz.shuidangran.top/gtthstzemh.html

[U30] Py：数据类
来源：http://hz.c1oappe.top/gtmgprxqev.html

@dataclass(slots=True)
来源：http://hz.zhongyouzk.top/gthuyfjmam.html

[U31] Py：单测
来源：http://hz.dashuyun.cn/gtiprcsbkf.html

python -m pytest -q
来源：http://hz.xziqi.cn/gtibqhgcoo.html

[U32] Py：代码格式化
来源：http://hz.aibaodan.cn/gtdzsduxyp.html

ruff format . && ruff check --fix .
来源：http://hz.andypj.xyz/gtngpvajpk.html

[U33] Py：打包发布
来源：http://hz.aibaodan.cn/gtuapzqtxa.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangshuangyany.cn/gtjgoqnqgt.html

[U34] Py：判断编码
来源：http://hz.hongshengwenyu.top/gtkhxtxkcc.html

chardet.detect(raw)
来源：http://hz.tian-w.cn/gtbawxhtqk.html

[U35] Py：发送邮件
来源：http://hz.xuetiantiany.cn/gtqxnjfwvq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.daxiang520.top/gtrvfwjpnf.html

[U36] Py：定时任务
来源：http://hz.yuxming.cn/gtchjgrlzp.html

schedule.every(10).minutes.do(job)
来源：http://hz.hfpthk.cn/gtphknrqry.html

[U37] Py：读写 Excel
来源：http://hz.chenjidiqi.icu/gtmcowsvzp.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.smart0.xyz/gtxsbusdfv.html

[U38] Py：获取脚本所在目录
来源：http://hz.yongpay.top/gtbhcvldsx.html

Path(__file__).resolve().parent
来源：http://hz.hnxiangtu.top/gtduppfvpc.html

[U39] Py：判断是否在交互环境
来源：http://hz.sxryk.cn/gthjcdoepe.html

sys.stdout.isatty()
来源：http://hz.sxryk.cn/gtthdhqlme.html

[U40] Py：打印到标准错误
来源：http://hz.xuanzx.com/gtkmaxaeec.html

print("err", file=sys.stderr)
来源：http://hz.jinghuilouyu.cn/gtmmpshcwq.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shangyingyoupin.top/gtfvwdbpew.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.wangshuangyany.cn/gtmqqsafpi.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yj20258.top/gtweghdxey.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yongpay.top/gtulmmbemd.html

[U43] PHP：声明命名空间
来源：http://hz.zhixingplan.top/gtgqxybell.html

namespace App\Http;
来源：http://hz.9152youxi.cn/gtkiqppiyl.html

[U44] PHP：开启严格类型
来源：http://hz.ybcxt.top/gtumcoyeqp.html

declare(strict_types=1);
来源：http://hz.shzxlz.cn/gtqoqgppcn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yj20258888.top/gtcumrpbfn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gthqeyujct.html

[U46] PHP：可空类型
来源：http://hz.yanxiufei.cn/gtzewkvtps.html

?string $name = null
来源：http://hz.316326.xyz/gtngrepsvn.html

[U47] PHP：联合类型
来源：http://hz.gaohongyu789.top/gtfwizzqcr.html

int|string $id
来源：http://hz.zycfv.cn/gtplgchnym.html

[U48] PHP：纯枚举
来源：http://hz.xingfuxueyuan.xyz/gtvexdfojs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jinqigufen.top/gtrebrjzas.html

[U49] PHP：只读属性
来源：http://hz.wangshuangyany.cn/gtrbkmgxnx.html

public readonly string $name
来源：http://hz.kuanghao11.cn/gttzsenlbt.html

[U50] PHP：构造器属性提升
来源：http://hz.hywenlv.cn/gtzexobfrl.html

public function __construct(private int $id) {}
来源：http://hz.shuidangran.top/gtedoifbnp.html

[U51] PHP：数组解构
来源：http://hz.cheryme.top/gtstmuosmq.html

[$a, $b] = $arr;
来源：http://hz.dianchejie.cn/gtruwzkcwn.html

[U52] PHP：箭头函数
来源：http://hz.andypj.xyz/gtxrrfvmxu.html

$double = fn($x) => $x * 2;
来源：http://hz.redwolf501.top/gtkwbqlacl.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtkpovpmfn.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangdashe.top/gtrkjrgeen.html

[U54] PHP：空安全调用
来源：http://hz.zdqjudy.top/gtkocohtsb.html

$obj?->method()
来源：http://hz.kuanghao11.cn/gtzmakcgey.html

[U55] PHP：match 表达式
来源：http://hz.jinyuanbaomall.cn/gtaduifaiy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cqqwz.cn/gtqigpzsub.html

[U56] PHP：命名参数
来源：http://hz.0kj1m.cn/gtszljqtsq.html

f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtsyowxreq.html

[U57] PHP：字符串插值
来源：http://hz.fzhhl.top/gtozckrnfu.html

"值: {$a}"
来源：http://hz.ehwqpu.com/gtoqbazkit.html

[U58] PHP：数组三件套
来源：http://hz.sweek.top/gtlbrcfukt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.0kj1m.cn/gthjzrsshd.html

[U59] PHP：自定义排序
来源：http://hz.xinyue.icu/gtxxjtutzk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtzbkddfoj.html

[U60] PHP：JSON 编解码
来源：http://hz.redwolf501.top/gtrdvfaggm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.cheryme.top/gttlwknotm.html

[U61] PHP：正则
来源：http://hz.yj20258.top/gthutvjcif.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtfxkcppzh.html

[U62] PHP：日期对象
来源：http://hz.zhaomingkeji.xyz/gtmkwkhaxi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.zhixingplan.top/gtxrusfcip.html

[U63] PHP：文件读写
来源：http://hz.tian-w.cn/gtqgtxsxbn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shzxlz.cn/gtlrzbdpvb.html

[U64] PHP：目录遍历
来源：http://hz.cucudq.cn/gtdgwpqmsq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.chenzaomai.com/gtmtrwjphn.html

[U65] PHP：会话
来源：http://hz.birdmap.top/gtckkybgpy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.chenjidiqi.icu/gtxcolmhbt.html

[U66] PHP：设置 Cookie
来源：http://hz.jianghu66.top/gtckadutqe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yonumen.top/gtwatexyru.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gteibbqcij.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cucudq.cn/gtihkbpjtk.html

[U68] PHP：PDO 连接
来源：http://hz.jlsjyb.cn/gtqztmrmto.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.wangshuangyany.cn/gtxhfhtfbc.html

[U69] PHP：PDO 预处理
来源：http://hz.yonumen.top/gthqasuhhz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.xziqi.cn/gtuagdvtzm.html

[U70] PHP：PDO 事务
来源：http://hz.nanxinkj.top/gtnusrnucb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhijiandao.cn/gtvjumhdtw.html

[U71] PHP：抛出异常
来源：http://hz.gogol.net.cn/gtjkxoedwd.html

throw new RuntimeException("失败", 500);
来源：http://hz.9152youxi.cn/gthpbxpaku.html

[U72] PHP：写错误日志
来源：http://hz.zhijiandao.cn/gtinzlhtxe.html

error_log("失败: " . $e->getMessage());
来源：http://hz.aibaodan.cn/gtpammobzq.html

[U73] PHP：读取 ini 配置
来源：http://hz.ydjk.org.cn/gtnnvsbkpm.html

parse_ini_file("config.ini", true)
来源：http://hz.yj20258.top/gtbzkmvwco.html

[U74] PHP：读取环境变量
来源：http://hz.shzxlz.cn/gtiguwdqbz.html

getenv("APP_ENV") ?: "production"
来源：http://hz.sufxvd.cn/gtlewzymia.html

[U75] PHP：依赖注入
来源：http://hz.yj20258.top/gtjxixthqc.html

composer require psr/container
来源：http://hz.jinghuilouyu.cn/gtswyfiiyi.html

[U76] PHP：简单路由
来源：http://hz.sxryk.cn/gtlpqyjijr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.jianghu66.top/gtwyypwbje.html


<!-- 参考信息 -->