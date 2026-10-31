代发 wailian999

while (std::getline(in, line)) { }
来源：http://xw.gzmigu.cn

[S49] C++：写文件
来源：http://mg.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://li.chemitech.net.cn

[S50] C++：格式化数字
来源：http://pr.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cy.asd995.cn

[S51] C++：显式类型转换
来源：http://js.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://xn.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://hs.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://wm.szsharing.cn

[S53] C++：移动语义
来源：http://wa.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://jz.lnxyls.cn

[S54] C++：异常处理
来源：http://da.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lm.huixinmuqiang.cn

[S55] C++：结构化绑定
来源：http://ei.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uj.jianghongdianzi.cn

[S56] C++：optional
来源：http://ke.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hy.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ny.hahajie.cn

constexpr int N = 10;
来源：http://ny.muxihuayi.cn

[S58] C++：命名空间
来源：http://pt.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://kx.szsharing.cn

[S59] C++：静态断言
来源：http://zx.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mn.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://fw.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ef.521024.cn

================================================================================
来源：http://fz.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xs.huixiangedu.cn

================================================================================
来源：http://jp.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://ko.lnxyls.cn

println("Hello")
来源：http://xb.szxytkj.cn

[T02] Kotlin：变量
来源：http://pj.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qy.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://hv.chemitech.net.cn

"值: $b"
来源：http://bj.asd995.cn

[T04] Kotlin：空安全
来源：http://cn.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://gh.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://ts.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bd.asd995.cn

[T06] Kotlin：集合映射
来源：http://xg.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://te.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://vb.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gj.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://ll.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://gr.colortex.cn

[T09] Kotlin：扩展函数
来源：http://og.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://wa.nszjky.cn

[T10] Kotlin：默认参数
来源：http://le.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kn.shxzskj.cn

[T11] Kotlin：协程
来源：http://jl.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ug.szsharing.cn

[T12] Kotlin：解构声明
来源：http://fr.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://dy.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://ku.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://jw.hnjuh.cn

[T14] Kotlin：循环
来源：http://wl.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://zo.szsharing.cn

[T15] Kotlin：接口
来源：http://ak.9csxet.cn

interface Shape { fun area(): Double }
来源：http://ve.panjiajie.cn

[T16] Swift：Hello World
来源：http://hp.hahajie.cn

print("Hello")
来源：http://vj.521024.cn

[T17] Swift：变量与常量
来源：http://vk.bjjhwx.cn

var a = 1;  let b = 2
来源：http://xh.panjiajie.cn

[T18] Swift：字符串插值
来源：http://va.nicolike.cn

"值: \(b)"
来源：http://cm.hahajie.cn

[T19] Swift：可选绑定
来源：http://te.wgjwhj.cn

if let n = opt { print(n) }
来源：http://bd.shtwfgs.cn

[T20] Swift：数组操作
来源：http://or.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ma.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://uc.panjiajie.cn

for x in a { print(x) }
来源：http://ug.panjiajie.cn

[T22] Swift：字典
来源：http://uo.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tl.521024.cn

[T23] Swift：函数
来源：http://qt.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nt.huanxung.cn

[T24] Swift：闭包
来源：http://jy.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rz.nszjky.cn

[T25] Swift：结构体
来源：http://qa.muxihuayi.cn

struct P { var x: Int }
来源：http://et.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ci.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://sl.muxihuayi.cn

[T27] Swift：错误处理
来源：http://gq.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://vr.yuexingan06.cn

[T28] Swift：枚举
来源：http://ui.bjjhwx.cn

enum Color { case red, green }
来源：http://ke.asd995.cn

[T29] Swift：guard 提前返回
来源：http://rh.muxihuayi.cn

guard let x = opt else { return }
来源：http://vf.jctech888.com.cn

[T30] Swift：协议
来源：http://lr.asd995.cn

protocol Shape { func area() -> Double }
来源：http://al.gzmigu.cn

[T31] Lua：Hello World
来源：http://yi.shtwfgs.cn

print("Hello")
来源：http://ib.shxzskj.cn

[T32] Lua：局部变量
来源：http://vt.szsharing.cn

local a = 1
来源：http://tl.nszjky.cn

[T33] Lua：表（数组）
来源：http://fe.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nv.shtwfgs.cn

[T34] Lua：遍历表
来源：http://zm.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yc.shxzskj.cn

