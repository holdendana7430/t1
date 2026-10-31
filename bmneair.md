代发 wailian999

while (std::getline(in, line)) { }
来源：http://yl.hnjuh.cn

[S49] C++：写文件
来源：http://uh.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wu.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://hz.shtwfgs.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nk.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://xt.hahajie.cn

static_cast<double>(a) / b
来源：http://xv.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://lz.521024.cn

int size() const noexcept { return n_; }
来源：http://ik.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://gv.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://fl.gzmigu.cn

[S54] C++：异常处理
来源：http://eq.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sb.asd995.cn

[S55] C++：结构化绑定
来源：http://iu.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wf.newstarts.cn

[S56] C++：optional
来源：http://uu.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dn.gzmigu.cn

[S57] C++：编译期常量
来源：http://qu.muxihuayi.cn

constexpr int N = 10;
来源：http://wf.shtwfgs.cn

[S58] C++：命名空间
来源：http://zs.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://gx.jctech888.com.cn

[S59] C++：静态断言
来源：http://zb.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rw.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://be.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ye.asd995.cn

================================================================================
来源：http://so.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://da.yuntaijiaju.cn

================================================================================
来源：http://de.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://sc.521024.cn

println("Hello")
来源：http://ot.newstarts.cn

[T02] Kotlin：变量
来源：http://um.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ib.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://li.gzmigu.cn

"值: $b"
来源：http://oc.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://cf.huanxung.cn

val n: String? = null;  n?.length
来源：http://tc.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://th.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wm.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://nk.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xb.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://vf.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uf.lnxyls.cn

[T08] Kotlin：数据类
来源：http://zn.asd995.cn

data class User(val name: String, val age: Int)
来源：http://pe.nicolike.cn

[T09] Kotlin：扩展函数
来源：http://da.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://we.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://bn.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vi.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://wu.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wj.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://xz.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://lz.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://lq.521024.cn

val m = mapOf("a" to 1)
来源：http://hk.haigaiapp.cn

[T14] Kotlin：循环
来源：http://bt.panjiajie.cn

for (i in 1..10) println(i)
来源：http://sh.wgjwhj.cn

[T15] Kotlin：接口
来源：http://ph.colortex.cn

interface Shape { fun area(): Double }
来源：http://bt.shxzskj.cn

[T16] Swift：Hello World
来源：http://tm.hahajie.cn

print("Hello")
来源：http://ju.nszjky.cn

[T17] Swift：变量与常量
来源：http://be.asd995.cn

var a = 1;  let b = 2
来源：http://yj.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://qu.bjjhwx.cn

"值: \(b)"
来源：http://ci.newstarts.cn

[T19] Swift：可选绑定
来源：http://ci.521024.cn

if let n = opt { print(n) }
来源：http://zr.hnjuh.cn

[T20] Swift：数组操作
来源：http://wp.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gp.wgjwhj.cn

[T21] Swift：遍历
来源：http://si.yuntaijiaju.cn

for x in a { print(x) }
来源：http://zk.bjjhwx.cn

[T22] Swift：字典
来源：http://ei.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tz.szsharing.cn

[T23] Swift：函数
来源：http://bv.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cb.haigaiapp.cn

[T24] Swift：闭包
来源：http://qa.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eq.shtwfgs.cn

[T25] Swift：结构体
来源：http://ph.huixinmuqiang.cn

struct P { var x: Int }
来源：http://il.bjjhwx.cn

[T26] Swift：类与重写
来源：http://zv.gzmigu.cn

class A: Base { override func f() {} }
来源：http://cl.muxihuayi.cn

[T27] Swift：错误处理
来源：http://pl.newstarts.cn

do { try f() } catch { print(error) }
来源：http://ha.yuexingan06.cn

[T28] Swift：枚举
来源：http://qo.jctech888.com.cn

enum Color { case red, green }
来源：http://ui.nicolike.cn

[T29] Swift：guard 提前返回
来源：http://aq.shtwfgs.cn

guard let x = opt else { return }
来源：http://un.wgjwhj.cn

[T30] Swift：协议
来源：http://pc.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://me.521024.cn

[T31] Lua：Hello World
来源：http://no.szxytkj.cn

print("Hello")
来源：http://to.wgjwhj.cn

[T32] Lua：局部变量
来源：http://ng.colortex.cn

local a = 1
来源：http://dl.hahajie.cn

[T33] Lua：表（数组）
来源：http://te.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jg.hahajie.cn

