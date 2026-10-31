代发 wailian999

while (std::getline(in, line)) { }
来源：http://yd.wgjwhj.cn

[S49] C++：写文件
来源：http://yx.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kj.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://ok.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vl.szsharing.cn

[S51] C++：显式类型转换
来源：http://fd.huanxung.cn

static_cast<double>(a) / b
来源：http://zy.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://on.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://fc.chemitech.net.cn

[S53] C++：移动语义
来源：http://qj.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://ku.newstarts.cn

[S54] C++：异常处理
来源：http://kh.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://di.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://lc.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oe.yuntaijiaju.cn

[S56] C++：optional
来源：http://fk.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://um.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://tb.colortex.cn

constexpr int N = 10;
来源：http://vk.szxytkj.cn

[S58] C++：命名空间
来源：http://xh.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://pj.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://xx.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dt.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://sh.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nw.yuexingan06.cn

================================================================================
来源：http://oh.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fu.huixinmuqiang.cn

================================================================================
来源：http://jn.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://lk.panjiajie.cn

println("Hello")
来源：http://yg.huanxung.cn

[T02] Kotlin：变量
来源：http://kp.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kq.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://ze.bookmarksfly.cn

"值: $b"
来源：http://zl.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://iy.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://ur.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://mr.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pv.szsharing.cn

[T06] Kotlin：集合映射
来源：http://vb.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gl.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://km.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ya.hnjuh.cn

[T08] Kotlin：数据类
来源：http://mq.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://aj.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://np.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://hg.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://vf.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tr.nicolike.cn

[T11] Kotlin：协程
来源：http://ui.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://em.colortex.cn

[T12] Kotlin：解构声明
来源：http://vh.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://si.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://rv.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://fv.bjjhwx.cn

[T14] Kotlin：循环
来源：http://lf.hnjuh.cn

for (i in 1..10) println(i)
来源：http://ym.huixiangedu.cn

[T15] Kotlin：接口
来源：http://gd.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://xf.szsharing.cn

[T16] Swift：Hello World
来源：http://le.yuexingan06.cn

print("Hello")
来源：http://ys.bjjhwx.cn

[T17] Swift：变量与常量
来源：http://xl.yuexingan06.cn

var a = 1;  let b = 2
来源：http://td.nszjky.cn

[T18] Swift：字符串插值
来源：http://ge.nszjky.cn

"值: \(b)"
来源：http://nf.shxzukj.cn

[T19] Swift：可选绑定
来源：http://zu.huixinmuqiang.cn

if let n = opt { print(n) }
来源：http://ow.bjjhwx.cn

[T20] Swift：数组操作
来源：http://vd.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gx.521024.cn

[T21] Swift：遍历
来源：http://ce.nicolike.cn

for x in a { print(x) }
来源：http://sx.jianghongdianzi.cn

[T22] Swift：字典
来源：http://on.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nk.521024.cn

[T23] Swift：函数
来源：http://lx.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mq.colortex.cn

[T24] Swift：闭包
来源：http://ue.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://if.hahajie.cn

[T25] Swift：结构体
来源：http://em.colortex.cn

struct P { var x: Int }
来源：http://bv.hahajie.cn

[T26] Swift：类与重写
来源：http://le.szxytkj.cn

class A: Base { override func f() {} }
来源：http://qx.yuexingan06.cn

[T27] Swift：错误处理
来源：http://uz.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://eg.colortex.cn

[T28] Swift：枚举
来源：http://pa.9csxet.cn

enum Color { case red, green }
来源：http://lv.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://ev.huixiangedu.cn

guard let x = opt else { return }
来源：http://wt.colortex.cn

[T30] Swift：协议
来源：http://ki.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://iv.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://mw.huixiangedu.cn

print("Hello")
来源：http://ap.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://ko.panjiajie.cn

local a = 1
来源：http://lu.9csxet.cn

[T33] Lua：表（数组）
来源：http://rx.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sx.wgjwhj.cn

[T34] Lua：遍历表
来源：http://ut.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nf.huixiangedu.cn

[T35] Lua：字典表
来源：http://jq.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://rb.hnjuh.cn

[T36] Lua：函数
来源：http://xn.hahajie.cn

function add(a, b) return a + b end
来源：http://sy.nszjky.cn

[T37] Lua：字符串拼接
来源：http://ju.521024.cn

"a" .. "b"
来源：http://sb.szsharing.cn

[T38] Lua：条件
来源：http://dc.huixiangedu.cn

if x > 0 then print("正") end
来源：http://ao.521024.cn

