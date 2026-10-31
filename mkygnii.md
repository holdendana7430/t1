代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gs.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://xw.asd995.cn

static_cast<double>(a) / b
来源：http://nb.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://md.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://sb.hahajie.cn

[S53] C++：移动语义
来源：http://ms.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://rr.bookmarksfly.cn

[S54] C++：异常处理
来源：http://wv.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bu.lnxyls.cn

[S55] C++：结构化绑定
来源：http://hm.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://st.bookmarksfly.cn

[S56] C++：optional
来源：http://nl.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vo.szsharing.cn

[S57] C++：编译期常量
来源：http://qk.hahajie.cn

constexpr int N = 10;
来源：http://tl.szsharing.cn

[S58] C++：命名空间
来源：http://be.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://tk.lnxyls.cn

[S59] C++：静态断言
来源：http://gj.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pu.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://xp.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ez.bjjhwx.cn

================================================================================
来源：http://vk.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jx.huanxung.cn

================================================================================
来源：http://wh.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://kg.chemitech.net.cn

println("Hello")
来源：http://vg.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://gt.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tp.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://jo.chemitech.net.cn

"值: $b"
来源：http://xy.szsharing.cn

[T04] Kotlin：空安全
来源：http://ek.9csxet.cn

val n: String? = null;  n?.length
来源：http://xm.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://zh.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lh.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://pq.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xo.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://kn.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ut.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://hn.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://hi.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://yf.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://bs.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://nw.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zp.panjiajie.cn

[T11] Kotlin：协程
来源：http://ks.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://un.nicolike.cn

[T12] Kotlin：解构声明
来源：http://dk.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://zc.9csxet.cn

[T13] Kotlin：只读 Map
来源：http://yc.asd995.cn

val m = mapOf("a" to 1)
来源：http://sg.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://iy.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://zv.huixiangedu.cn

[T15] Kotlin：接口
来源：http://ae.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://fj.nicolike.cn

[T16] Swift：Hello World
来源：http://ri.jctech888.com.cn

print("Hello")
来源：http://ln.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://cb.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://sn.newstarts.cn

[T18] Swift：字符串插值
来源：http://si.shxzskj.cn

"值: \(b)"
来源：http://ds.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://en.newstarts.cn

if let n = opt { print(n) }
来源：http://bi.jctech888.com.cn

[T20] Swift：数组操作
来源：http://zu.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nc.szsharing.cn

[T21] Swift：遍历
来源：http://nu.hahajie.cn

for x in a { print(x) }
来源：http://aa.nicolike.cn

[T22] Swift：字典
来源：http://ua.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oc.yuexingan06.cn

[T23] Swift：函数
来源：http://ga.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wk.gzmigu.cn

[T24] Swift：闭包
来源：http://ye.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ac.newstarts.cn

[T25] Swift：结构体
来源：http://wl.haigaiapp.cn

struct P { var x: Int }
来源：http://py.haigaiapp.cn

[T26] Swift：类与重写
来源：http://fn.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://na.szsharing.cn

[T27] Swift：错误处理
来源：http://ez.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://lo.nszjky.cn

[T28] Swift：枚举
来源：http://ig.huixinmuqiang.cn

enum Color { case red, green }
来源：http://zl.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://yg.hnjuh.cn

guard let x = opt else { return }
来源：http://ag.lnxyls.cn

[T30] Swift：协议
来源：http://jy.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://nj.shtwfgs.cn

[T31] Lua：Hello World
来源：http://rp.hahajie.cn

print("Hello")
来源：http://gm.colortex.cn

[T32] Lua：局部变量
来源：http://zf.newstarts.cn

local a = 1
来源：http://tn.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://kn.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nl.lnxyls.cn

[T34] Lua：遍历表
来源：http://lu.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zy.9csxet.cn

[T35] Lua：字典表
来源：http://yn.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://cz.huixiangedu.cn

[T36] Lua：函数
来源：http://vu.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://dq.nicolike.cn

[T37] Lua：字符串拼接
来源：http://wr.nicolike.cn

"a" .. "b"
来源：http://gn.muxihuayi.cn

[T38] Lua：条件
来源：http://ig.lnxyls.cn