[T34] Lua：遍历表
来源：http://gh.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://il.chemitech.net.cn

[T35] Lua：字典表
来源：http://bh.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://qq.chemitech.net.cn

[T36] Lua：函数
来源：http://zy.jctech888.com.cn

function add(a, b) return a + b end
来源：http://zc.nszjky.cn

[T37] Lua：字符串拼接
来源：http://rq.colortex.cn

"a" .. "b"
来源：http://my.huixinmuqiang.cn

[T38] Lua：条件
来源：http://kd.nicolike.cn

if x > 0 then print("正") end
来源：http://up.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://or.chemitech.net.cn

string.find(s, "%d+")
来源：http://vn.chemitech.net.cn

[T40] Lua：元表
来源：http://ai.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://yg.nszjky.cn

[T41] Perl：Hello World
来源：http://qn.bjjhwx.cn

print "Hello\n";
来源：http://rd.521024.cn

[T42] Perl：变量类型
来源：http://mr.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tk.newstarts.cn

[T43] Perl：字符串插值
来源：http://lf.asd995.cn

"值: $a"
来源：http://cw.chemitech.net.cn

[T44] Perl：条件
来源：http://wh.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://ce.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://yc.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://hk.newstarts.cn

[T46] Perl：哈希操作
来源：http://nd.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ej.colortex.cn

[T47] Perl：正则捕获
来源：http://qr.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ps.szsharing.cn

[T48] Perl：正则替换
来源：http://rl.panjiajie.cn

$s =~ s/old/new/g;
来源：http://do.bookmarksfly.cn

[T49] Perl：函数
来源：http://hq.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pm.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://gq.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ci.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://so.huixiangedu.cn

[T51] Scala：Hello World
来源：http://ly.nicolike.cn

println("Hello")
来源：http://bm.lnxyls.cn

[T52] Scala：变量
来源：http://nz.jctech888.com.cn

val a = 1;  var b = 2
来源：http://ci.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://zg.haigaiapp.cn

s"值: $b"
来源：http://mr.colortex.cn

[T54] Scala：集合映射
来源：http://lx.szsharing.cn

List(1, 2, 3).map(_ * 2)
来源：http://gu.lnxyls.cn

[T55] Scala：集合过滤
来源：http://ku.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://et.huanxung.cn

[T56] Scala：样例类
来源：http://ph.gzmigu.cn

case class User(name: String, age: Int)
来源：http://xf.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ks.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vo.muxihuayi.cn

[T58] Scala：函数定义
来源：http://ji.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bp.yuntaijiaju.cn

[T59] Scala：循环
来源：http://cm.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://mz.colortex.cn

[T60] Scala：折叠
来源：http://wn.szxytkj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zx.muxihuayi.cn

================================================================================
来源：http://jw.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ba.jctech888.com.cn

================================================================================
来源：http://pg.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://ni.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nb.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://mg.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tp.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://fj.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qy.9csxet.cn

[U04] Py：变量调试打印
来源：http://vh.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ua.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://iv.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://xr.asd995.cn

[U06] Py：合并两个字典
来源：http://sk.colortex.cn

{**a, **b}
来源：http://od.szxytkj.cn

[U07] Py：反转字典键值
来源：http://rg.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://uv.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://vk.szsharing.cn

[y for x in nested for y in x]
来源：http://wa.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://uc.521024.cn

max(d, key=d.get)
来源：http://ch.huanxung.cn

[U10] Py：按值排序字典
来源：http://oc.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fj.asd995.cn

[U11] Py：生成器表达式
来源：http://qo.chemitech.net.cn

(x * 2 for x in arr)
来源：http://fw.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lm.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://wv.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://dr.shtwfgs.cn

deque(maxlen=10)
来源：http://sz.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ww.huixinmuqiang.cn

defaultdict(list)
来源：http://rl.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://rk.shxzskj.cn

t = time.perf_counter()
来源：http://ex.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://cw.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pu.hahajie.cn

[U17] Py：初始化日志
来源：http://ts.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://aq.hnjuh.cn

[U18] Py：预编译正则
来源：http://oa.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://hk.colortex.cn

[U19] Py：正则替换带回调
来源：http://vo.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rp.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://qb.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://im.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://to.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ui.colortex.cn

[U22] Py：矩阵转置
来源：http://tm.yuntaijiaju.cn

list(zip(*m))
来源：http://uw.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://qh.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pk.asd995.cn