[T35] Lua：字典表
来源：http://ga.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://jh.9csxet.cn

[T36] Lua：函数
来源：http://kj.jctech888.com.cn

function add(a, b) return a + b end
来源：http://hx.9csxet.cn

[T37] Lua：字符串拼接
来源：http://fb.yuntaijiaju.cn

"a" .. "b"
来源：http://jj.hnjuh.cn

[T38] Lua：条件
来源：http://zp.nszjky.cn

if x > 0 then print("正") end
来源：http://dl.panjiajie.cn

[T39] Lua：模式匹配
来源：http://gi.521024.cn

string.find(s, "%d+")
来源：http://aj.nszjky.cn

[T40] Lua：元表
来源：http://ee.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://bq.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://am.nszjky.cn

print "Hello\n";
来源：http://tl.hahajie.cn

[T42] Perl：变量类型
来源：http://ce.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jn.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://hv.huixiangedu.cn

"值: $a"
来源：http://yg.521024.cn

[T44] Perl：条件
来源：http://yg.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://fb.9csxet.cn

[T45] Perl：数组遍历
来源：http://cf.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://mj.nszjky.cn

[T46] Perl：哈希操作
来源：http://qc.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mo.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://sg.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ye.wgjwhj.cn

[T48] Perl：正则替换
来源：http://mb.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://le.shxzskj.cn

[T49] Perl：函数
来源：http://tv.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yl.newstarts.cn

[T50] Perl：逐行读文件
来源：http://yg.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dj.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://uf.szsharing.cn

[T51] Scala：Hello World
来源：http://kn.shtwfgs.cn

println("Hello")
来源：http://ja.newstarts.cn

[T52] Scala：变量
来源：http://fn.panjiajie.cn

val a = 1;  var b = 2
来源：http://pz.9csxet.cn

[T53] Scala：字符串插值
来源：http://lz.9csxet.cn

s"值: $b"
来源：http://vs.asd995.cn

[T54] Scala：集合映射
来源：http://of.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://ua.hahajie.cn

[T55] Scala：集合过滤
来源：http://ns.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cp.9csxet.cn

[T56] Scala：样例类
来源：http://bg.9csxet.cn

case class User(name: String, age: Int)
来源：http://rb.521024.cn

[T57] Scala：模式匹配
来源：http://ld.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ga.shtwfgs.cn

[T58] Scala：函数定义
来源：http://kq.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mt.lnxyls.cn

[T59] Scala：循环
来源：http://sp.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ad.hahajie.cn

[T60] Scala：折叠
来源：http://ef.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kh.szsharing.cn

================================================================================
来源：http://ax.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qs.jctech888.com.cn

================================================================================
来源：http://sq.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://ti.szxytkj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fr.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://uc.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hn.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://rl.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qa.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://to.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ww.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://sq.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://qb.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://ln.bookmarksfly.cn

{**a, **b}
来源：http://vi.szxytkj.cn

[U07] Py：反转字典键值
来源：http://xp.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://ok.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://jx.nszjky.cn

[y for x in nested for y in x]
来源：http://si.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://cc.hnjuh.cn

max(d, key=d.get)
来源：http://ou.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://pi.huanxung.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sp.szsharing.cn

[U11] Py：生成器表达式
来源：http://ai.jctech888.com.cn

(x * 2 for x in arr)
来源：http://gv.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ej.chemitech.net.cn

Counter(arr).most_common(3)
来源：http://wk.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://sl.muxihuayi.cn

deque(maxlen=10)
来源：http://bm.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://he.wgjwhj.cn

defaultdict(list)
来源：http://vw.hahajie.cn

[U15] Py：高精度计时
来源：http://rw.newstarts.cn

t = time.perf_counter()
来源：http://dr.colortex.cn

[U16] Py：命令行参数解析
来源：http://of.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oy.haigaiapp.cn

[U17] Py：初始化日志
来源：http://pw.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://mt.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://fi.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://xu.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://dv.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xj.9csxet.cn

[U20] Py：缓存函数结果
来源：http://bl.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://dm.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://ay.shxzukj.cn

@contextlib.contextmanager
来源：http://vo.hahajie.cn

[U22] Py：矩阵转置
来源：http://ou.szxytkj.cn

list(zip(*m))
来源：http://fz.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://ok.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fo.shtwfgs.cn

