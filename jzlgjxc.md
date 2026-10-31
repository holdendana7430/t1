代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://xo.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rt.szsharing.cn

[S48] C++：逐行读文件
来源：http://qf.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hi.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ij.bookmarksfly.cn

[S49] C++：写文件
来源：http://wo.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ax.panjiajie.cn

[S50] C++：格式化数字
来源：http://be.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://du.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://ua.haigaiapp.cn

static_cast<double>(a) / b
来源：http://xl.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://vc.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://kv.9csxet.cn

[S53] C++：移动语义
来源：http://gn.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://aa.hnjuh.cn

[S54] C++：异常处理
来源：http://et.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://av.gzmigu.cn

[S55] C++：结构化绑定
来源：http://do.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uv.bjjhwx.cn

[S56] C++：optional
来源：http://kt.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zo.yuexingan06.cn

[S57] C++：编译期常量
来源：http://zb.chemitech.net.cn

constexpr int N = 10;
来源：http://rr.hnjuh.cn

[S58] C++：命名空间
来源：http://jg.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://yh.bookmarksfly.cn

[S59] C++：静态断言
来源：http://qn.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nz.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://yp.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ca.hnjuh.cn

================================================================================
来源：http://ly.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tb.521024.cn

================================================================================
来源：http://xd.nszjky.cn

[T01] Kotlin：Hello World
来源：http://qj.colortex.cn

println("Hello")
来源：http://lu.gzmigu.cn

[T02] Kotlin：变量
来源：http://xa.nicolike.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lq.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://cw.yuntaijiaju.cn

"值: $b"
来源：http://fb.newstarts.cn

[T04] Kotlin：空安全
来源：http://fo.nicolike.cn

val n: String? = null;  n?.length
来源：http://fs.asd995.cn

[T05] Kotlin：when 表达式
来源：http://vy.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mk.asd995.cn

[T06] Kotlin：集合映射
来源：http://vv.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xg.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://fi.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cx.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://do.asd995.cn

data class User(val name: String, val age: Int)
来源：http://xp.chemitech.net.cn

[T09] Kotlin：扩展函数
来源：http://ba.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://ol.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://ku.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cu.bjjhwx.cn

[T11] Kotlin：协程
来源：http://ls.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qr.nicolike.cn

[T12] Kotlin：解构声明
来源：http://te.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ms.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://oz.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://xh.nicolike.cn

[T14] Kotlin：循环
来源：http://js.asd995.cn

for (i in 1..10) println(i)
来源：http://sv.chemitech.net.cn

[T15] Kotlin：接口
来源：http://ko.nszjky.cn

interface Shape { fun area(): Double }
来源：http://dt.muxihuayi.cn

[T16] Swift：Hello World
来源：http://cj.chemitech.net.cn

print("Hello")
来源：http://kw.hnjuh.cn

[T17] Swift：变量与常量
来源：http://vk.gzmigu.cn

var a = 1;  let b = 2
来源：http://ay.newstarts.cn

[T18] Swift：字符串插值
来源：http://ga.newstarts.cn

"值: \(b)"
来源：http://wx.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://kr.newstarts.cn

if let n = opt { print(n) }
来源：http://ht.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://sq.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ab.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://iz.muxihuayi.cn

for x in a { print(x) }
来源：http://ly.lnxyls.cn

[T22] Swift：字典
来源：http://tg.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gy.panjiajie.cn

[T23] Swift：函数
来源：http://es.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://th.gzmigu.cn

[T24] Swift：闭包
来源：http://up.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hb.newstarts.cn

[T25] Swift：结构体
来源：http://mx.szxytkj.cn

struct P { var x: Int }
来源：http://yw.wgjwhj.cn

[T26] Swift：类与重写
来源：http://tn.lnxyls.cn

class A: Base { override func f() {} }
来源：http://dw.nicolike.cn

[T27] Swift：错误处理
来源：http://xg.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://kw.lnxyls.cn

[T28] Swift：枚举
来源：http://pa.bjjhwx.cn

enum Color { case red, green }
来源：http://vs.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://ru.wgjwhj.cn

guard let x = opt else { return }
来源：http://rw.panjiajie.cn

[T30] Swift：协议
来源：http://gv.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://qe.panjiajie.cn

[T31] Lua：Hello World
来源：http://fg.jianghongdianzi.cn

print("Hello")
来源：http://ot.9csxet.cn