[U24] Py：路径操作
来源：http://pc.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hr.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://ml.hnjuh.cn

csv.DictReader(f)
来源：http://gs.lnxyls.cn

[U26] Py：并发下载
来源：http://qn.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ug.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://jf.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://mh.lnxyls.cn

[U28] Py：类型别名
来源：http://yo.bookmarksfly.cn

UserId = int
来源：http://wb.lnxyls.cn

[U29] Py：属性校验
来源：http://qg.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://ae.lnxyls.cn

[U30] Py：数据类
来源：http://kc.shxzskj.cn

@dataclass(slots=True)
来源：http://uu.jianghongdianzi.cn

[U31] Py：单测
来源：http://pk.shxzskj.cn

python -m pytest -q
来源：http://pm.shxzukj.cn

[U32] Py：代码格式化
来源：http://bu.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://fh.shtwfgs.cn

[U33] Py：打包发布
来源：http://zu.9csxet.cn

python -m build  （依赖 pyproject.toml）
来源：http://vh.hnjuh.cn

[U34] Py：判断编码
来源：http://hx.shxzskj.cn

chardet.detect(raw)
来源：http://xe.newstarts.cn

[U35] Py：发送邮件
来源：http://qj.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hg.szsharing.cn

[U36] Py：定时任务
来源：http://rn.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://in.panjiajie.cn

[U37] Py：读写 Excel
来源：http://ev.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gx.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://oq.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://az.nicolike.cn

[U39] Py：判断是否在交互环境
来源：http://ry.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://vu.521024.cn

[U40] Py：打印到标准错误
来源：http://dc.shxzskj.cn

print("err", file=sys.stderr)
来源：http://or.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://yi.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cg.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://lb.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eq.szxytkj.cn

[U43] PHP：声明命名空间
来源：http://rm.newstarts.cn

namespace App\Http;
来源：http://de.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://oa.haigaiapp.cn

declare(strict_types=1);
来源：http://uv.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://lb.muxihuayi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hi.lnxyls.cn

[U46] PHP：可空类型
来源：http://vu.shxzukj.cn

?string $name = null
来源：http://cs.chemitech.net.cn

[U47] PHP：联合类型
来源：http://sq.colortex.cn

int|string $id
来源：http://gx.asd995.cn

[U48] PHP：纯枚举
来源：http://ln.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ce.hahajie.cn

[U49] PHP：只读属性
来源：http://tc.colortex.cn

public readonly string $name
来源：http://ct.colortex.cn

[U50] PHP：构造器属性提升
来源：http://ap.lnxyls.cn

public function __construct(private int $id) {}
来源：http://au.szxytkj.cn

[U51] PHP：数组解构
来源：http://zw.szxytkj.cn

[$a, $b] = $arr;
来源：http://oi.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://mm.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://rb.asd995.cn

[U53] PHP：空合并运算符
来源：http://jr.521024.cn

$v = $a ?? $b ?? "default";
来源：http://jz.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://rj.asd995.cn

$obj?->method()
来源：http://wy.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://lx.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pa.yuntaijiaju.cn

[U56] PHP：命名参数
来源：http://gn.shtwfgs.cn

f(a: 1, b: 2)
来源：http://ul.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://fl.panjiajie.cn

"值: {$a}"
来源：http://wo.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://yp.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://on.newstarts.cn

[U59] PHP：自定义排序
来源：http://il.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mf.colortex.cn

[U60] PHP：JSON 编解码
来源：http://ia.shxzskj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tt.nszjky.cn

[U61] PHP：正则
来源：http://kk.lnxyls.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ng.huixiangedu.cn

[U62] PHP：日期对象
来源：http://no.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gc.szxytkj.cn

[U63] PHP：文件读写
来源：http://kk.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iq.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://dj.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://rx.nszjky.cn

[U65] PHP：会话
来源：http://rs.haigaiapp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://am.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://es.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yx.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://ln.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aq.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://xk.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yt.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://cj.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vo.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://se.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vt.shxzskj.cn

[U71] PHP：抛出异常
来源：http://if.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://si.bookmarksfly.cn

[U72] PHP：写错误日志
来源：http://tb.521024.cn

error_log("失败: " . $e->getMessage());
来源：http://ik.asd995.cn

[U73] PHP：读取 ini 配置
来源：http://zz.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://vw.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ic.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://wv.szsharing.cn


<!-- 参考信息 -->