[T39] Lua：模式匹配
来源：http://er.hahajie.cn

string.find(s, "%d+")
来源：http://wo.muxihuayi.cn

[T40] Lua：元表
来源：http://qw.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://mi.shtwfgs.cn

[T41] Perl：Hello World
来源：http://qt.szxytkj.cn

print "Hello\n";
来源：http://xu.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://ur.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eo.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://kr.hahajie.cn

"值: $a"
来源：http://gc.newstarts.cn

[T44] Perl：条件
来源：http://ul.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://wr.panjiajie.cn

[T45] Perl：数组遍历
来源：http://hh.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://ua.szxytkj.cn

[T46] Perl：哈希操作
来源：http://lv.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fu.panjiajie.cn

[T47] Perl：正则捕获
来源：http://uz.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yh.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://wv.newstarts.cn

$s =~ s/old/new/g;
来源：http://gt.521024.cn

[T49] Perl：函数
来源：http://wh.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vh.szsharing.cn

[T50] Perl：逐行读文件
来源：http://wl.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rw.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://iu.gzmigu.cn

[T51] Scala：Hello World
来源：http://sg.haigaiapp.cn

println("Hello")
来源：http://lb.szxytkj.cn

[T52] Scala：变量
来源：http://zt.muxihuayi.cn

val a = 1;  var b = 2
来源：http://vt.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://lv.jctech888.com.cn

s"值: $b"
来源：http://sd.asd995.cn

[T54] Scala：集合映射
来源：http://pa.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://zb.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://qj.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vu.9csxet.cn

[T56] Scala：样例类
来源：http://ba.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://nv.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://uk.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sv.wgjwhj.cn

[T58] Scala：函数定义
来源：http://bj.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://do.gzmigu.cn

[T59] Scala：循环
来源：http://wf.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://wi.colortex.cn

[T60] Scala：折叠
来源：http://qh.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eq.shxzskj.cn

================================================================================
来源：http://jc.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pc.gzmigu.cn

================================================================================
来源：http://ug.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://nc.huixinmuqiang.cn

python -m venv .venv && source .venv/bin/activate
来源：http://er.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://oh.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://om.lnxyls.cn

[U03] Py：加载 .env 配置
来源：http://lp.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lc.hahajie.cn

[U04] Py：变量调试打印
来源：http://fw.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://om.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://es.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://lx.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://dk.bookmarksfly.cn

{**a, **b}
来源：http://fd.panjiajie.cn

[U07] Py：反转字典键值
来源：http://hp.hahajie.cn

{v: k for k, v in d.items()}
来源：http://du.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://au.521024.cn

[y for x in nested for y in x]
来源：http://fj.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://em.gzmigu.cn

max(d, key=d.get)
来源：http://ue.shxzukj.cn

[U10] Py：按值排序字典
来源：http://bq.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aq.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://ni.shxzskj.cn

(x * 2 for x in arr)
来源：http://wa.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sz.hnjuh.cn

Counter(arr).most_common(3)
来源：http://jg.hahajie.cn

[U13] Py：固定长度队列
来源：http://jp.shtwfgs.cn

deque(maxlen=10)
来源：http://uy.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://fo.shxzukj.cn

defaultdict(list)
来源：http://dd.gzmigu.cn

[U15] Py：高精度计时
来源：http://wf.9csxet.cn

t = time.perf_counter()
来源：http://kz.9csxet.cn

[U16] Py：命令行参数解析
来源：http://jo.newstarts.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ia.panjiajie.cn

[U17] Py：初始化日志
来源：http://kl.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://gx.shxzskj.cn

[U18] Py：预编译正则
来源：http://hz.nicolike.cn

pat = re.compile(r"\d+")
来源：http://wv.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://gg.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gn.szsharing.cn

[U20] Py：缓存函数结果
来源：http://op.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://zm.521024.cn

[U21] Py：自定义上下文管理器
来源：http://xz.wgjwhj.cn

@contextlib.contextmanager
来源：http://vw.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://ax.huixinmuqiang.cn

list(zip(*m))
来源：http://gu.muxihuayi.cn

[U23] Py：分块读取大文件
来源：http://sw.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ss.haigaiapp.cn

[U24] Py：路径操作
来源：http://lm.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kc.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://ok.nszjky.cn

csv.DictReader(f)
来源：http://og.haigaiapp.cn

[U26] Py：并发下载
来源：http://ys.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qp.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://yu.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://ud.shxzskj.cn

[U28] Py：类型别名
来源：http://kq.huixinmuqiang.cn

