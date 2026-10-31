代发 wailian999

[S43] C++：智能指针
来源：http://xy.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://kt.shxzskj.cn

[S44] C++：引用传参
来源：http://ru.colortex.cn

void inc(int &x) { ++x; }
来源：http://bs.521024.cn

[S45] C++：lambda
来源：http://zl.nszjky.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ic.szsharing.cn

[S46] C++：函数模板
来源：http://qk.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://op.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://kf.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ys.521024.cn

[S48] C++：逐行读文件
来源：http://yg.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kr.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://en.hnjuh.cn

[S49] C++：写文件
来源：http://wy.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mk.huixiangedu.cn

[S50] C++：格式化数字
来源：http://qf.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uf.shxzskj.cn

[S51] C++：显式类型转换
来源：http://pm.yuexingan06.cn

static_cast<double>(a) / b
来源：http://nx.521024.cn

[S52] C++：const 与 noexcept
来源：http://qu.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://qb.panjiajie.cn

[S53] C++：移动语义
来源：http://lr.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://op.shtwfgs.cn

[S54] C++：异常处理
来源：http://cl.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fv.hahajie.cn

[S55] C++：结构化绑定
来源：http://ld.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://if.muxihuayi.cn

[S56] C++：optional
来源：http://fe.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rw.haigaiapp.cn

[S57] C++：编译期常量
来源：http://rn.hnjuh.cn

constexpr int N = 10;
来源：http://bg.521024.cn

[S58] C++：命名空间
来源：http://bc.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://un.asd995.cn

[S59] C++：静态断言
来源：http://gc.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ku.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://yb.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ru.nszjky.cn

================================================================================
来源：http://bh.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nw.yuexingan06.cn

================================================================================
来源：http://aj.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://hq.bjjhwx.cn

println("Hello")
来源：http://ll.lnxyls.cn

[T02] Kotlin：变量
来源：http://sn.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jy.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://uu.haigaiapp.cn

"值: $b"
来源：http://la.lnxyls.cn

[T04] Kotlin：空安全
来源：http://nm.panjiajie.cn

val n: String? = null;  n?.length
来源：http://zv.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://lp.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ny.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://ih.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ms.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ry.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kj.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://xp.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://pz.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://ko.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://wj.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://re.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hf.nszjky.cn

[T11] Kotlin：协程
来源：http://eq.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gh.newstarts.cn

[T12] Kotlin：解构声明
来源：http://my.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://je.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://ug.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://bv.yuexingan06.cn

[T14] Kotlin：循环
来源：http://oh.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://vo.shxzskj.cn

[T15] Kotlin：接口
来源：http://aa.521024.cn

interface Shape { fun area(): Double }
来源：http://cs.shtwfgs.cn

[T16] Swift：Hello World
来源：http://wg.bjjhwx.cn

print("Hello")
来源：http://gh.gzmigu.cn

[T17] Swift：变量与常量
来源：http://cl.szxytkj.cn

var a = 1;  let b = 2
来源：http://wi.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://qs.huixiangedu.cn

"值: \(b)"
来源：http://om.hnjuh.cn

[T19] Swift：可选绑定
来源：http://zs.haigaiapp.cn

if let n = opt { print(n) }
来源：http://xk.huanxung.cn

[T20] Swift：数组操作
来源：http://tg.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dj.jctech888.com.cn

[T21] Swift：遍历
来源：http://wk.asd995.cn

for x in a { print(x) }
来源：http://sm.huixinmuqiang.cn

[T22] Swift：字典
来源：http://sm.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ew.nicolike.cn

[T23] Swift：函数
来源：http://ot.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zf.shxzukj.cn

[T24] Swift：闭包
来源：http://gp.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pd.nicolike.cn

[T25] Swift：结构体
来源：http://ht.gzmigu.cn

struct P { var x: Int }
来源：http://hj.bjjhwx.cn

[T26] Swift：类与重写
来源：http://kq.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://wn.521024.cn

[T27] Swift：错误处理
来源：http://gm.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://qj.shtwfgs.cn

[T28] Swift：枚举
来源：http://yu.szxytkj.cn

enum Color { case red, green }
来源：http://zd.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://hs.shxzskj.cn

guard let x = opt else { return }
来源：http://zy.nicolike.cn

[T30] Swift：协议
来源：http://vo.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://gb.haigaiapp.cn

[T31] Lua：Hello World
来源：http://ml.521024.cn

print("Hello")
来源：http://sg.szxytkj.cn

