代发 wailian999

while (std::getline(in, line)) { }
来源：http://ng.panjiajie.cn

[S49] C++：写文件
来源：http://kb.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://st.huixiangedu.cn

[S50] C++：格式化数字
来源：http://ur.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mf.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://nv.muxihuayi.cn

static_cast<double>(a) / b
来源：http://hu.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yi.colortex.cn

int size() const noexcept { return n_; }
来源：http://xp.muxihuayi.cn

[S53] C++：移动语义
来源：http://ri.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://cr.yuexingan06.cn

[S54] C++：异常处理
来源：http://ky.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lw.newstarts.cn

[S55] C++：结构化绑定
来源：http://jw.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zh.muxihuayi.cn

[S56] C++：optional
来源：http://fs.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cc.shxzukj.cn

[S57] C++：编译期常量
来源：http://uo.nicolike.cn

constexpr int N = 10;
来源：http://un.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://zz.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://un.newstarts.cn

[S59] C++：静态断言
来源：http://kd.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ej.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://on.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cs.asd995.cn

================================================================================
来源：http://cr.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dc.yuntaijiaju.cn

================================================================================
来源：http://eq.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://tu.hnjuh.cn

println("Hello")
来源：http://td.haigaiapp.cn

[T02] Kotlin：变量
来源：http://kb.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ez.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://zb.9csxet.cn

"值: $b"
来源：http://jr.shxzukj.cn

[T04] Kotlin：空安全
来源：http://gy.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://tn.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://pu.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bw.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://dt.hnjuh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kh.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://jb.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ph.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://rg.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://ap.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://nr.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://cv.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://cd.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dc.hahajie.cn

[T11] Kotlin：协程
来源：http://kg.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xr.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://lk.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://ny.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://vd.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://wl.shxzukj.cn

[T14] Kotlin：循环
来源：http://bi.huanxung.cn

for (i in 1..10) println(i)
来源：http://jc.asd995.cn

[T15] Kotlin：接口
来源：http://bi.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://bo.gzmigu.cn

[T16] Swift：Hello World
来源：http://ji.yuntaijiaju.cn

print("Hello")
来源：http://xt.hahajie.cn

[T17] Swift：变量与常量
来源：http://bs.hahajie.cn

var a = 1;  let b = 2
来源：http://xd.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://gk.huixinmuqiang.cn

"值: \(b)"
来源：http://ow.szsharing.cn

[T19] Swift：可选绑定
来源：http://og.bjjhwx.cn

if let n = opt { print(n) }
来源：http://qe.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://yg.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://no.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://wz.bookmarksfly.cn

for x in a { print(x) }
来源：http://of.szsharing.cn

[T22] Swift：字典
来源：http://ca.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://my.hahajie.cn

[T23] Swift：函数
来源：http://am.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://po.newstarts.cn

[T24] Swift：闭包
来源：http://bb.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qn.wgjwhj.cn

[T25] Swift：结构体
来源：http://hx.gzmigu.cn

struct P { var x: Int }
来源：http://us.jianghongdianzi.cn

[T26] Swift：类与重写
来源：http://fc.shxzukj.cn

class A: Base { override func f() {} }
来源：http://gj.jctech888.com.cn

[T27] Swift：错误处理
来源：http://pe.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://tr.muxihuayi.cn

[T28] Swift：枚举
来源：http://af.huixiangedu.cn

enum Color { case red, green }
来源：http://jz.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://dx.newstarts.cn

guard let x = opt else { return }
来源：http://cp.yuntaijiaju.cn

[T30] Swift：协议
来源：http://wk.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ua.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://sv.nicolike.cn

print("Hello")
来源：http://ep.bjjhwx.cn

[T32] Lua：局部变量
来源：http://rh.9csxet.cn

local a = 1
来源：http://px.nicolike.cn

[T33] Lua：表（数组）
来源：http://iz.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rh.panjiajie.cn

[T34] Lua：遍历表
来源：http://tp.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lo.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://ww.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://in.jianghongdianzi.cn

[T36] Lua：函数
来源：http://xo.wgjwhj.cn

