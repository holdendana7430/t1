代发 wailian999

while (std::getline(in, line)) { }
来源：http://jo.asd995.cn

[S49] C++：写文件
来源：http://ls.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nq.chemitech.net.cn

[S50] C++：格式化数字
来源：http://ft.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xw.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://wr.newstarts.cn

static_cast<double>(a) / b
来源：http://ri.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://ul.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://tw.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ul.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://bp.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://uj.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yz.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://py.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oh.nszjky.cn

[S56] C++：optional
来源：http://sh.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qv.shxzskj.cn

[S57] C++：编译期常量
来源：http://ul.gzmigu.cn

constexpr int N = 10;
来源：http://oi.muxihuayi.cn

[S58] C++：命名空间
来源：http://bf.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://gx.nszjky.cn

[S59] C++：静态断言
来源：http://wq.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rr.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://kc.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lf.asd995.cn

================================================================================
来源：http://oq.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hw.bookmarksfly.cn

================================================================================
来源：http://lk.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ue.huixinmuqiang.cn

println("Hello")
来源：http://mo.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://xr.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ls.521024.cn

[T03] Kotlin：字符串模板
来源：http://bi.yuexingan06.cn

"值: $b"
来源：http://xt.newstarts.cn

[T04] Kotlin：空安全
来源：http://xo.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://to.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://cy.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rh.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://xl.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kn.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://xc.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yc.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://xk.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://ic.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://ym.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://we.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://dp.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lt.shxzskj.cn

[T11] Kotlin：协程
来源：http://kz.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lw.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://gc.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://am.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://vi.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://ut.hnjuh.cn

[T14] Kotlin：循环
来源：http://kh.gzmigu.cn

for (i in 1..10) println(i)
来源：http://xr.asd995.cn

[T15] Kotlin：接口
来源：http://kt.hnjuh.cn

interface Shape { fun area(): Double }
来源：http://oi.9csxet.cn

[T16] Swift：Hello World
来源：http://iv.yuntaijiaju.cn

print("Hello")
来源：http://tl.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://ls.muxihuayi.cn

var a = 1;  let b = 2
来源：http://ea.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://rz.chemitech.net.cn

"值: \(b)"
来源：http://zy.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://pp.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://ul.chemitech.net.cn

[T20] Swift：数组操作
来源：http://sn.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ve.lnxyls.cn

[T21] Swift：遍历
来源：http://lv.shxzskj.cn

for x in a { print(x) }
来源：http://zs.jctech888.com.cn

[T22] Swift：字典
来源：http://vj.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://em.bookmarksfly.cn

[T23] Swift：函数
来源：http://wc.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ly.muxihuayi.cn

[T24] Swift：闭包
来源：http://ru.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fp.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://aq.muxihuayi.cn

struct P { var x: Int }
来源：http://mn.huixinmuqiang.cn

[T26] Swift：类与重写
来源：http://qo.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://uo.yuexingan06.cn

[T27] Swift：错误处理
来源：http://yi.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://td.yuexingan06.cn

[T28] Swift：枚举
来源：http://yt.nicolike.cn

enum Color { case red, green }
来源：http://aa.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://zy.9csxet.cn

guard let x = opt else { return }
来源：http://hf.newstarts.cn

[T30] Swift：协议
来源：http://rt.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://ok.9csxet.cn

[T31] Lua：Hello World
来源：http://tw.shxzskj.cn

print("Hello")
来源：http://qa.huanxung.cn

[T32] Lua：局部变量
来源：http://st.asd995.cn

local a = 1
来源：http://uo.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://lj.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hw.asd995.cn

[T34] Lua：遍历表
来源：http://ch.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lw.szsharing.cn

[T35] Lua：字典表
来源：http://ok.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://yf.haigaiapp.cn

[T36] Lua：函数
来源：http://oi.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://ec.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://rs.wgjwhj.cn

"a" .. "b"
来源：http://qk.newstarts.cn

[T38] Lua：条件
来源：http://gr.huanxung.cn