[T32] Lua：局部变量
来源：http://tr.huanxung.cn

local a = 1
来源：http://ec.shxzskj.cn

[T33] Lua：表（数组）
来源：http://jn.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gx.huixiangedu.cn

[T34] Lua：遍历表
来源：http://uu.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gr.chemitech.net.cn

[T35] Lua：字典表
来源：http://rq.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://xp.lnxyls.cn

[T36] Lua：函数
来源：http://ju.huixiangedu.cn

function add(a, b) return a + b end
来源：http://eg.newstarts.cn

[T37] Lua：字符串拼接
来源：http://cf.huixinmuqiang.cn

"a" .. "b"
来源：http://nw.gzmigu.cn

[T38] Lua：条件
来源：http://ax.haigaiapp.cn

if x > 0 then print("正") end
来源：http://ty.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://wb.huixiangedu.cn

string.find(s, "%d+")
来源：http://tc.wgjwhj.cn

[T40] Lua：元表
来源：http://vo.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://at.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://dt.gzmigu.cn

print "Hello\n";
来源：http://qb.shxzskj.cn

[T42] Perl：变量类型
来源：http://vv.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oc.lnxyls.cn

[T43] Perl：字符串插值
来源：http://zh.newstarts.cn

"值: $a"
来源：http://gk.panjiajie.cn

[T44] Perl：条件
来源：http://tl.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://lu.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://gc.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://bj.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://fu.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uo.panjiajie.cn

[T47] Perl：正则捕获
来源：http://sb.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qe.shxzukj.cn

[T48] Perl：正则替换
来源：http://tf.gzmigu.cn

$s =~ s/old/new/g;
来源：http://uo.shtwfgs.cn

[T49] Perl：函数
来源：http://gm.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vy.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://xm.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hn.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://aj.muxihuayi.cn

[T51] Scala：Hello World
来源：http://wq.chemitech.net.cn

println("Hello")
来源：http://cy.jctech888.com.cn

[T52] Scala：变量
来源：http://mc.hahajie.cn

val a = 1;  var b = 2
来源：http://fx.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://yx.shxzskj.cn

s"值: $b"
来源：http://st.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://em.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://ay.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://fw.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://at.bjjhwx.cn

[T56] Scala：样例类
来源：http://ck.9csxet.cn

case class User(name: String, age: Int)
来源：http://pb.lnxyls.cn

[T57] Scala：模式匹配
来源：http://oa.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vw.hahajie.cn

[T58] Scala：函数定义
来源：http://rg.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://el.nszjky.cn

[T59] Scala：循环
来源：http://kb.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://wd.muxihuayi.cn

[T60] Scala：折叠
来源：http://ui.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hd.huixiangedu.cn

================================================================================
来源：http://uh.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jc.muxihuayi.cn

================================================================================
来源：http://ev.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://dx.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://go.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://wc.hahajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dr.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://ur.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uq.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://sb.yuntaijiaju.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xw.newstarts.cn

[U05] Py：列表去重且保序
来源：http://aq.521024.cn

list(dict.fromkeys(arr))
来源：http://wl.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://wi.shxzukj.cn

{**a, **b}
来源：http://ai.huanxung.cn

[U07] Py：反转字典键值
来源：http://fn.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://gy.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://mu.hahajie.cn

[y for x in nested for y in x]
来源：http://ag.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://fn.huixiangedu.cn

max(d, key=d.get)
来源：http://jc.shxzukj.cn

[U10] Py：按值排序字典
来源：http://jc.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lc.gzmigu.cn

[U11] Py：生成器表达式
来源：http://nk.nszjky.cn

(x * 2 for x in arr)
来源：http://cw.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oz.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://eh.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://hm.lnxyls.cn

deque(maxlen=10)
来源：http://rx.nszjky.cn

[U14] Py：分组收集到列表
来源：http://eb.haigaiapp.cn

defaultdict(list)
来源：http://jl.9csxet.cn

[U15] Py：高精度计时
来源：http://en.yuexingan06.cn

t = time.perf_counter()
来源：http://rj.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://ra.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ne.huixiangedu.cn

[U17] Py：初始化日志
来源：http://ut.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://jw.521024.cn

[U18] Py：预编译正则
来源：http://gd.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://md.521024.cn

[U19] Py：正则替换带回调
来源：http://oj.asd995.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ms.chemitech.net.cn

[U20] Py：缓存函数结果
来源：http://ew.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://mq.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://eb.muxihuayi.cn

