代发 wailian999

while (std::getline(in, line)) { }
来源：http://mt.muxihuayi.cn

[S49] C++：写文件
来源：http://zm.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pg.wgjwhj.cn

[S50] C++：格式化数字
来源：http://px.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pk.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://hm.shtwfgs.cn

static_cast<double>(a) / b
来源：http://ii.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://wr.nszjky.cn

int size() const noexcept { return n_; }
来源：http://hn.shxzukj.cn

[S53] C++：移动语义
来源：http://xo.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://lk.szsharing.cn

[S54] C++：异常处理
来源：http://fh.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ux.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://oq.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ee.521024.cn

[S56] C++：optional
来源：http://fk.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kf.bjjhwx.cn

[S57] C++：编译期常量
来源：http://ny.szsharing.cn

constexpr int N = 10;
来源：http://vk.chemitech.net.cn

[S58] C++：命名空间
来源：http://zi.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://hx.shxzskj.cn

[S59] C++：静态断言
来源：http://uc.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hf.jctech888.com.cn

[S60] C++：遍历并删除元素
来源：http://nh.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ma.shxzukj.cn

================================================================================
来源：http://bn.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yv.jctech888.com.cn

================================================================================
来源：http://eq.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://rg.shxzukj.cn

println("Hello")
来源：http://oz.nicolike.cn

[T02] Kotlin：变量
来源：http://um.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ss.colortex.cn

[T03] Kotlin：字符串模板
来源：http://zl.szsharing.cn

"值: $b"
来源：http://aa.nicolike.cn

[T04] Kotlin：空安全
来源：http://rx.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://qg.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://lh.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yq.colortex.cn

[T06] Kotlin：集合映射
来源：http://kl.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fo.521024.cn

[T07] Kotlin：集合过滤
来源：http://gq.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://un.szsharing.cn

[T08] Kotlin：数据类
来源：http://fl.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ll.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://yv.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://pw.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://wy.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xu.shxzukj.cn

[T11] Kotlin：协程
来源：http://hw.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ud.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://yw.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://lh.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://iz.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ka.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://zm.szxytkj.cn

for (i in 1..10) println(i)
来源：http://xk.newstarts.cn

[T15] Kotlin：接口
来源：http://qv.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://kp.haigaiapp.cn

[T16] Swift：Hello World
来源：http://sb.9csxet.cn

print("Hello")
来源：http://iy.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://zt.asd995.cn

var a = 1;  let b = 2
来源：http://mh.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://nf.nicolike.cn

"值: \(b)"
来源：http://nu.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://py.shxzskj.cn

if let n = opt { print(n) }
来源：http://tw.bjjhwx.cn

[T20] Swift：数组操作
来源：http://bn.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tk.shxzukj.cn

[T21] Swift：遍历
来源：http://kb.huanxung.cn

for x in a { print(x) }
来源：http://ne.nicolike.cn

[T22] Swift：字典
来源：http://cb.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kc.szsharing.cn

[T23] Swift：函数
来源：http://pm.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nt.colortex.cn

[T24] Swift：闭包
来源：http://fw.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pk.521024.cn

[T25] Swift：结构体
来源：http://tq.panjiajie.cn

struct P { var x: Int }
来源：http://dz.nszjky.cn

[T26] Swift：类与重写
来源：http://qs.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://ma.shtwfgs.cn

[T27] Swift：错误处理
来源：http://je.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://fq.newstarts.cn

[T28] Swift：枚举
来源：http://zx.szxytkj.cn

enum Color { case red, green }
来源：http://ty.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://en.hnjuh.cn

guard let x = opt else { return }
来源：http://uv.szxytkj.cn

[T30] Swift：协议
来源：http://aa.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://hn.lnxyls.cn

[T31] Lua：Hello World
来源：http://yb.panjiajie.cn

print("Hello")
来源：http://lx.shxzukj.cn

[T32] Lua：局部变量
来源：http://hz.asd995.cn

local a = 1
来源：http://gk.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://wr.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yh.shtwfgs.cn

[T34] Lua：遍历表
来源：http://vc.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ix.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://fw.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://hj.shxzskj.cn

[T36] Lua：函数
来源：http://wi.shxzukj.cn

