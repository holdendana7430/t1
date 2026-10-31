代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://qm.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mm.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://ir.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sb.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://uh.haigaiapp.cn

[S49] C++：写文件
来源：http://ls.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sz.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://mx.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://px.shxzukj.cn

[S51] C++：显式类型转换
来源：http://jg.bjjhwx.cn

static_cast<double>(a) / b
来源：http://yn.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://bv.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://zl.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://kk.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://jd.muxihuayi.cn

[S54] C++：异常处理
来源：http://mf.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dv.shxzskj.cn

[S55] C++：结构化绑定
来源：http://cs.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ed.newstarts.cn

[S56] C++：optional
来源：http://sj.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rf.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ol.yuntaijiaju.cn

constexpr int N = 10;
来源：http://zj.wgjwhj.cn

[S58] C++：命名空间
来源：http://ty.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://vq.asd995.cn

[S59] C++：静态断言
来源：http://td.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tb.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://fk.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ws.haigaiapp.cn

================================================================================
来源：http://uk.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://us.huixinmuqiang.cn

================================================================================
来源：http://hx.bjjhwx.cn

[T01] Kotlin：Hello World
来源：http://kl.hahajie.cn

println("Hello")
来源：http://uo.nicolike.cn

[T02] Kotlin：变量
来源：http://yr.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iv.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://js.bjjhwx.cn

"值: $b"
来源：http://fq.gzmigu.cn

[T04] Kotlin：空安全
来源：http://od.huanxung.cn

val n: String? = null;  n?.length
来源：http://lf.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ec.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cj.hahajie.cn

[T06] Kotlin：集合映射
来源：http://qa.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ft.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://ok.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rt.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://ap.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://dz.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ox.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://ct.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://ze.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wq.panjiajie.cn

[T11] Kotlin：协程
来源：http://lw.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gm.newstarts.cn

[T12] Kotlin：解构声明
来源：http://cu.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://jt.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://cm.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://io.panjiajie.cn

[T14] Kotlin：循环
来源：http://qz.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://ql.gzmigu.cn

[T15] Kotlin：接口
来源：http://ca.9csxet.cn

interface Shape { fun area(): Double }
来源：http://ed.szsharing.cn

[T16] Swift：Hello World
来源：http://rt.shxzukj.cn

print("Hello")
来源：http://dv.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ji.newstarts.cn

var a = 1;  let b = 2
来源：http://ac.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://dh.shxzskj.cn

"值: \(b)"
来源：http://zb.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://bs.jctech888.com.cn

if let n = opt { print(n) }
来源：http://ri.newstarts.cn

[T20] Swift：数组操作
来源：http://tn.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pa.shtwfgs.cn

[T21] Swift：遍历
来源：http://lv.shxzukj.cn

for x in a { print(x) }
来源：http://iv.hnjuh.cn

[T22] Swift：字典
来源：http://ko.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oc.szsharing.cn

[T23] Swift：函数
来源：http://dw.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rp.gzmigu.cn

[T24] Swift：闭包
来源：http://uq.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ll.shtwfgs.cn

[T25] Swift：结构体
来源：http://lx.haigaiapp.cn

struct P { var x: Int }
来源：http://rx.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://gz.asd995.cn

class A: Base { override func f() {} }
来源：http://wx.lnxyls.cn

[T27] Swift：错误处理
来源：http://ih.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://sg.nszjky.cn

[T28] Swift：枚举
来源：http://xg.jctech888.com.cn

enum Color { case red, green }
来源：http://wk.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://ak.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://bt.szsharing.cn

[T30] Swift：协议
来源：http://ph.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://dj.lnxyls.cn

[T31] Lua：Hello World
来源：http://no.shxzskj.cn

print("Hello")
来源：http://me.hahajie.cn

[T32] Lua：局部变量
来源：http://ch.muxihuayi.cn

local a = 1
来源：http://fr.nicolike.cn

[T33] Lua：表（数组）
来源：http://qk.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gd.szxytkj.cn

[T34] Lua：遍历表
来源：http://fc.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sv.szxytkj.cn