function add(a, b) return a + b end
来源：http://pl.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://hb.yuexingan06.cn

"a" .. "b"
来源：http://zu.9csxet.cn

[T38] Lua：条件
来源：http://yw.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://zx.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://qi.hahajie.cn

string.find(s, "%d+")
来源：http://eq.9csxet.cn

[T40] Lua：元表
来源：http://cl.9csxet.cn

setmetatable({}, { __index = base })
来源：http://oh.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://hv.hnjuh.cn

print "Hello\n";
来源：http://cq.szxytkj.cn

[T42] Perl：变量类型
来源：http://xb.huixinmuqiang.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gd.521024.cn

[T43] Perl：字符串插值
来源：http://gk.asd995.cn

"值: $a"
来源：http://sc.asd995.cn

[T44] Perl：条件
来源：http://zo.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://bs.hnjuh.cn

[T45] Perl：数组遍历
来源：http://rn.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://ne.panjiajie.cn

[T46] Perl：哈希操作
来源：http://ae.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ki.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ja.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ah.jctech888.com.cn

[T48] Perl：正则替换
来源：http://zi.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://er.asd995.cn

[T49] Perl：函数
来源：http://yh.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://om.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://vu.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ku.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://hr.9csxet.cn

[T51] Scala：Hello World
来源：http://ap.shxzukj.cn

println("Hello")
来源：http://xg.521024.cn

[T52] Scala：变量
来源：http://qc.hnjuh.cn

val a = 1;  var b = 2
来源：http://pu.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://xv.colortex.cn

s"值: $b"
来源：http://ft.panjiajie.cn

[T54] Scala：集合映射
来源：http://cr.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://no.panjiajie.cn

[T55] Scala：集合过滤
来源：http://sx.yuexingan06.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dz.gzmigu.cn

[T56] Scala：样例类
来源：http://hb.nicolike.cn

case class User(name: String, age: Int)
来源：http://rz.shxzukj.cn

[T57] Scala：模式匹配
来源：http://mg.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gq.huixiangedu.cn

[T58] Scala：函数定义
来源：http://ec.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sy.jctech888.com.cn

[T59] Scala：循环
来源：http://wn.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://tt.colortex.cn

[T60] Scala：折叠
来源：http://pc.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vn.jianghongdianzi.cn

================================================================================
来源：http://bc.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pe.bjjhwx.cn

================================================================================
来源：http://fs.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://pr.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gj.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://su.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lt.yuntaijiaju.cn

[U03] Py：加载 .env 配置
来源：http://at.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pa.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://hk.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gp.newstarts.cn

[U05] Py：列表去重且保序
来源：http://jt.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://il.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://pe.521024.cn

{**a, **b}
来源：http://nz.asd995.cn

[U07] Py：反转字典键值
来源：http://ny.9csxet.cn

{v: k for k, v in d.items()}
来源：http://ne.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://do.shxzskj.cn

[y for x in nested for y in x]
来源：http://bc.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://ci.shxzukj.cn

max(d, key=d.get)
来源：http://li.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://eh.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uz.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://de.szsharing.cn

(x * 2 for x in arr)
来源：http://ur.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rw.hnjuh.cn

Counter(arr).most_common(3)
来源：http://fg.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://da.jctech888.com.cn

deque(maxlen=10)
来源：http://mb.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://kq.yuntaijiaju.cn

defaultdict(list)
来源：http://ja.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://yw.wgjwhj.cn

t = time.perf_counter()
来源：http://ov.nszjky.cn

[U16] Py：命令行参数解析
来源：http://xb.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xu.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://dp.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://wu.haigaiapp.cn

[U18] Py：预编译正则
来源：http://zl.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://xk.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://lj.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ok.colortex.cn

[U20] Py：缓存函数结果
来源：http://rg.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://lb.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://gi.lnxyls.cn

@contextlib.contextmanager
来源：http://ua.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://ru.hnjuh.cn

list(zip(*m))
来源：http://sh.nicolike.cn

[U23] Py：分块读取大文件
来源：http://dh.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ml.shxzukj.cn

[U24] Py：路径操作
来源：http://bu.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ky.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://vu.gzmigu.cn

