代发 wailian999

while (std::getline(in, line)) { }
来源：http://du.shtwfgs.cn

[S49] C++：写文件
来源：http://zv.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ev.jctech888.com.cn

[S50] C++：格式化数字
来源：http://wm.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://re.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://xd.jctech888.com.cn

static_cast<double>(a) / b
来源：http://ip.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://gu.colortex.cn

int size() const noexcept { return n_; }
来源：http://qh.521024.cn

[S53] C++：移动语义
来源：http://pv.asd995.cn

std::vector<int> w = std::move(v);
来源：http://ms.bjjhwx.cn

[S54] C++：异常处理
来源：http://lv.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ba.huanxung.cn

[S55] C++：结构化绑定
来源：http://ou.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kq.huanxung.cn

[S56] C++：optional
来源：http://ea.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yx.hahajie.cn

[S57] C++：编译期常量
来源：http://ve.jctech888.com.cn

constexpr int N = 10;
来源：http://st.521024.cn

[S58] C++：命名空间
来源：http://fa.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://db.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://zi.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zs.colortex.cn

[S60] C++：遍历并删除元素
来源：http://ga.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tk.yuexingan06.cn

================================================================================
来源：http://az.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wu.lnxyls.cn

================================================================================
来源：http://zq.newstarts.cn

[T01] Kotlin：Hello World
来源：http://ok.nicolike.cn

println("Hello")
来源：http://gm.bjjhwx.cn

[T02] Kotlin：变量
来源：http://lx.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jy.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://hy.shtwfgs.cn

"值: $b"
来源：http://lb.huanxung.cn

[T04] Kotlin：空安全
来源：http://cx.colortex.cn

val n: String? = null;  n?.length
来源：http://kt.asd995.cn

[T05] Kotlin：when 表达式
来源：http://wp.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ke.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://jm.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qv.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://cr.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://om.hnjuh.cn

[T08] Kotlin：数据类
来源：http://nl.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://tl.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://nz.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://yg.asd995.cn

[T10] Kotlin：默认参数
来源：http://aj.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ol.shxzskj.cn

[T11] Kotlin：协程
来源：http://hk.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mf.9csxet.cn

[T12] Kotlin：解构声明
来源：http://wx.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://nk.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://lv.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ex.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://lb.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://ns.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://vo.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://mv.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://kt.yuntaijiaju.cn

print("Hello")
来源：http://he.shxzukj.cn

[T17] Swift：变量与常量
来源：http://en.nicolike.cn

var a = 1;  let b = 2
来源：http://go.panjiajie.cn

[T18] Swift：字符串插值
来源：http://bm.bjjhwx.cn

"值: \(b)"
来源：http://gf.haigaiapp.cn

[T19] Swift：可选绑定
来源：http://ak.wgjwhj.cn

if let n = opt { print(n) }
来源：http://cg.shxzukj.cn

[T20] Swift：数组操作
来源：http://la.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lw.yuexingan06.cn

[T21] Swift：遍历
来源：http://kf.jianghongdianzi.cn

for x in a { print(x) }
来源：http://jz.hahajie.cn

[T22] Swift：字典
来源：http://tv.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xf.wgjwhj.cn

[T23] Swift：函数
来源：http://uv.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yc.szxytkj.cn

[T24] Swift：闭包
来源：http://ga.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xu.hnjuh.cn

[T25] Swift：结构体
来源：http://ku.hnjuh.cn

struct P { var x: Int }
来源：http://bh.shxzukj.cn

[T26] Swift：类与重写
来源：http://ko.521024.cn

class A: Base { override func f() {} }
来源：http://gm.szxytkj.cn

[T27] Swift：错误处理
来源：http://vb.hahajie.cn

do { try f() } catch { print(error) }
来源：http://ho.szsharing.cn

[T28] Swift：枚举
来源：http://aa.colortex.cn

enum Color { case red, green }
来源：http://zm.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://nv.hnjuh.cn

guard let x = opt else { return }
来源：http://dz.nicolike.cn

[T30] Swift：协议
来源：http://ew.asd995.cn

protocol Shape { func area() -> Double }
来源：http://qu.9csxet.cn

[T31] Lua：Hello World
来源：http://pw.jianghongdianzi.cn

print("Hello")
来源：http://se.lnxyls.cn

[T32] Lua：局部变量
来源：http://xh.yuntaijiaju.cn

