代发 wailian999

while (std::getline(in, line)) { }
来源：http://xw.nszjky.cn

[S49] C++：写文件
来源：http://cx.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ga.nicolike.cn

[S50] C++：格式化数字
来源：http://ln.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xi.9csxet.cn

[S51] C++：显式类型转换
来源：http://ui.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://nt.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://lx.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://us.newstarts.cn

[S53] C++：移动语义
来源：http://qp.asd995.cn

std::vector<int> w = std::move(v);
来源：http://fe.gzmigu.cn

[S54] C++：异常处理
来源：http://hz.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dk.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://tr.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ib.shxzukj.cn

[S56] C++：optional
来源：http://yy.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sq.gzmigu.cn

[S57] C++：编译期常量
来源：http://ip.jctech888.com.cn

constexpr int N = 10;
来源：http://ly.chemitech.net.cn

[S58] C++：命名空间
来源：http://oq.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://ns.gzmigu.cn

[S59] C++：静态断言
来源：http://tt.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://td.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://rj.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mn.chemitech.net.cn

================================================================================
来源：http://ux.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fi.9csxet.cn

================================================================================
来源：http://oi.9csxet.cn

[T01] Kotlin：Hello World
来源：http://zj.newstarts.cn

println("Hello")
来源：http://gi.huanxung.cn

[T02] Kotlin：变量
来源：http://ot.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mm.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://af.hahajie.cn

"值: $b"
来源：http://oi.hahajie.cn

[T04] Kotlin：空安全
来源：http://hs.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://tn.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://jb.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sv.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://bx.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gi.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://pe.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tt.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://wh.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://hj.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://ej.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://hu.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://dx.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uv.nszjky.cn

[T11] Kotlin：协程
来源：http://rj.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://da.9csxet.cn

[T12] Kotlin：解构声明
来源：http://of.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://qb.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://rh.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://iu.szxytkj.cn

[T14] Kotlin：循环
来源：http://ub.nicolike.cn

for (i in 1..10) println(i)
来源：http://nj.yuexingan06.cn

[T15] Kotlin：接口
来源：http://rv.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://iz.shxzukj.cn

[T16] Swift：Hello World
来源：http://tf.huixinmuqiang.cn

print("Hello")
来源：http://nt.521024.cn

[T17] Swift：变量与常量
来源：http://vg.huixiangedu.cn

var a = 1;  let b = 2
来源：http://uw.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://te.muxihuayi.cn

"值: \(b)"
来源：http://nn.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ye.shxzukj.cn

if let n = opt { print(n) }
来源：http://xu.521024.cn

[T20] Swift：数组操作
来源：http://wu.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iu.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://pc.jctech888.com.cn

for x in a { print(x) }
来源：http://ib.haigaiapp.cn

[T22] Swift：字典
来源：http://ro.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gj.szxytkj.cn

[T23] Swift：函数
来源：http://hm.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uz.shtwfgs.cn

[T24] Swift：闭包
来源：http://la.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cy.yuexingan06.cn

[T25] Swift：结构体
来源：http://hp.shtwfgs.cn

struct P { var x: Int }
来源：http://qf.shxzukj.cn

[T26] Swift：类与重写
来源：http://qk.lnxyls.cn

class A: Base { override func f() {} }
来源：http://hp.chemitech.net.cn

[T27] Swift：错误处理
来源：http://us.nicolike.cn

do { try f() } catch { print(error) }
来源：http://jx.huixiangedu.cn

[T28] Swift：枚举
来源：http://kl.muxihuayi.cn

enum Color { case red, green }
来源：http://wp.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://zn.yuexingan06.cn

guard let x = opt else { return }
来源：http://yu.haigaiapp.cn

[T30] Swift：协议
来源：http://ms.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://qg.colortex.cn

[T31] Lua：Hello World
来源：http://om.gzmigu.cn

print("Hello")
来源：http://no.lnxyls.cn

[T32] Lua：局部变量
来源：http://jt.chemitech.net.cn

local a = 1
来源：http://xe.hahajie.cn

[T33] Lua：表（数组）
来源：http://yj.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hj.huanxung.cn

[T34] Lua：遍历表
来源：http://wq.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://md.szsharing.cn

[T35] Lua：字典表
来源：http://xa.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://af.gzmigu.cn