if x > 0 then print("正") end
来源：http://gx.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://nm.haigaiapp.cn

string.find(s, "%d+")
来源：http://fz.haigaiapp.cn

[T40] Lua：元表
来源：http://lk.szsharing.cn

setmetatable({}, { __index = base })
来源：http://jt.nszjky.cn

[T41] Perl：Hello World
来源：http://pz.chemitech.net.cn

print "Hello\n";
来源：http://pl.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://na.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ht.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://wu.9csxet.cn

"值: $a"
来源：http://un.asd995.cn

[T44] Perl：条件
来源：http://jj.521024.cn

if ($a > 0) { print "正"; }
来源：http://ax.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://xo.gzmigu.cn

for my $x (@arr) { print $x; }
来源：http://au.521024.cn

[T46] Perl：哈希操作
来源：http://us.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mt.nszjky.cn

[T47] Perl：正则捕获
来源：http://uq.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ai.panjiajie.cn

[T48] Perl：正则替换
来源：http://up.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://uy.panjiajie.cn

[T49] Perl：函数
来源：http://yg.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ef.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://qv.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ry.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://si.hahajie.cn

[T51] Scala：Hello World
来源：http://pl.chemitech.net.cn

println("Hello")
来源：http://zs.yuexingan06.cn

[T52] Scala：变量
来源：http://tc.jctech888.com.cn

val a = 1;  var b = 2
来源：http://at.colortex.cn

[T53] Scala：字符串插值
来源：http://xm.nszjky.cn

s"值: $b"
来源：http://id.nszjky.cn

[T54] Scala：集合映射
来源：http://qf.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://cw.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://sp.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://du.muxihuayi.cn

[T56] Scala：样例类
来源：http://hm.huanxung.cn

case class User(name: String, age: Int)
来源：http://da.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://kd.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wh.yuexingan06.cn

[T58] Scala：函数定义
来源：http://ta.jctech888.com.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kf.gzmigu.cn

[T59] Scala：循环
来源：http://sj.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://xa.yuexingan06.cn

[T60] Scala：折叠
来源：http://ip.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zq.jianghongdianzi.cn

================================================================================
来源：http://zr.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xb.chemitech.net.cn

================================================================================
来源：http://tg.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://qu.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fu.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://hp.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lo.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://ze.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gf.hahajie.cn

[U04] Py：变量调试打印
来源：http://bd.shxzukj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sh.nszjky.cn

[U05] Py：列表去重且保序
来源：http://jj.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://bt.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://ub.gzmigu.cn

{**a, **b}
来源：http://zt.hnjuh.cn

[U07] Py：反转字典键值
来源：http://hb.shxzukj.cn

{v: k for k, v in d.items()}
来源：http://qi.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://ph.huixiangedu.cn

[y for x in nested for y in x]
来源：http://hc.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://fh.shtwfgs.cn

max(d, key=d.get)
来源：http://us.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://hi.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gu.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://tr.chemitech.net.cn

(x * 2 for x in arr)
来源：http://lj.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bf.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://cx.asd995.cn

[U13] Py：固定长度队列
来源：http://po.lnxyls.cn

deque(maxlen=10)
来源：http://xn.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://zr.nicolike.cn

defaultdict(list)
来源：http://ff.lnxyls.cn

[U15] Py：高精度计时
来源：http://ez.gzmigu.cn

t = time.perf_counter()
来源：http://tw.521024.cn

[U16] Py：命令行参数解析
来源：http://vx.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cp.9csxet.cn

[U17] Py：初始化日志
来源：http://sb.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://ik.asd995.cn

[U18] Py：预编译正则
来源：http://cs.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://kd.huixiangedu.cn

[U19] Py：正则替换带回调
来源：http://hk.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ga.hahajie.cn

[U20] Py：缓存函数结果
来源：http://kn.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://lg.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://xz.bookmarksfly.cn

@contextlib.contextmanager
来源：http://se.lnxyls.cn

[U22] Py：矩阵转置
来源：http://gr.bookmarksfly.cn