[T32] Lua：局部变量
来源：http://zz.jianghongdianzi.cn

local a = 1
来源：http://sz.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://iz.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hx.yuexingan06.cn

[T34] Lua：遍历表
来源：http://bp.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ze.panjiajie.cn

[T35] Lua：字典表
来源：http://hq.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://ag.huixiangedu.cn

[T36] Lua：函数
来源：http://ur.chemitech.net.cn

function add(a, b) return a + b end
来源：http://zm.colortex.cn

[T37] Lua：字符串拼接
来源：http://ez.shtwfgs.cn

"a" .. "b"
来源：http://tv.yuntaijiaju.cn

[T38] Lua：条件
来源：http://ou.lnxyls.cn

if x > 0 then print("正") end
来源：http://oz.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://by.shxzukj.cn

string.find(s, "%d+")
来源：http://ci.wgjwhj.cn

[T40] Lua：元表
来源：http://zo.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ut.jctech888.com.cn

[T41] Perl：Hello World
来源：http://ue.panjiajie.cn

print "Hello\n";
来源：http://io.jctech888.com.cn

[T42] Perl：变量类型
来源：http://in.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zl.521024.cn

[T43] Perl：字符串插值
来源：http://zt.szsharing.cn

"值: $a"
来源：http://zf.newstarts.cn

[T44] Perl：条件
来源：http://gt.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://yt.newstarts.cn

[T45] Perl：数组遍历
来源：http://tc.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://xm.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://uv.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fk.szxytkj.cn

[T47] Perl：正则捕获
来源：http://eg.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gw.gzmigu.cn

[T48] Perl：正则替换
来源：http://yy.521024.cn

$s =~ s/old/new/g;
来源：http://ny.shxzukj.cn

[T49] Perl：函数
来源：http://un.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bv.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://yn.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qd.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://kp.shxzukj.cn

[T51] Scala：Hello World
来源：http://rq.nicolike.cn

println("Hello")
来源：http://ep.huixinmuqiang.cn

[T52] Scala：变量
来源：http://bc.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://sj.nicolike.cn

[T53] Scala：字符串插值
来源：http://rk.szxytkj.cn

s"值: $b"
来源：http://id.521024.cn

[T54] Scala：集合映射
来源：http://hj.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://uv.huanxung.cn

[T55] Scala：集合过滤
来源：http://uq.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xk.asd995.cn

[T56] Scala：样例类
来源：http://ay.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://mn.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://fy.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pr.newstarts.cn

[T58] Scala：函数定义
来源：http://gq.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vo.521024.cn

[T59] Scala：循环
来源：http://dp.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://vg.nicolike.cn

[T60] Scala：折叠
来源：http://qn.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lm.yuexingan06.cn

================================================================================
来源：http://nf.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cw.huixiangedu.cn

================================================================================
来源：http://cv.colortex.cn

[U01] Py：创建虚拟环境
来源：http://lj.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pg.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://qw.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://du.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://jb.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uo.szxytkj.cn

[U04] Py：变量调试打印
来源：http://ez.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xw.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://uw.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://xe.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://lq.9csxet.cn

{**a, **b}
来源：http://ds.shxzskj.cn

[U07] Py：反转字典键值
来源：http://na.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://oy.huixinmuqiang.cn

[U08] Py：展平二维列表
来源：http://vp.huanxung.cn

[y for x in nested for y in x]
来源：http://mm.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://ec.shtwfgs.cn

max(d, key=d.get)
来源：http://cf.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://jk.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://in.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://av.wgjwhj.cn

(x * 2 for x in arr)
来源：http://nm.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pd.asd995.cn

Counter(arr).most_common(3)
来源：http://nw.panjiajie.cn

[U13] Py：固定长度队列
来源：http://hu.hahajie.cn

deque(maxlen=10)
来源：http://oi.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://uh.shxzskj.cn

defaultdict(list)
来源：http://dz.521024.cn

[U15] Py：高精度计时
来源：http://on.szxytkj.cn

t = time.perf_counter()
来源：http://xu.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://re.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oc.lnxyls.cn

[U17] Py：初始化日志
来源：http://dd.colortex.cn

logging.basicConfig(level=logging.INFO)
来源：http://tt.colortex.cn

[U18] Py：预编译正则
来源：http://pj.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://xe.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://xi.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cy.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://yk.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://hg.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ge.yuexingan06.cn