UserId = int
来源：http://ki.huixinmuqiang.cn

[U29] Py：属性校验
来源：http://bc.nszjky.cn

@property 与 @x.setter 配合
来源：http://gc.shxzukj.cn

[U30] Py：数据类
来源：http://eo.panjiajie.cn

@dataclass(slots=True)
来源：http://am.muxihuayi.cn

[U31] Py：单测
来源：http://sz.haigaiapp.cn

python -m pytest -q
来源：http://yu.gzmigu.cn

[U32] Py：代码格式化
来源：http://bq.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://mb.shxzskj.cn

[U33] Py：打包发布
来源：http://hr.chemitech.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://az.newstarts.cn

[U34] Py：判断编码
来源：http://jy.huanxung.cn

chardet.detect(raw)
来源：http://yl.shxzskj.cn

[U35] Py：发送邮件
来源：http://hg.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rr.shtwfgs.cn

[U36] Py：定时任务
来源：http://ri.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://no.hahajie.cn

[U37] Py：读写 Excel
来源：http://aw.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oo.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://sl.shxzskj.cn

Path(__file__).resolve().parent
来源：http://sl.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://er.muxihuayi.cn

sys.stdout.isatty()
来源：http://bx.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://hs.huanxung.cn

print("err", file=sys.stderr)
来源：http://pv.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ie.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pt.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://cs.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xw.bookmarksfly.cn

[U43] PHP：声明命名空间
来源：http://be.panjiajie.cn

namespace App\Http;
来源：http://jr.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://tg.huixiangedu.cn

declare(strict_types=1);
来源：http://kb.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://gu.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hi.chemitech.net.cn

[U46] PHP：可空类型
来源：http://zy.newstarts.cn

?string $name = null
来源：http://xl.haigaiapp.cn

[U47] PHP：联合类型
来源：http://kq.521024.cn

int|string $id
来源：http://vl.huanxung.cn

[U48] PHP：纯枚举
来源：http://tu.huixinmuqiang.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ue.haigaiapp.cn

[U49] PHP：只读属性
来源：http://ks.yuntaijiaju.cn

public readonly string $name
来源：http://hr.521024.cn

[U50] PHP：构造器属性提升
来源：http://kj.huixiangedu.cn

public function __construct(private int $id) {}
来源：http://gj.hahajie.cn

[U51] PHP：数组解构
来源：http://mh.nicolike.cn

[$a, $b] = $arr;
来源：http://tk.gzmigu.cn

[U52] PHP：箭头函数
来源：http://gg.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://wt.hahajie.cn

[U53] PHP：空合并运算符
来源：http://bv.gzmigu.cn

$v = $a ?? $b ?? "default";
来源：http://pp.colortex.cn

[U54] PHP：空安全调用
来源：http://se.huixinmuqiang.cn

$obj?->method()
来源：http://td.9csxet.cn

[U55] PHP：match 表达式
来源：http://an.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kr.hnjuh.cn

[U56] PHP：命名参数
来源：http://ks.huanxung.cn

f(a: 1, b: 2)
来源：http://hk.nicolike.cn

[U57] PHP：字符串插值
来源：http://im.521024.cn

"值: {$a}"
来源：http://ek.newstarts.cn

[U58] PHP：数组三件套
来源：http://zw.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zr.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://cj.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hr.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://pn.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xm.wgjwhj.cn

[U61] PHP：正则
来源：http://ro.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ce.yuexingan06.cn

[U62] PHP：日期对象
来源：http://gn.szxytkj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zf.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://nj.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fs.shxzukj.cn

[U64] PHP：目录遍历
来源：http://ca.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ps.hahajie.cn

[U65] PHP：会话
来源：http://em.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fl.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://un.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ha.szsharing.cn

[U67] PHP：处理文件上传
来源：http://wp.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xo.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://bk.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wj.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://tz.huixinmuqiang.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ck.9csxet.cn

[U70] PHP：PDO 事务
来源：http://ih.haigaiapp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xo.hnjuh.cn

[U71] PHP：抛出异常
来源：http://er.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://dn.gzmigu.cn

[U72] PHP：写错误日志
来源：http://nv.yuexingan06.cn

error_log("失败: " . $e->getMessage());
来源：http://ur.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://fp.colortex.cn

parse_ini_file("config.ini", true)
来源：http://jn.bookmarksfly.cn

[U74] PHP：读取环境变量
来源：http://hh.haigaiapp.cn

getenv("APP_ENV") ?: "production"
来源：http://ay.hahajie.cn


<!-- 参考信息 -->