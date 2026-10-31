代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jg.lnxyls.cn

[S51] C++：显式类型转换
来源：http://yk.nszjky.cn

static_cast<double>(a) / b
来源：http://tt.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://sk.newstarts.cn

int size() const noexcept { return n_; }
来源：http://lr.huixiangedu.cn

[S53] C++：移动语义
来源：http://xz.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://bh.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://gt.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ke.521024.cn

[S55] C++：结构化绑定
来源：http://sw.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ea.huixiangedu.cn

[S56] C++：optional
来源：http://gw.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bj.gzmigu.cn

[S57] C++：编译期常量
来源：http://uh.wgjwhj.cn

constexpr int N = 10;
来源：http://nk.asd995.cn

[S58] C++：命名空间
来源：http://ml.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://cp.gzmigu.cn

[S59] C++：静态断言
来源：http://qg.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qf.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://sh.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mh.hahajie.cn

================================================================================
来源：http://is.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kp.gzmigu.cn

================================================================================
来源：http://zm.9csxet.cn

[T01] Kotlin：Hello World
来源：http://dc.huanxung.cn

println("Hello")
来源：http://yp.gzmigu.cn

[T02] Kotlin：变量
来源：http://qn.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ga.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://bn.9csxet.cn

"值: $b"
来源：http://ys.newstarts.cn

[T04] Kotlin：空安全
来源：http://su.hahajie.cn

val n: String? = null;  n?.length
来源：http://bu.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://hd.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ym.huanxung.cn

[T06] Kotlin：集合映射
来源：http://yp.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qj.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://xh.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sr.szsharing.cn

[T08] Kotlin：数据类
来源：http://xe.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://ce.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://gs.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://ll.nszjky.cn

[T10] Kotlin：默认参数
来源：http://xx.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pd.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://wx.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qq.nszjky.cn

[T12] Kotlin：解构声明
来源：http://jd.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://ul.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://ln.9csxet.cn

val m = mapOf("a" to 1)
来源：http://vl.521024.cn

[T14] Kotlin：循环
来源：http://pn.szsharing.cn

for (i in 1..10) println(i)
来源：http://um.yuexingan06.cn

[T15] Kotlin：接口
来源：http://ez.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://wt.shtwfgs.cn

[T16] Swift：Hello World
来源：http://nq.lnxyls.cn

print("Hello")
来源：http://vk.nszjky.cn

[T17] Swift：变量与常量
来源：http://gi.bjjhwx.cn

var a = 1;  let b = 2
来源：http://ef.hahajie.cn

[T18] Swift：字符串插值
来源：http://gh.nszjky.cn

"值: \(b)"
来源：http://rl.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://wu.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://nr.newstarts.cn

[T20] Swift：数组操作
来源：http://zm.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vj.9csxet.cn

[T21] Swift：遍历
来源：http://jz.hahajie.cn

for x in a { print(x) }
来源：http://wh.szxytkj.cn

[T22] Swift：字典
来源：http://ay.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hj.yuntaijiaju.cn

[T23] Swift：函数
来源：http://zq.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://go.haigaiapp.cn

[T24] Swift：闭包
来源：http://oo.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://en.newstarts.cn

[T25] Swift：结构体
来源：http://ex.asd995.cn

struct P { var x: Int }
来源：http://rq.huixiangedu.cn

[T26] Swift：类与重写
来源：http://ck.gzmigu.cn

class A: Base { override func f() {} }
来源：http://ck.haigaiapp.cn

[T27] Swift：错误处理
来源：http://yh.521024.cn

do { try f() } catch { print(error) }
来源：http://df.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://cp.bookmarksfly.cn

enum Color { case red, green }
来源：http://oj.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://rc.shxzukj.cn

guard let x = opt else { return }
来源：http://ec.huixiangedu.cn

[T30] Swift：协议
来源：http://ya.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://vk.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ct.521024.cn

print("Hello")
来源：http://nj.huanxung.cn

[T32] Lua：局部变量
来源：http://ft.bjjhwx.cn

local a = 1
来源：http://vy.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://hs.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ef.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://mf.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bf.521024.cn

[T35] Lua：字典表
来源：http://iv.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://my.9csxet.cn

[T36] Lua：函数
来源：http://rx.newstarts.cn

function add(a, b) return a + b end
来源：http://dr.colortex.cn

[T37] Lua：字符串拼接
来源：http://de.shxzukj.cn