if x > 0 then print("正") end
来源：http://fa.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://ik.szxytkj.cn

string.find(s, "%d+")
来源：http://ql.asd995.cn

[T40] Lua：元表
来源：http://vm.hahajie.cn

setmetatable({}, { __index = base })
来源：http://zc.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://ex.bookmarksfly.cn

print "Hello\n";
来源：http://dh.yuexingan06.cn

[T42] Perl：变量类型
来源：http://dq.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wf.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://mc.muxihuayi.cn

"值: $a"
来源：http://gr.panjiajie.cn

[T44] Perl：条件
来源：http://yh.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://xy.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://ga.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://bz.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://le.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cc.521024.cn

[T47] Perl：正则捕获
来源：http://me.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://do.9csxet.cn

[T48] Perl：正则替换
来源：http://br.szxytkj.cn

$s =~ s/old/new/g;
来源：http://mh.hahajie.cn

[T49] Perl：函数
来源：http://wx.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jz.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://bb.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nt.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://eq.newstarts.cn

[T51] Scala：Hello World
来源：http://hu.hnjuh.cn

println("Hello")
来源：http://al.szsharing.cn

[T52] Scala：变量
来源：http://bf.shxzskj.cn

val a = 1;  var b = 2
来源：http://xo.szsharing.cn

[T53] Scala：字符串插值
来源：http://pm.shtwfgs.cn

s"值: $b"
来源：http://op.muxihuayi.cn

[T54] Scala：集合映射
来源：http://su.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://gm.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://mq.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jw.jctech888.com.cn

[T56] Scala：样例类
来源：http://nj.nszjky.cn

case class User(name: String, age: Int)
来源：http://ri.asd995.cn

[T57] Scala：模式匹配
来源：http://tq.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vf.huixiangedu.cn

[T58] Scala：函数定义
来源：http://wx.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lc.muxihuayi.cn

[T59] Scala：循环
来源：http://tw.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://nx.gzmigu.cn

[T60] Scala：折叠
来源：http://fs.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mv.colortex.cn

================================================================================
来源：http://uk.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://je.gzmigu.cn

================================================================================
来源：http://qy.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://au.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uw.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://iq.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mx.yuexingan06.cn

[U03] Py：加载 .env 配置
来源：http://rp.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hb.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://zh.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kn.szsharing.cn

[U05] Py：列表去重且保序
来源：http://wf.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://cs.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://lh.hnjuh.cn

{**a, **b}
来源：http://ce.shxzukj.cn

[U07] Py：反转字典键值
来源：http://ow.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://qz.szsharing.cn

[U08] Py：展平二维列表
来源：http://ui.newstarts.cn

[y for x in nested for y in x]
来源：http://vl.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://yi.szxytkj.cn

max(d, key=d.get)
来源：http://ow.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://ej.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dj.newstarts.cn

[U11] Py：生成器表达式
来源：http://if.hahajie.cn

(x * 2 for x in arr)
来源：http://mb.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gg.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ta.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://mg.szsharing.cn

deque(maxlen=10)
来源：http://xj.huanxung.cn

[U14] Py：分组收集到列表
来源：http://tb.gzmigu.cn

defaultdict(list)
来源：http://ct.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://qt.nicolike.cn

t = time.perf_counter()
来源：http://ed.lnxyls.cn

[U16] Py：命令行参数解析
来源：http://ij.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ex.haigaiapp.cn

[U17] Py：初始化日志
来源：http://nt.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://dr.shxzukj.cn

[U18] Py：预编译正则
来源：http://hg.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ou.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://sn.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pt.shtwfgs.cn

[U20] Py：缓存函数结果
来源：http://dy.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://rk.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://yu.newstarts.cn

@contextlib.contextmanager
来源：http://id.gzmigu.cn

[U22] Py：矩阵转置
来源：http://kp.jctech888.com.cn

list(zip(*m))
来源：http://ej.asd995.cn

[U23] Py：分块读取大文件
来源：http://ww.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sm.szxytkj.cn

[U24] Py：路径操作
来源：http://wn.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ie.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://jn.9csxet.cn

csv.DictReader(f)
来源：http://dn.nicolike.cn

[U26] Py：并发下载
来源：http://mm.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ji.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://mo.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://qs.huanxung.cn