[T35] Lua：字典表
来源：http://hg.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://pd.nicolike.cn

[T36] Lua：函数
来源：http://zu.521024.cn

function add(a, b) return a + b end
来源：http://qp.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://ob.hnjuh.cn

"a" .. "b"
来源：http://nn.gzmigu.cn

[T38] Lua：条件
来源：http://mi.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://od.panjiajie.cn

[T39] Lua：模式匹配
来源：http://cw.muxihuayi.cn

string.find(s, "%d+")
来源：http://qh.hahajie.cn

[T40] Lua：元表
来源：http://qx.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://kp.9csxet.cn

[T41] Perl：Hello World
来源：http://qt.bookmarksfly.cn

print "Hello\n";
来源：http://hv.yuexingan06.cn

[T42] Perl：变量类型
来源：http://gv.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jw.nicolike.cn

[T43] Perl：字符串插值
来源：http://en.jianghongdianzi.cn

"值: $a"
来源：http://nz.szsharing.cn

[T44] Perl：条件
来源：http://vc.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://jp.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://vd.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://zt.nszjky.cn

[T46] Perl：哈希操作
来源：http://rv.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yc.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://go.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gx.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://vj.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://yk.9csxet.cn

[T49] Perl：函数
来源：http://mj.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vv.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://eh.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ss.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://vh.muxihuayi.cn

[T51] Scala：Hello World
来源：http://fu.nszjky.cn

println("Hello")
来源：http://zs.muxihuayi.cn

[T52] Scala：变量
来源：http://hl.newstarts.cn

val a = 1;  var b = 2
来源：http://qa.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://js.newstarts.cn

s"值: $b"
来源：http://dx.521024.cn

[T54] Scala：集合映射
来源：http://bp.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://zc.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ge.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jo.nszjky.cn

[T56] Scala：样例类
来源：http://xc.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://ro.lnxyls.cn

[T57] Scala：模式匹配
来源：http://jv.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://he.jctech888.com.cn

[T58] Scala：函数定义
来源：http://wk.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://os.yuexingan06.cn

[T59] Scala：循环
来源：http://sz.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://tj.muxihuayi.cn

[T60] Scala：折叠
来源：http://ae.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zi.lnxyls.cn

================================================================================
来源：http://sy.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sj.wgjwhj.cn

================================================================================
来源：http://qj.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://dz.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ye.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://rf.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yc.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://je.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ym.newstarts.cn

[U04] Py：变量调试打印
来源：http://gm.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pi.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://pg.nszjky.cn

list(dict.fromkeys(arr))
来源：http://cq.huanxung.cn

[U06] Py：合并两个字典
来源：http://gu.hnjuh.cn

{**a, **b}
来源：http://hn.nicolike.cn

[U07] Py：反转字典键值
来源：http://ve.szsharing.cn

{v: k for k, v in d.items()}
来源：http://yo.shxzskj.cn

[U08] Py：展平二维列表
来源：http://rl.shxzskj.cn

[y for x in nested for y in x]
来源：http://xu.521024.cn

[U09] Py：字典取最大值的键
来源：http://ft.shxzukj.cn

max(d, key=d.get)
来源：http://dx.shxzukj.cn

[U10] Py：按值排序字典
来源：http://gt.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gs.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://ra.newstarts.cn

(x * 2 for x in arr)
来源：http://wp.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oi.szsharing.cn

Counter(arr).most_common(3)
来源：http://cn.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ma.huixiangedu.cn

deque(maxlen=10)
来源：http://mu.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://af.colortex.cn

defaultdict(list)
来源：http://tz.colortex.cn

[U15] Py：高精度计时
来源：http://yl.nszjky.cn

t = time.perf_counter()
来源：http://qz.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://ha.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ze.9csxet.cn

[U17] Py：初始化日志
来源：http://gj.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ue.huanxung.cn

[U18] Py：预编译正则
来源：http://er.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://vr.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://cv.bjjhwx.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jh.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://em.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://ax.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://iv.hahajie.cn

@contextlib.contextmanager
来源：http://fp.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://qz.yuntaijiaju.cn