local a = 1
来源：http://aq.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://to.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eh.gzmigu.cn

[T34] Lua：遍历表
来源：http://hd.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ml.haigaiapp.cn

[T35] Lua：字典表
来源：http://nj.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://oe.shxzukj.cn

[T36] Lua：函数
来源：http://mt.nicolike.cn

function add(a, b) return a + b end
来源：http://uf.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://eq.wgjwhj.cn

"a" .. "b"
来源：http://bg.hnjuh.cn

[T38] Lua：条件
来源：http://jm.shxzukj.cn

if x > 0 then print("正") end
来源：http://tu.panjiajie.cn

[T39] Lua：模式匹配
来源：http://ow.shtwfgs.cn

string.find(s, "%d+")
来源：http://gq.shxzukj.cn

[T40] Lua：元表
来源：http://hz.nicolike.cn

setmetatable({}, { __index = base })
来源：http://po.gzmigu.cn

[T41] Perl：Hello World
来源：http://wh.9csxet.cn

print "Hello\n";
来源：http://mf.hnjuh.cn

[T42] Perl：变量类型
来源：http://pf.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gw.szxytkj.cn

[T43] Perl：字符串插值
来源：http://al.panjiajie.cn

"值: $a"
来源：http://om.szxytkj.cn

[T44] Perl：条件
来源：http://pt.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://ge.huanxung.cn

[T45] Perl：数组遍历
来源：http://dd.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ac.szxytkj.cn

[T46] Perl：哈希操作
来源：http://jf.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://we.shxzskj.cn

[T47] Perl：正则捕获
来源：http://dg.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wv.asd995.cn

[T48] Perl：正则替换
来源：http://vh.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ba.haigaiapp.cn

[T49] Perl：函数
来源：http://hh.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mc.hahajie.cn

[T50] Perl：逐行读文件
来源：http://zc.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rh.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ab.wgjwhj.cn

[T51] Scala：Hello World
来源：http://gn.jianghongdianzi.cn

println("Hello")
来源：http://xg.wgjwhj.cn

[T52] Scala：变量
来源：http://bl.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://tz.nszjky.cn

[T53] Scala：字符串插值
来源：http://hk.huanxung.cn

s"值: $b"
来源：http://su.yuexingan06.cn

[T54] Scala：集合映射
来源：http://rv.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://pz.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://ka.huixiangedu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ov.szsharing.cn

[T56] Scala：样例类
来源：http://bj.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://iz.hahajie.cn

[T57] Scala：模式匹配
来源：http://uo.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zs.jctech888.com.cn

[T58] Scala：函数定义
来源：http://fl.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xj.wgjwhj.cn

[T59] Scala：循环
来源：http://qk.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://vx.szxytkj.cn

[T60] Scala：折叠
来源：http://sg.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cu.bjjhwx.cn

================================================================================
来源：http://qc.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tm.colortex.cn

================================================================================
来源：http://ff.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://az.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nl.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://yx.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wr.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://tb.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zz.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://qk.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ii.szsharing.cn

[U05] Py：列表去重且保序
来源：http://ey.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://ib.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://ac.bookmarksfly.cn

{**a, **b}
来源：http://id.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://gv.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://db.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://ak.huanxung.cn

[y for x in nested for y in x]
来源：http://ai.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://kk.huixinmuqiang.cn

max(d, key=d.get)
来源：http://hl.shxzukj.cn

[U10] Py：按值排序字典
来源：http://tp.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zo.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://jk.chemitech.net.cn

(x * 2 for x in arr)
来源：http://xi.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kz.colortex.cn

Counter(arr).most_common(3)
来源：http://yo.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://dr.hahajie.cn

deque(maxlen=10)
来源：http://tf.huanxung.cn

[U14] Py：分组收集到列表
来源：http://bq.yuntaijiaju.cn

defaultdict(list)
来源：http://wj.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://lt.shxzskj.cn

t = time.perf_counter()
来源：http://cc.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://jf.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vt.jctech888.com.cn

[U17] Py：初始化日志
来源：http://ip.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://zp.shxzukj.cn

[U18] Py：预编译正则
来源：http://kh.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://fg.szsharing.cn

[U19] Py：正则替换带回调
来源：http://km.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pf.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://qa.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://yy.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://xw.gzmigu.cn

@contextlib.contextmanager
来源：http://dt.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://up.gzmigu.cn