[U28] Py：类型别名
来源：http://ld.shxzskj.cn

UserId = int
来源：http://op.huixiangedu.cn

[U29] Py：属性校验
来源：http://pw.yuexingan06.cn

@property 与 @x.setter 配合
来源：http://uj.huixinmuqiang.cn

[U30] Py：数据类
来源：http://bk.lnxyls.cn

@dataclass(slots=True)
来源：http://dq.wgjwhj.cn

[U31] Py：单测
来源：http://jr.huanxung.cn

python -m pytest -q
来源：http://zr.wgjwhj.cn

[U32] Py：代码格式化
来源：http://at.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://eb.bjjhwx.cn

[U33] Py：打包发布
来源：http://eh.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://qf.bjjhwx.cn

[U34] Py：判断编码
来源：http://ke.nicolike.cn

chardet.detect(raw)
来源：http://oj.shtwfgs.cn

[U35] Py：发送邮件
来源：http://ye.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xs.huixiangedu.cn

[U36] Py：定时任务
来源：http://dw.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://im.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://ln.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lh.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://nu.newstarts.cn

Path(__file__).resolve().parent
来源：http://uh.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://ri.haigaiapp.cn

sys.stdout.isatty()
来源：http://sl.521024.cn

[U40] Py：打印到标准错误
来源：http://bi.chemitech.net.cn

print("err", file=sys.stderr)
来源：http://yy.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://do.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vb.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://lb.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://av.colortex.cn

[U43] PHP：声明命名空间
来源：http://zq.521024.cn

namespace App\Http;
来源：http://xh.yuexingan06.cn

[U44] PHP：开启严格类型
来源：http://xv.yuexingan06.cn

declare(strict_types=1);
来源：http://eq.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://sd.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://co.yuexingan06.cn

[U46] PHP：可空类型
来源：http://is.szsharing.cn

?string $name = null
来源：http://bk.nicolike.cn

[U47] PHP：联合类型
来源：http://ed.bookmarksfly.cn

int|string $id
来源：http://xj.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://dc.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rk.hnjuh.cn

[U49] PHP：只读属性
来源：http://kg.shxzukj.cn

public readonly string $name
来源：http://ge.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ak.9csxet.cn

public function __construct(private int $id) {}
来源：http://cj.huixinmuqiang.cn

[U51] PHP：数组解构
来源：http://dw.hnjuh.cn

[$a, $b] = $arr;
来源：http://mp.jctech888.com.cn

[U52] PHP：箭头函数
来源：http://hl.9csxet.cn

$double = fn($x) => $x * 2;
来源：http://sv.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://li.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://qn.bjjhwx.cn

[U54] PHP：空安全调用
来源：http://ur.huixiangedu.cn

$obj?->method()
来源：http://mq.szxytkj.cn

[U55] PHP：match 表达式
来源：http://fy.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ld.bjjhwx.cn

[U56] PHP：命名参数
来源：http://sm.hahajie.cn

f(a: 1, b: 2)
来源：http://nq.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://nz.yuexingan06.cn

"值: {$a}"
来源：http://qh.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://sh.gzmigu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://id.asd995.cn

[U59] PHP：自定义排序
来源：http://nh.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fw.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://vh.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hu.hnjuh.cn

[U61] PHP：正则
来源：http://yf.hnjuh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yh.szxytkj.cn

[U62] PHP：日期对象
来源：http://jg.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nj.9csxet.cn

[U63] PHP：文件读写
来源：http://im.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://un.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://jd.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://as.gzmigu.cn

[U65] PHP：会话
来源：http://ej.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zx.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://lj.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ih.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://hb.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ka.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://kq.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ga.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://dv.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wl.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://qv.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://re.szxytkj.cn

[U71] PHP：抛出异常
来源：http://rg.521024.cn

throw new RuntimeException("失败", 500);
来源：http://na.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://up.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://uz.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://jf.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://ue.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://qu.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://jk.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://kd.shxzskj.cn

composer require psr/container
来源：http://ba.szxytkj.cn

[U76] PHP：简单路由
来源：http://ya.wgjwhj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qf.nicolike.cn


<!-- 参考信息 -->