list(zip(*m))
来源：http://ot.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://en.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rg.szxytkj.cn

[U24] Py：路径操作
来源：http://rj.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bg.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://sr.colortex.cn

csv.DictReader(f)
来源：http://lh.huanxung.cn

[U26] Py：并发下载
来源：http://gh.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lx.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://vg.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://no.yuexingan06.cn

[U28] Py：类型别名
来源：http://oq.shtwfgs.cn

UserId = int
来源：http://ni.huanxung.cn

[U29] Py：属性校验
来源：http://en.shxzukj.cn

@property 与 @x.setter 配合
来源：http://xx.huanxung.cn

[U30] Py：数据类
来源：http://yf.yuexingan06.cn

@dataclass(slots=True)
来源：http://li.yuexingan06.cn

[U31] Py：单测
来源：http://kz.szxytkj.cn

python -m pytest -q
来源：http://xw.jctech888.com.cn

[U32] Py：代码格式化
来源：http://db.521024.cn

ruff format . && ruff check --fix .
来源：http://lt.shtwfgs.cn

[U33] Py：打包发布
来源：http://ta.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://oj.shxzukj.cn

[U34] Py：判断编码
来源：http://nx.newstarts.cn

chardet.detect(raw)
来源：http://ee.haigaiapp.cn

[U35] Py：发送邮件
来源：http://gi.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lv.haigaiapp.cn

[U36] Py：定时任务
来源：http://pt.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://jn.newstarts.cn

[U37] Py：读写 Excel
来源：http://rk.haigaiapp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hv.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://vx.shxzskj.cn

Path(__file__).resolve().parent
来源：http://ii.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://mb.newstarts.cn

sys.stdout.isatty()
来源：http://eh.colortex.cn

[U40] Py：打印到标准错误
来源：http://gi.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://cj.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://xw.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mv.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://qx.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://km.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://wd.shxzskj.cn

namespace App\Http;
来源：http://st.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://yo.9csxet.cn

declare(strict_types=1);
来源：http://js.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://ps.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://mo.yuexingan06.cn

[U46] PHP：可空类型
来源：http://qq.lnxyls.cn

?string $name = null
来源：http://fg.hahajie.cn

[U47] PHP：联合类型
来源：http://hm.newstarts.cn

int|string $id
来源：http://ff.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://of.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qr.bookmarksfly.cn

[U49] PHP：只读属性
来源：http://xs.colortex.cn

public readonly string $name
来源：http://bv.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://pb.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://vf.huixiangedu.cn

[U51] PHP：数组解构
来源：http://rp.gzmigu.cn

[$a, $b] = $arr;
来源：http://hs.colortex.cn

[U52] PHP：箭头函数
来源：http://hj.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://xy.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://pm.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://mi.asd995.cn

[U54] PHP：空安全调用
来源：http://hr.panjiajie.cn

$obj?->method()
来源：http://eq.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://xt.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uq.asd995.cn

[U56] PHP：命名参数
来源：http://pp.chemitech.net.cn

f(a: 1, b: 2)
来源：http://rc.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://bq.newstarts.cn

"值: {$a}"
来源：http://kb.nicolike.cn

[U58] PHP：数组三件套
来源：http://mh.wgjwhj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fx.szsharing.cn

[U59] PHP：自定义排序
来源：http://rs.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vp.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://ec.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xj.szxytkj.cn

[U61] PHP：正则
来源：http://xi.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mt.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://cq.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ne.haigaiapp.cn

[U63] PHP：文件读写
来源：http://zz.shxzskj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gq.asd995.cn

[U64] PHP：目录遍历
来源：http://tr.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://ag.nszjky.cn

[U65] PHP：会话
来源：http://ox.huanxung.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ol.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://ze.9csxet.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mj.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://nz.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ue.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://hr.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fq.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://re.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iw.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://kt.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tt.panjiajie.cn

[U71] PHP：抛出异常
来源：http://oe.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://td.9csxet.cn

[U72] PHP：写错误日志
来源：http://fg.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://pd.szsharing.cn


<!-- 参考信息 -->