[T36] Lua：函数
来源：http://bb.chemitech.net.cn

function add(a, b) return a + b end
来源：http://gp.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://xk.chemitech.net.cn

"a" .. "b"
来源：http://ew.521024.cn

[T38] Lua：条件
来源：http://ic.szxytkj.cn

if x > 0 then print("正") end
来源：http://qu.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://uk.panjiajie.cn

string.find(s, "%d+")
来源：http://vl.lnxyls.cn

[T40] Lua：元表
来源：http://es.huanxung.cn

setmetatable({}, { __index = base })
来源：http://dt.szxytkj.cn

[T41] Perl：Hello World
来源：http://kz.nszjky.cn

print "Hello\n";
来源：http://il.shxzskj.cn

[T42] Perl：变量类型
来源：http://ot.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nd.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://bk.gzmigu.cn

"值: $a"
来源：http://dc.huixiangedu.cn

[T44] Perl：条件
来源：http://la.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://zi.colortex.cn

[T45] Perl：数组遍历
来源：http://cp.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://rj.521024.cn

[T46] Perl：哈希操作
来源：http://xa.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sp.newstarts.cn

[T47] Perl：正则捕获
来源：http://jj.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lk.huanxung.cn

[T48] Perl：正则替换
来源：http://sf.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://va.szsharing.cn

[T49] Perl：函数
来源：http://rl.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wt.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://zy.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yp.gzmigu.cn

while (my $line = <$fh>) { print $line; }
来源：http://gu.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ab.huixiangedu.cn

println("Hello")
来源：http://px.hahajie.cn

[T52] Scala：变量
来源：http://el.lnxyls.cn

val a = 1;  var b = 2
来源：http://fw.newstarts.cn

[T53] Scala：字符串插值
来源：http://wg.shxzukj.cn

s"值: $b"
来源：http://wh.panjiajie.cn

[T54] Scala：集合映射
来源：http://eq.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://ow.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://ut.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ud.szsharing.cn

[T56] Scala：样例类
来源：http://yv.szsharing.cn

case class User(name: String, age: Int)
来源：http://vp.szxytkj.cn

[T57] Scala：模式匹配
来源：http://mw.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xr.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://zg.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mh.bjjhwx.cn

[T59] Scala：循环
来源：http://kv.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://xc.shxzukj.cn

[T60] Scala：折叠
来源：http://jc.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zb.newstarts.cn

================================================================================
来源：http://pn.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jc.shxzskj.cn

================================================================================
来源：http://tb.521024.cn

[U01] Py：创建虚拟环境
来源：http://ba.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sr.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://pf.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iz.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://cj.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nq.huanxung.cn

[U04] Py：变量调试打印
来源：http://ys.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://db.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://kq.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://df.bjjhwx.cn

[U06] Py：合并两个字典
来源：http://br.chemitech.net.cn

{**a, **b}
来源：http://zs.521024.cn

[U07] Py：反转字典键值
来源：http://bf.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://vn.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://yt.newstarts.cn

[y for x in nested for y in x]
来源：http://fd.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://vy.gzmigu.cn

max(d, key=d.get)
来源：http://vg.nicolike.cn

[U10] Py：按值排序字典
来源：http://dc.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cf.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://fi.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://oy.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wk.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://jz.nicolike.cn

[U13] Py：固定长度队列
来源：http://ps.bjjhwx.cn

deque(maxlen=10)
来源：http://no.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://cf.gzmigu.cn

defaultdict(list)
来源：http://xu.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://tm.huixinmuqiang.cn

t = time.perf_counter()
来源：http://zn.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://st.wgjwhj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ne.gzmigu.cn

[U17] Py：初始化日志
来源：http://qg.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://uw.huanxung.cn

[U18] Py：预编译正则
来源：http://kg.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://jf.521024.cn

[U19] Py：正则替换带回调
来源：http://fi.huanxung.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bo.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://wa.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://qo.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://yl.bjjhwx.cn

@contextlib.contextmanager
来源：http://nj.colortex.cn

[U22] Py：矩阵转置
来源：http://gk.haigaiapp.cn

list(zip(*m))
来源：http://pm.nicolike.cn

[U23] Py：分块读取大文件
来源：http://og.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rb.wgjwhj.cn