list(zip(*m))
来源：http://vw.newstarts.cn

[U23] Py：分块读取大文件
来源：http://rx.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fk.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://sr.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ps.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://uv.huanxung.cn

csv.DictReader(f)
来源：http://zi.jctech888.com.cn

[U26] Py：并发下载
来源：http://qv.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://av.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://wi.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://ur.asd995.cn

[U28] Py：类型别名
来源：http://lj.huanxung.cn

UserId = int
来源：http://mv.huanxung.cn

[U29] Py：属性校验
来源：http://pf.521024.cn

@property 与 @x.setter 配合
来源：http://ma.shxzukj.cn

[U30] Py：数据类
来源：http://bo.muxihuayi.cn

@dataclass(slots=True)
来源：http://fs.bjjhwx.cn

[U31] Py：单测
来源：http://im.panjiajie.cn

python -m pytest -q
来源：http://fs.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://an.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ym.nszjky.cn

[U33] Py：打包发布
来源：http://dd.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://rh.muxihuayi.cn

[U34] Py：判断编码
来源：http://lg.muxihuayi.cn

chardet.detect(raw)
来源：http://sr.hahajie.cn

[U35] Py：发送邮件
来源：http://xi.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ft.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://gv.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://na.lnxyls.cn

[U37] Py：读写 Excel
来源：http://in.szxytkj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bk.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://ke.huanxung.cn

Path(__file__).resolve().parent
来源：http://ay.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://qk.szxytkj.cn

sys.stdout.isatty()
来源：http://lp.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://kt.szxytkj.cn

print("err", file=sys.stderr)
来源：http://lv.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://tq.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jg.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://yq.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://up.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://ik.asd995.cn

namespace App\Http;
来源：http://zy.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://yt.szxytkj.cn

declare(strict_types=1);
来源：http://eo.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://gk.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qs.colortex.cn

[U46] PHP：可空类型
来源：http://qp.huixinmuqiang.cn

?string $name = null
来源：http://eq.chemitech.net.cn

[U47] PHP：联合类型
来源：http://td.lnxyls.cn

int|string $id
来源：http://hm.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://az.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vp.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://ra.yuexingan06.cn

public readonly string $name
来源：http://wf.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://nz.newstarts.cn

public function __construct(private int $id) {}
来源：http://xb.521024.cn

[U51] PHP：数组解构
来源：http://bh.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://rs.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://lr.521024.cn

$double = fn($x) => $x * 2;
来源：http://ze.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://ma.shxzukj.cn

$v = $a ?? $b ?? "default";
来源：http://pl.shxzukj.cn

[U54] PHP：空安全调用
来源：http://hy.szxytkj.cn

$obj?->method()
来源：http://cp.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://pe.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qa.asd995.cn

[U56] PHP：命名参数
来源：http://es.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://ox.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://ao.hnjuh.cn

"值: {$a}"
来源：http://fx.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://gs.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jx.gzmigu.cn

[U59] PHP：自定义排序
来源：http://pj.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yj.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://mc.asd995.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://og.lnxyls.cn

[U61] PHP：正则
来源：http://cw.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ja.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://if.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rv.huixiangedu.cn

[U63] PHP：文件读写
来源：http://ei.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rd.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://tk.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://vv.bookmarksfly.cn

[U65] PHP：会话
来源：http://gm.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dc.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://ye.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rl.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://xs.colortex.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://il.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://jb.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nn.nicolike.cn

[U69] PHP：PDO 预处理
来源：http://sa.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://di.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://cy.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hh.gzmigu.cn

[U71] PHP：抛出异常
来源：http://gp.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://ni.newstarts.cn

[U72] PHP：写错误日志
来源：http://ly.panjiajie.cn

error_log("失败: " . $e->getMessage());
来源：http://sh.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://ze.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://ff.hahajie.cn

[U74] PHP：读取环境变量
来源：http://zz.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://st.bookmarksfly.cn


<!-- 参考信息 -->