"a" .. "b"
来源：http://am.bjjhwx.cn

[T38] Lua：条件
来源：http://yo.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://jb.panjiajie.cn

[T39] Lua：模式匹配
来源：http://lk.newstarts.cn

string.find(s, "%d+")
来源：http://ol.muxihuayi.cn

[T40] Lua：元表
来源：http://wi.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://qg.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://zb.huanxung.cn

print "Hello\n";
来源：http://yt.shxzskj.cn

[T42] Perl：变量类型
来源：http://ys.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jr.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://sj.panjiajie.cn

"值: $a"
来源：http://tc.bjjhwx.cn

[T44] Perl：条件
来源：http://rv.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://wp.9csxet.cn

[T45] Perl：数组遍历
来源：http://wi.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://hy.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://kr.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qa.hahajie.cn

[T47] Perl：正则捕获
来源：http://fz.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sw.521024.cn

[T48] Perl：正则替换
来源：http://wp.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://yc.szxytkj.cn

[T49] Perl：函数
来源：http://kb.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://li.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ka.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qu.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://pk.shxzukj.cn

[T51] Scala：Hello World
来源：http://xm.lnxyls.cn

println("Hello")
来源：http://dm.lnxyls.cn

[T52] Scala：变量
来源：http://ut.huanxung.cn

val a = 1;  var b = 2
来源：http://hb.nszjky.cn

[T53] Scala：字符串插值
来源：http://ao.521024.cn

s"值: $b"
来源：http://lf.nicolike.cn

[T54] Scala：集合映射
来源：http://go.521024.cn

List(1, 2, 3).map(_ * 2)
来源：http://nq.lnxyls.cn

[T55] Scala：集合过滤
来源：http://zc.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nh.muxihuayi.cn

[T56] Scala：样例类
来源：http://xd.lnxyls.cn

case class User(name: String, age: Int)
来源：http://fq.szxytkj.cn

[T57] Scala：模式匹配
来源：http://fn.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rq.jctech888.com.cn

[T58] Scala：函数定义
来源：http://mg.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sy.szsharing.cn

[T59] Scala：循环
来源：http://cp.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://vv.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://xc.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yp.jianghongdianzi.cn

================================================================================
来源：http://oo.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yl.huixinmuqiang.cn

================================================================================
来源：http://pj.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://jt.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pr.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://ng.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ph.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://zd.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bp.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://il.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cm.huanxung.cn

[U05] Py：列表去重且保序
来源：http://fw.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://gz.huanxung.cn

[U06] Py：合并两个字典
来源：http://bj.colortex.cn

{**a, **b}
来源：http://bj.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://uu.colortex.cn

{v: k for k, v in d.items()}
来源：http://sw.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://wo.hahajie.cn

[y for x in nested for y in x]
来源：http://yg.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://er.shxzskj.cn

max(d, key=d.get)
来源：http://ur.nszjky.cn

[U10] Py：按值排序字典
来源：http://nv.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gg.szxytkj.cn

[U11] Py：生成器表达式
来源：http://vl.szsharing.cn

(x * 2 for x in arr)
来源：http://wq.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xw.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://uq.hnjuh.cn

[U13] Py：固定长度队列
来源：http://gt.asd995.cn

deque(maxlen=10)
来源：http://jc.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://kg.yuntaijiaju.cn

defaultdict(list)
来源：http://tv.szsharing.cn

[U15] Py：高精度计时
来源：http://bv.chemitech.net.cn

t = time.perf_counter()
来源：http://jl.colortex.cn

[U16] Py：命令行参数解析
来源：http://gf.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qp.panjiajie.cn

[U17] Py：初始化日志
来源：http://nw.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://th.szxytkj.cn

[U18] Py：预编译正则
来源：http://nk.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://id.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://cb.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zm.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://hh.wgjwhj.cn

@functools.lru_cache(maxsize=None)
来源：http://dv.szsharing.cn

[U21] Py：自定义上下文管理器
来源：http://mv.bjjhwx.cn

@contextlib.contextmanager
来源：http://cz.shxzukj.cn

[U22] Py：矩阵转置
来源：http://zm.jianghongdianzi.cn

list(zip(*m))
来源：http://gk.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://yp.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ej.shxzukj.cn

[U24] Py：路径操作
来源：http://ja.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://av.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://wz.shxzskj.cn

csv.DictReader(f)
来源：http://ny.huixinmuqiang.cn