csv.DictReader(f)
来源：http://ul.szsharing.cn

[U26] Py：并发下载
来源：http://ze.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ov.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://kl.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://uw.nszjky.cn

[U28] Py：类型别名
来源：http://uj.asd995.cn

UserId = int
来源：http://tv.chemitech.net.cn

[U29] Py：属性校验
来源：http://yl.gzmigu.cn

@property 与 @x.setter 配合
来源：http://wq.szsharing.cn

[U30] Py：数据类
来源：http://vc.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://ph.gzmigu.cn

[U31] Py：单测
来源：http://vf.gzmigu.cn

python -m pytest -q
来源：http://oq.huixiangedu.cn

[U32] Py：代码格式化
来源：http://el.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://tv.haigaiapp.cn

[U33] Py：打包发布
来源：http://zc.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ru.shtwfgs.cn

[U34] Py：判断编码
来源：http://pn.nszjky.cn

chardet.detect(raw)
来源：http://an.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://da.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://go.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://jl.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://hn.lnxyls.cn

[U37] Py：读写 Excel
来源：http://yi.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zt.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://vy.hahajie.cn

Path(__file__).resolve().parent
来源：http://gm.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://gb.bookmarksfly.cn

sys.stdout.isatty()
来源：http://ac.hahajie.cn

[U40] Py：打印到标准错误
来源：http://zv.colortex.cn

print("err", file=sys.stderr)
来源：http://xy.jctech888.com.cn

[U41] PHP：初始化 Composer 项目
来源：http://yi.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vh.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://up.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eu.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://ka.szsharing.cn

namespace App\Http;
来源：http://zg.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://qj.bjjhwx.cn

declare(strict_types=1);
来源：http://fe.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://ub.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xw.gzmigu.cn

[U46] PHP：可空类型
来源：http://gf.hahajie.cn

?string $name = null
来源：http://ey.szxytkj.cn

[U47] PHP：联合类型
来源：http://ue.gzmigu.cn

int|string $id
来源：http://op.colortex.cn

[U48] PHP：纯枚举
来源：http://hd.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xz.shtwfgs.cn

[U49] PHP：只读属性
来源：http://fd.asd995.cn

public readonly string $name
来源：http://yk.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://np.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://tx.haigaiapp.cn

[U51] PHP：数组解构
来源：http://fa.hnjuh.cn

[$a, $b] = $arr;
来源：http://zd.newstarts.cn

[U52] PHP：箭头函数
来源：http://ps.colortex.cn

$double = fn($x) => $x * 2;
来源：http://jy.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://yy.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://zc.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://mw.muxihuayi.cn

$obj?->method()
来源：http://tm.szsharing.cn

[U55] PHP：match 表达式
来源：http://rv.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qv.9csxet.cn

[U56] PHP：命名参数
来源：http://xf.jctech888.com.cn

f(a: 1, b: 2)
来源：http://pm.hnjuh.cn

[U57] PHP：字符串插值
来源：http://yq.haigaiapp.cn

"值: {$a}"
来源：http://np.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://nf.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cg.nicolike.cn

[U59] PHP：自定义排序
来源：http://se.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yr.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://uw.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vw.yuntaijiaju.cn

[U61] PHP：正则
来源：http://zw.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jd.nszjky.cn

[U62] PHP：日期对象
来源：http://uz.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eg.hahajie.cn

[U63] PHP：文件读写
来源：http://ej.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qr.asd995.cn

[U64] PHP：目录遍历
来源：http://zp.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://vh.nicolike.cn

[U65] PHP：会话
来源：http://kv.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://em.shxzskj.cn

[U66] PHP：设置 Cookie
来源：http://nt.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xl.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://ve.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://op.szsharing.cn

[U68] PHP：PDO 连接
来源：http://nt.nicolike.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pl.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://qd.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hn.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://sx.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dk.lnxyls.cn

[U71] PHP：抛出异常
来源：http://yj.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://dz.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://ov.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://ys.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://ha.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://vg.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://cp.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://aa.jianghongdianzi.cn


<!-- 参考信息 -->