@contextlib.contextmanager
来源：http://tj.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://ia.hnjuh.cn

list(zip(*m))
来源：http://qe.shxzukj.cn

[U23] Py：分块读取大文件
来源：http://ce.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tg.chemitech.net.cn

[U24] Py：路径操作
来源：http://cs.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ge.521024.cn

[U25] Py：CSV 按字典读
来源：http://jg.yuexingan06.cn

csv.DictReader(f)
来源：http://mn.muxihuayi.cn

[U26] Py：并发下载
来源：http://ik.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tm.hahajie.cn

[U27] Py：异步 HTTP
来源：http://tn.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://tt.yuexingan06.cn

[U28] Py：类型别名
来源：http://up.hnjuh.cn

UserId = int
来源：http://uk.shxzukj.cn

[U29] Py：属性校验
来源：http://er.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://fi.colortex.cn

[U30] Py：数据类
来源：http://ul.chemitech.net.cn

@dataclass(slots=True)
来源：http://il.shxzukj.cn

[U31] Py：单测
来源：http://nr.huixinmuqiang.cn

python -m pytest -q
来源：http://ni.haigaiapp.cn

[U32] Py：代码格式化
来源：http://ni.newstarts.cn

ruff format . && ruff check --fix .
来源：http://sf.wgjwhj.cn

[U33] Py：打包发布
来源：http://bz.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://mb.bjjhwx.cn

[U34] Py：判断编码
来源：http://uu.shxzukj.cn

chardet.detect(raw)
来源：http://ew.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://cj.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yd.gzmigu.cn

[U36] Py：定时任务
来源：http://ts.521024.cn

schedule.every(10).minutes.do(job)
来源：http://lj.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://iv.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pe.521024.cn

[U38] Py：获取脚本所在目录
来源：http://cl.9csxet.cn

Path(__file__).resolve().parent
来源：http://ai.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://xc.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://ly.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ta.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://wi.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://zm.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://be.wgjwhj.cn

[U42] PHP：PSR-4 自动加载
来源：http://ue.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yo.colortex.cn

[U43] PHP：声明命名空间
来源：http://lq.chemitech.net.cn

namespace App\Http;
来源：http://md.huanxung.cn

[U44] PHP：开启严格类型
来源：http://ne.nicolike.cn

declare(strict_types=1);
来源：http://er.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://jf.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://na.hnjuh.cn

[U46] PHP：可空类型
来源：http://uw.szxytkj.cn

?string $name = null
来源：http://ln.9csxet.cn

[U47] PHP：联合类型
来源：http://ka.lnxyls.cn

int|string $id
来源：http://hd.asd995.cn

[U48] PHP：纯枚举
来源：http://rq.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aj.9csxet.cn

[U49] PHP：只读属性
来源：http://sg.asd995.cn

public readonly string $name
来源：http://gk.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ue.haigaiapp.cn

public function __construct(private int $id) {}
来源：http://pw.huixiangedu.cn

[U51] PHP：数组解构
来源：http://gz.bjjhwx.cn

[$a, $b] = $arr;
来源：http://lk.panjiajie.cn

[U52] PHP：箭头函数
来源：http://tx.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://jx.521024.cn

[U53] PHP：空合并运算符
来源：http://jq.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://ho.szxytkj.cn

[U54] PHP：空安全调用
来源：http://zw.jianghongdianzi.cn

$obj?->method()
来源：http://us.newstarts.cn

[U55] PHP：match 表达式
来源：http://fi.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ue.shtwfgs.cn

[U56] PHP：命名参数
来源：http://gy.shtwfgs.cn

f(a: 1, b: 2)
来源：http://uq.nszjky.cn

[U57] PHP：字符串插值
来源：http://pz.colortex.cn

"值: {$a}"
来源：http://wp.521024.cn

[U58] PHP：数组三件套
来源：http://ns.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://le.bookmarksfly.cn

[U59] PHP：自定义排序
来源：http://rz.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://vt.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ge.9csxet.cn

[U61] PHP：正则
来源：http://vp.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dl.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://qh.asd995.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://la.haigaiapp.cn

[U63] PHP：文件读写
来源：http://fp.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fo.shxzskj.cn

[U64] PHP：目录遍历
来源：http://uw.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ut.bookmarksfly.cn

[U65] PHP：会话
来源：http://hc.bjjhwx.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oj.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://ga.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://th.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://zg.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uu.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://lb.szsharing.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wo.chemitech.net.cn


<!-- 参考信息 -->