list(zip(*m))
来源：http://ct.asd995.cn

[U23] Py：分块读取大文件
来源：http://io.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nj.szxytkj.cn

[U24] Py：路径操作
来源：http://ho.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ey.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://aj.lnxyls.cn

csv.DictReader(f)
来源：http://rq.shxzukj.cn

[U26] Py：并发下载
来源：http://wn.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ho.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ti.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://cy.yuexingan06.cn

[U28] Py：类型别名
来源：http://mi.shtwfgs.cn

UserId = int
来源：http://al.bjjhwx.cn

[U29] Py：属性校验
来源：http://bq.shxzukj.cn

@property 与 @x.setter 配合
来源：http://mc.panjiajie.cn

[U30] Py：数据类
来源：http://lo.huixiangedu.cn

@dataclass(slots=True)
来源：http://hx.panjiajie.cn

[U31] Py：单测
来源：http://hx.muxihuayi.cn

python -m pytest -q
来源：http://qn.haigaiapp.cn

[U32] Py：代码格式化
来源：http://vg.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://fr.wgjwhj.cn

[U33] Py：打包发布
来源：http://mz.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://ta.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://ka.haigaiapp.cn

chardet.detect(raw)
来源：http://dy.huanxung.cn

[U35] Py：发送邮件
来源：http://tz.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fo.nicolike.cn

[U36] Py：定时任务
来源：http://bt.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://pu.szsharing.cn

[U37] Py：读写 Excel
来源：http://bk.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sc.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://pk.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://am.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://ge.newstarts.cn

sys.stdout.isatty()
来源：http://pi.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ni.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://vy.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://jo.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ql.jianghongdianzi.cn

[U42] PHP：PSR-4 自动加载
来源：http://te.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fp.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://yd.shtwfgs.cn

namespace App\Http;
来源：http://sm.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://em.shxzukj.cn

declare(strict_types=1);
来源：http://de.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://su.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lf.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://og.bookmarksfly.cn

?string $name = null
来源：http://dh.asd995.cn

[U47] PHP：联合类型
来源：http://aj.gzmigu.cn

int|string $id
来源：http://cv.jianghongdianzi.cn

[U48] PHP：纯枚举
来源：http://wd.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uq.huixiangedu.cn

[U49] PHP：只读属性
来源：http://vy.hnjuh.cn

public readonly string $name
来源：http://wa.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://qe.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://hd.lnxyls.cn

[U51] PHP：数组解构
来源：http://fb.haigaiapp.cn

[$a, $b] = $arr;
来源：http://xa.haigaiapp.cn

[U52] PHP：箭头函数
来源：http://bv.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://aw.chemitech.net.cn

[U53] PHP：空合并运算符
来源：http://ux.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://dy.521024.cn

[U54] PHP：空安全调用
来源：http://mg.newstarts.cn

$obj?->method()
来源：http://vb.nicolike.cn

[U55] PHP：match 表达式
来源：http://vp.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dw.panjiajie.cn

[U56] PHP：命名参数
来源：http://hp.nszjky.cn

f(a: 1, b: 2)
来源：http://ll.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://ec.nszjky.cn

"值: {$a}"
来源：http://ev.gzmigu.cn

[U58] PHP：数组三件套
来源：http://cr.haigaiapp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gq.nszjky.cn

[U59] PHP：自定义排序
来源：http://nb.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oh.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://wh.huixiangedu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bv.lnxyls.cn

[U61] PHP：正则
来源：http://bi.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zj.nszjky.cn

[U62] PHP：日期对象
来源：http://xo.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://un.huanxung.cn

[U63] PHP：文件读写
来源：http://wk.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hj.huixinmuqiang.cn

[U64] PHP：目录遍历
来源：http://ud.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://vj.nicolike.cn

[U65] PHP：会话
来源：http://dh.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://un.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://ge.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oy.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://pm.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://su.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://qq.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pn.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://rk.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vs.521024.cn

[U70] PHP：PDO 事务
来源：http://kx.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://di.lnxyls.cn

[U71] PHP：抛出异常
来源：http://jc.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://wd.asd995.cn

[U72] PHP：写错误日志
来源：http://or.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://gz.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://xb.huixiangedu.cn

parse_ini_file("config.ini", true)
来源：http://bq.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://bu.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://il.shtwfgs.cn


<!-- 参考信息 -->