function add(a, b) return a + b end
来源：http://tz.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://xh.haigaiapp.cn

"a" .. "b"
来源：http://hk.newstarts.cn

[T38] Lua：条件
来源：http://rb.newstarts.cn

if x > 0 then print("正") end
来源：http://ar.asd995.cn

[T39] Lua：模式匹配
来源：http://zr.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://tp.szsharing.cn

[T40] Lua：元表
来源：http://gh.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://vx.newstarts.cn

[T41] Perl：Hello World
来源：http://bj.yuntaijiaju.cn

print "Hello\n";
来源：http://hk.lnxyls.cn

[T42] Perl：变量类型
来源：http://qp.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gw.nszjky.cn

[T43] Perl：字符串插值
来源：http://sk.szxytkj.cn

"值: $a"
来源：http://ww.asd995.cn

[T44] Perl：条件
来源：http://zi.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://ve.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ku.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://xd.hahajie.cn

[T46] Perl：哈希操作
来源：http://mm.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lj.shxzskj.cn

[T47] Perl：正则捕获
来源：http://qi.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yz.lnxyls.cn

[T48] Perl：正则替换
来源：http://wr.shxzukj.cn

$s =~ s/old/new/g;
来源：http://mz.shtwfgs.cn

[T49] Perl：函数
来源：http://mm.nszjky.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ju.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://is.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kp.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://ky.chemitech.net.cn

[T51] Scala：Hello World
来源：http://dw.shxzukj.cn

println("Hello")
来源：http://zo.bjjhwx.cn

[T52] Scala：变量
来源：http://mr.asd995.cn

val a = 1;  var b = 2
来源：http://yx.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://bz.lnxyls.cn

s"值: $b"
来源：http://fr.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://hg.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://be.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://oj.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mt.shxzskj.cn

[T56] Scala：样例类
来源：http://ta.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://rj.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://us.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gd.haigaiapp.cn

[T58] Scala：函数定义
来源：http://tz.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ks.521024.cn

[T59] Scala：循环
来源：http://gs.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://fc.shxzskj.cn

[T60] Scala：折叠
来源：http://ft.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fs.huixiangedu.cn

================================================================================
来源：http://iy.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yo.jctech888.com.cn

================================================================================
来源：http://vw.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://lf.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gu.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://zt.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ht.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://tq.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pl.szsharing.cn

[U04] Py：变量调试打印
来源：http://je.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cf.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://mf.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://cn.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://bt.bjjhwx.cn

{**a, **b}
来源：http://yn.shxzukj.cn

[U07] Py：反转字典键值
来源：http://xc.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://eq.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://fy.nszjky.cn

[y for x in nested for y in x]
来源：http://hy.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://zt.wgjwhj.cn

max(d, key=d.get)
来源：http://uv.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ou.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://en.gzmigu.cn

[U11] Py：生成器表达式
来源：http://vj.jctech888.com.cn

(x * 2 for x in arr)
来源：http://xm.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://og.9csxet.cn

Counter(arr).most_common(3)
来源：http://hn.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ye.huixinmuqiang.cn

deque(maxlen=10)
来源：http://uy.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://vy.huixinmuqiang.cn

defaultdict(list)
来源：http://qv.hnjuh.cn

[U15] Py：高精度计时
来源：http://fg.shxzskj.cn

t = time.perf_counter()
来源：http://og.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://fm.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ss.bjjhwx.cn

[U17] Py：初始化日志
来源：http://wm.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://hr.shxzskj.cn

[U18] Py：预编译正则
来源：http://ui.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://sm.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://pu.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vr.shxzukj.cn

[U20] Py：缓存函数结果
来源：http://aj.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://pg.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://pp.shtwfgs.cn

@contextlib.contextmanager
来源：http://si.szxytkj.cn

[U22] Py：矩阵转置
来源：http://fj.jctech888.com.cn

list(zip(*m))
来源：http://mv.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://yy.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rs.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://oo.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ic.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://tv.lnxyls.cn

csv.DictReader(f)
来源：http://tt.hahajie.cn

[U26] Py：并发下载
来源：http://mk.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dq.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ep.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://jq.9csxet.cn

[U28] Py：类型别名
来源：http://hv.szsharing.cn