[U24] Py：路径操作
来源：http://sb.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cx.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://mp.huixinmuqiang.cn

csv.DictReader(f)
来源：http://zl.9csxet.cn

[U26] Py：并发下载
来源：http://to.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yy.nicolike.cn

[U27] Py：异步 HTTP
来源：http://bf.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://im.bookmarksfly.cn

[U28] Py：类型别名
来源：http://fc.bookmarksfly.cn

UserId = int
来源：http://if.shtwfgs.cn

[U29] Py：属性校验
来源：http://xb.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://yw.huixinmuqiang.cn

[U30] Py：数据类
来源：http://mn.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://ck.shtwfgs.cn

[U31] Py：单测
来源：http://xv.jianghongdianzi.cn

python -m pytest -q
来源：http://nb.gzmigu.cn

[U32] Py：代码格式化
来源：http://ig.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://bd.hahajie.cn

[U33] Py：打包发布
来源：http://fm.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://bc.newstarts.cn

[U34] Py：判断编码
来源：http://no.muxihuayi.cn

chardet.detect(raw)
来源：http://fz.lnxyls.cn

[U35] Py：发送邮件
来源：http://vo.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zp.huanxung.cn

[U36] Py：定时任务
来源：http://oo.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://uz.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://mb.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yg.jianghongdianzi.cn

[U38] Py：获取脚本所在目录
来源：http://kh.bookmarksfly.cn

Path(__file__).resolve().parent
来源：http://dv.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://hc.panjiajie.cn

sys.stdout.isatty()
来源：http://gg.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://tc.szxytkj.cn

print("err", file=sys.stderr)
来源：http://up.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://lm.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wd.szxytkj.cn

[U42] PHP：PSR-4 自动加载
来源：http://kv.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kq.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://fx.nicolike.cn

namespace App\Http;
来源：http://vx.szsharing.cn

[U44] PHP：开启严格类型
来源：http://xg.panjiajie.cn

declare(strict_types=1);
来源：http://le.jctech888.com.cn

[U45] PHP：类型声明与返回类型
来源：http://ij.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lk.yuexingan06.cn

[U46] PHP：可空类型
来源：http://on.szxytkj.cn

?string $name = null
来源：http://az.shxzukj.cn

[U47] PHP：联合类型
来源：http://me.shxzukj.cn

int|string $id
来源：http://zh.bookmarksfly.cn

[U48] PHP：纯枚举
来源：http://fh.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eh.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://yg.chemitech.net.cn

public readonly string $name
来源：http://db.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://po.9csxet.cn

public function __construct(private int $id) {}
来源：http://ob.szsharing.cn

[U51] PHP：数组解构
来源：http://by.521024.cn

[$a, $b] = $arr;
来源：http://cc.521024.cn

[U52] PHP：箭头函数
来源：http://ps.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://fd.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://tw.panjiajie.cn

$v = $a ?? $b ?? "default";
来源：http://sv.chemitech.net.cn

[U54] PHP：空安全调用
来源：http://of.lnxyls.cn

$obj?->method()
来源：http://la.szsharing.cn

[U55] PHP：match 表达式
来源：http://oc.521024.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fn.9csxet.cn

[U56] PHP：命名参数
来源：http://wg.lnxyls.cn

f(a: 1, b: 2)
来源：http://ui.szxytkj.cn

[U57] PHP：字符串插值
来源：http://pl.hnjuh.cn

"值: {$a}"
来源：http://tp.shxzskj.cn

[U58] PHP：数组三件套
来源：http://ut.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kq.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://cb.panjiajie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jg.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://uf.jctech888.com.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tt.lnxyls.cn

[U61] PHP：正则
来源：http://na.szxytkj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://km.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://mc.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kl.nicolike.cn

[U63] PHP：文件读写
来源：http://yn.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rb.newstarts.cn

[U64] PHP：目录遍历
来源：http://xg.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://xw.panjiajie.cn

[U65] PHP：会话
来源：http://qe.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://li.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://ga.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zx.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://uv.nicolike.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tk.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://zu.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jw.521024.cn

[U69] PHP：PDO 预处理
来源：http://yq.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://so.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://qf.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qj.huixinmuqiang.cn

[U71] PHP：抛出异常
来源：http://dn.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://xb.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://ob.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://rg.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://ty.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://oa.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://gl.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://hz.lnxyls.cn


<!-- 参考信息 -->