@contextlib.contextmanager
来源：http://zw.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://tk.wgjwhj.cn

list(zip(*m))
来源：http://mb.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://xw.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hf.huixiangedu.cn

[U24] Py：路径操作
来源：http://fe.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mb.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://hd.szsharing.cn

csv.DictReader(f)
来源：http://yj.bjjhwx.cn

[U26] Py：并发下载
来源：http://fg.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://su.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://sj.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://ji.asd995.cn

[U28] Py：类型别名
来源：http://zn.gzmigu.cn

UserId = int
来源：http://uo.hnjuh.cn

[U29] Py：属性校验
来源：http://bi.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://qz.huixiangedu.cn

[U30] Py：数据类
来源：http://ek.shxzskj.cn

@dataclass(slots=True)
来源：http://ju.hnjuh.cn

[U31] Py：单测
来源：http://wi.hahajie.cn

python -m pytest -q
来源：http://gp.newstarts.cn

[U32] Py：代码格式化
来源：http://nr.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://bk.asd995.cn

[U33] Py：打包发布
来源：http://wt.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://cd.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://gp.asd995.cn

chardet.detect(raw)
来源：http://ou.muxihuayi.cn

[U35] Py：发送邮件
来源：http://hk.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ki.hnjuh.cn

[U36] Py：定时任务
来源：http://rx.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://yw.nicolike.cn

[U37] Py：读写 Excel
来源：http://qn.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iu.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://gc.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://me.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://pz.chemitech.net.cn

sys.stdout.isatty()
来源：http://ku.bjjhwx.cn

[U40] Py：打印到标准错误
来源：http://jd.521024.cn

print("err", file=sys.stderr)
来源：http://wq.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://ys.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://np.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://xh.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zc.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://qh.chemitech.net.cn

namespace App\Http;
来源：http://hp.9csxet.cn

[U44] PHP：开启严格类型
来源：http://hu.hahajie.cn

declare(strict_types=1);
来源：http://rx.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://ls.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zg.asd995.cn

[U46] PHP：可空类型
来源：http://ll.nicolike.cn

?string $name = null
来源：http://dw.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://ip.yuntaijiaju.cn

int|string $id
来源：http://ad.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://sj.shtwfgs.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kg.nszjky.cn

[U49] PHP：只读属性
来源：http://qk.yuntaijiaju.cn

public readonly string $name
来源：http://xb.shxzskj.cn

[U50] PHP：构造器属性提升
来源：http://sa.huixinmuqiang.cn

public function __construct(private int $id) {}
来源：http://sp.szsharing.cn

[U51] PHP：数组解构
来源：http://yr.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://yr.panjiajie.cn

[U52] PHP：箭头函数
来源：http://fm.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://jy.shxzukj.cn

[U53] PHP：空合并运算符
来源：http://lr.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://xc.jctech888.com.cn

[U54] PHP：空安全调用
来源：http://os.muxihuayi.cn

$obj?->method()
来源：http://tt.hahajie.cn

[U55] PHP：match 表达式
来源：http://wl.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tz.huanxung.cn

[U56] PHP：命名参数
来源：http://dk.panjiajie.cn

f(a: 1, b: 2)
来源：http://oy.9csxet.cn

[U57] PHP：字符串插值
来源：http://pp.jctech888.com.cn

"值: {$a}"
来源：http://vb.nicolike.cn

[U58] PHP：数组三件套
来源：http://fc.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fy.newstarts.cn

[U59] PHP：自定义排序
来源：http://ca.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nx.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://zb.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://he.newstarts.cn

[U61] PHP：正则
来源：http://lj.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nx.9csxet.cn

[U62] PHP：日期对象
来源：http://ip.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vq.shtwfgs.cn

[U63] PHP：文件读写
来源：http://vn.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://es.9csxet.cn

[U64] PHP：目录遍历
来源：http://pq.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://nz.bjjhwx.cn

[U65] PHP：会话
来源：http://rz.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sl.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://uv.huixinmuqiang.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oq.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://rg.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gb.colortex.cn

[U68] PHP：PDO 连接
来源：http://qs.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tb.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://dp.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://py.bookmarksfly.cn

[U70] PHP：PDO 事务
来源：http://qx.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nf.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://zk.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://by.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://yn.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://yy.huixiangedu.cn


<!-- 参考信息 -->