[U26] Py：并发下载
来源：http://nf.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jy.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://sm.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://pe.wgjwhj.cn

[U28] Py：类型别名
来源：http://ik.521024.cn

UserId = int
来源：http://ej.hnjuh.cn

[U29] Py：属性校验
来源：http://li.gzmigu.cn

@property 与 @x.setter 配合
来源：http://bn.hnjuh.cn

[U30] Py：数据类
来源：http://cm.newstarts.cn

@dataclass(slots=True)
来源：http://am.bookmarksfly.cn

[U31] Py：单测
来源：http://mx.chemitech.net.cn

python -m pytest -q
来源：http://gu.521024.cn

[U32] Py：代码格式化
来源：http://sy.hahajie.cn

ruff format . && ruff check --fix .
来源：http://rq.newstarts.cn

[U33] Py：打包发布
来源：http://hh.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://ms.gzmigu.cn

[U34] Py：判断编码
来源：http://pw.szxytkj.cn

chardet.detect(raw)
来源：http://bx.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://rd.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://et.bjjhwx.cn

[U36] Py：定时任务
来源：http://pl.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://bk.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://wj.lnxyls.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lw.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://ao.panjiajie.cn

Path(__file__).resolve().parent
来源：http://jj.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://bm.jctech888.com.cn

sys.stdout.isatty()
来源：http://dl.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://bt.colortex.cn

print("err", file=sys.stderr)
来源：http://hd.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://co.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ez.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://vj.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xl.szsharing.cn

[U43] PHP：声明命名空间
来源：http://hb.9csxet.cn

namespace App\Http;
来源：http://ww.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ei.bjjhwx.cn

declare(strict_types=1);
来源：http://mg.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://mv.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qp.szxytkj.cn

[U46] PHP：可空类型
来源：http://ss.newstarts.cn

?string $name = null
来源：http://xo.jianghongdianzi.cn

[U47] PHP：联合类型
来源：http://ke.hahajie.cn

int|string $id
来源：http://ce.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://tq.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rm.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://rq.521024.cn

public readonly string $name
来源：http://ho.yuntaijiaju.cn

[U50] PHP：构造器属性提升
来源：http://tc.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://ia.bjjhwx.cn

[U51] PHP：数组解构
来源：http://vo.nicolike.cn

[$a, $b] = $arr;
来源：http://qp.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://yp.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://fo.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://xg.huixinmuqiang.cn

$v = $a ?? $b ?? "default";
来源：http://ob.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://gw.yuntaijiaju.cn

$obj?->method()
来源：http://wp.szxytkj.cn

[U55] PHP：match 表达式
来源：http://ah.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://go.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://qw.nszjky.cn

f(a: 1, b: 2)
来源：http://jm.huanxung.cn

[U57] PHP：字符串插值
来源：http://hq.haigaiapp.cn

"值: {$a}"
来源：http://pb.newstarts.cn

[U58] PHP：数组三件套
来源：http://go.shxzskj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://by.gzmigu.cn

[U59] PHP：自定义排序
来源：http://ed.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xt.hnjuh.cn

[U60] PHP：JSON 编解码
来源：http://rp.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qi.nszjky.cn

[U61] PHP：正则
来源：http://lj.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wa.newstarts.cn

[U62] PHP：日期对象
来源：http://wf.yuexingan06.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sb.huanxung.cn

[U63] PHP：文件读写
来源：http://lo.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ak.shxzukj.cn

[U64] PHP：目录遍历
来源：http://sm.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://bl.colortex.cn

[U65] PHP：会话
来源：http://ny.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://oq.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://fw.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wi.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://dm.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xj.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://pq.hahajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jc.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://mr.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uq.huanxung.cn

[U70] PHP：PDO 事务
来源：http://td.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://az.lnxyls.cn

[U71] PHP：抛出异常
来源：http://fm.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://cm.hnjuh.cn

[U72] PHP：写错误日志
来源：http://rf.szxytkj.cn

error_log("失败: " . $e->getMessage());
来源：http://wm.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://ls.shtwfgs.cn

parse_ini_file("config.ini", true)
来源：http://rm.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://zl.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://mc.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://wq.szxytkj.cn

composer require psr/container
来源：http://zn.shtwfgs.cn

[U76] PHP：简单路由
来源：http://xk.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gw.hnjuh.cn


<!-- 参考信息 -->