[U24] Py：路径操作
来源：http://zc.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bl.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ox.szsharing.cn

csv.DictReader(f)
来源：http://cf.wgjwhj.cn

[U26] Py：并发下载
来源：http://ss.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hr.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://jv.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://eq.shtwfgs.cn

[U28] Py：类型别名
来源：http://ee.colortex.cn

UserId = int
来源：http://vz.bookmarksfly.cn

[U29] Py：属性校验
来源：http://vi.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://wv.huanxung.cn

[U30] Py：数据类
来源：http://gy.bookmarksfly.cn

@dataclass(slots=True)
来源：http://kb.panjiajie.cn

[U31] Py：单测
来源：http://af.hnjuh.cn

python -m pytest -q
来源：http://rw.wgjwhj.cn

[U32] Py：代码格式化
来源：http://qu.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://dt.lnxyls.cn

[U33] Py：打包发布
来源：http://hu.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://rv.shtwfgs.cn

[U34] Py：判断编码
来源：http://ua.haigaiapp.cn

chardet.detect(raw)
来源：http://tt.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://vp.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gz.521024.cn

[U36] Py：定时任务
来源：http://wz.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://bs.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://fw.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fe.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://nb.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://cm.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://pb.colortex.cn

sys.stdout.isatty()
来源：http://jh.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://dx.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://rb.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://dy.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://eu.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://sy.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tz.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://mh.jianghongdianzi.cn

namespace App\Http;
来源：http://uk.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://ch.yuexingan06.cn

declare(strict_types=1);
来源：http://ri.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://gp.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ro.shxzukj.cn

[U46] PHP：可空类型
来源：http://oc.lnxyls.cn

?string $name = null
来源：http://jb.asd995.cn

[U47] PHP：联合类型
来源：http://vz.szsharing.cn

int|string $id
来源：http://wr.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://sy.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qn.gzmigu.cn

[U49] PHP：只读属性
来源：http://qw.shxzskj.cn

public readonly string $name
来源：http://lh.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://iu.nicolike.cn

public function __construct(private int $id) {}
来源：http://ak.bjjhwx.cn

[U51] PHP：数组解构
来源：http://mh.newstarts.cn

[$a, $b] = $arr;
来源：http://pz.asd995.cn

[U52] PHP：箭头函数
来源：http://vy.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://cr.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://cc.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://jk.szsharing.cn

[U54] PHP：空安全调用
来源：http://jq.chemitech.net.cn

$obj?->method()
来源：http://ch.lnxyls.cn

[U55] PHP：match 表达式
来源：http://qr.huanxung.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yf.nicolike.cn

[U56] PHP：命名参数
来源：http://rr.wgjwhj.cn

f(a: 1, b: 2)
来源：http://sk.nszjky.cn

[U57] PHP：字符串插值
来源：http://lc.nszjky.cn

"值: {$a}"
来源：http://ui.asd995.cn

[U58] PHP：数组三件套
来源：http://lq.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kq.nicolike.cn

[U59] PHP：自定义排序
来源：http://zh.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hi.huixiangedu.cn

[U60] PHP：JSON 编解码
来源：http://yz.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tr.szsharing.cn

[U61] PHP：正则
来源：http://vc.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xg.shxzukj.cn

[U62] PHP：日期对象
来源：http://xa.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nl.haigaiapp.cn

[U63] PHP：文件读写
来源：http://sl.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zj.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://gd.szxytkj.cn

glob("dir/*.php");  scandir("dir");
来源：http://ui.huixinmuqiang.cn

[U65] PHP：会话
来源：http://wx.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gi.muxihuayi.cn

[U66] PHP：设置 Cookie
来源：http://aj.jianghongdianzi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rc.nszjky.cn

[U67] PHP：处理文件上传
来源：http://jg.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zi.jianghongdianzi.cn

[U68] PHP：PDO 连接
来源：http://lq.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eq.gzmigu.cn

[U69] PHP：PDO 预处理
来源：http://yu.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ir.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://nc.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qu.huanxung.cn

[U71] PHP：抛出异常
来源：http://xu.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://eb.nszjky.cn

[U72] PHP：写错误日志
来源：http://vs.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://gs.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://np.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://wr.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://mv.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://jy.nszjky.cn


<!-- 参考信息 -->