UserId = int
来源：http://wd.hnjuh.cn

[U29] Py：属性校验
来源：http://zy.shxzukj.cn

@property 与 @x.setter 配合
来源：http://yu.nicolike.cn

[U30] Py：数据类
来源：http://wu.lnxyls.cn

@dataclass(slots=True)
来源：http://mv.gzmigu.cn

[U31] Py：单测
来源：http://dg.shtwfgs.cn

python -m pytest -q
来源：http://qs.panjiajie.cn

[U32] Py：代码格式化
来源：http://ee.nicolike.cn

ruff format . && ruff check --fix .
来源：http://as.bookmarksfly.cn

[U33] Py：打包发布
来源：http://vo.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://ug.shxzskj.cn

[U34] Py：判断编码
来源：http://ng.gzmigu.cn

chardet.detect(raw)
来源：http://uv.shtwfgs.cn

[U35] Py：发送邮件
来源：http://qd.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://di.hahajie.cn

[U36] Py：定时任务
来源：http://oi.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://os.521024.cn

[U37] Py：读写 Excel
来源：http://ep.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ke.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://xi.nszjky.cn

Path(__file__).resolve().parent
来源：http://qn.gzmigu.cn

[U39] Py：判断是否在交互环境
来源：http://fe.shtwfgs.cn

sys.stdout.isatty()
来源：http://mk.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ul.asd995.cn

print("err", file=sys.stderr)
来源：http://dn.gzmigu.cn

[U41] PHP：初始化 Composer 项目
来源：http://ds.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://po.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://vw.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ru.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://ua.shxzukj.cn

namespace App\Http;
来源：http://oh.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://py.wgjwhj.cn

declare(strict_types=1);
来源：http://ud.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://uk.lnxyls.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xv.yuexingan06.cn

[U46] PHP：可空类型
来源：http://go.haigaiapp.cn

?string $name = null
来源：http://ta.bjjhwx.cn

[U47] PHP：联合类型
来源：http://as.shtwfgs.cn

int|string $id
来源：http://yc.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://cp.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zg.jctech888.com.cn

[U49] PHP：只读属性
来源：http://mz.521024.cn

public readonly string $name
来源：http://qe.521024.cn

[U50] PHP：构造器属性提升
来源：http://cy.gzmigu.cn

public function __construct(private int $id) {}
来源：http://so.jianghongdianzi.cn

[U51] PHP：数组解构
来源：http://dn.huanxung.cn

[$a, $b] = $arr;
来源：http://ga.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://zn.asd995.cn

$double = fn($x) => $x * 2;
来源：http://rf.newstarts.cn

[U53] PHP：空合并运算符
来源：http://do.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://hz.hahajie.cn

[U54] PHP：空安全调用
来源：http://hb.hahajie.cn

$obj?->method()
来源：http://ry.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://lm.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ri.haigaiapp.cn

[U56] PHP：命名参数
来源：http://de.shxzskj.cn

f(a: 1, b: 2)
来源：http://vi.newstarts.cn

[U57] PHP：字符串插值
来源：http://li.bookmarksfly.cn

"值: {$a}"
来源：http://xh.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ng.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qe.lnxyls.cn

[U59] PHP：自定义排序
来源：http://hi.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kv.521024.cn

[U60] PHP：JSON 编解码
来源：http://gf.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://za.yuntaijiaju.cn

[U61] PHP：正则
来源：http://ro.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://px.haigaiapp.cn

[U62] PHP：日期对象
来源：http://zn.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gb.asd995.cn

[U63] PHP：文件读写
来源：http://sh.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ox.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://em.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://pm.nszjky.cn

[U65] PHP：会话
来源：http://ig.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gv.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://ow.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://or.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://st.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ri.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://nw.huanxung.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ws.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://em.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://op.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://bk.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bu.521024.cn

[U71] PHP：抛出异常
来源：http://vl.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://hp.nszjky.cn

[U72] PHP：写错误日志
来源：http://ml.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://yb.huixiangedu.cn

[U73] PHP：读取 ini 配置
来源：http://dx.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://ct.yuexingan06.cn

[U74] PHP：读取环境变量
来源：http://ou.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://ma.shtwfgs.cn


<!-- 参考信息 -->