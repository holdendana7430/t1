代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://vd.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ch.huanxung.cn

[S48] C++：逐行读文件
来源：http://sm.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tz.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://rs.hnjuh.cn

[S49] C++：写文件
来源：http://ao.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mf.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://fn.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kl.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://wj.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://kq.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://hk.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://hq.wgjwhj.cn

[S53] C++：移动语义
来源：http://hr.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://al.hahajie.cn

[S54] C++：异常处理
来源：http://op.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dd.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://wj.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xb.szxytkj.cn

[S56] C++：optional
来源：http://vq.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ui.nicolike.cn

[S57] C++：编译期常量
来源：http://tw.shtwfgs.cn

constexpr int N = 10;
来源：http://hk.shxzukj.cn

[S58] C++：命名空间
来源：http://re.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://mr.muxihuayi.cn

[S59] C++：静态断言
来源：http://fr.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ri.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://pn.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://if.szxytkj.cn

================================================================================
来源：http://bz.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zt.yuntaijiaju.cn

================================================================================
来源：http://ps.asd995.cn

[T01] Kotlin：Hello World
来源：http://sm.asd995.cn

println("Hello")
来源：http://fb.gzmigu.cn

[T02] Kotlin：变量
来源：http://pt.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pp.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://if.newstarts.cn

"值: $b"
来源：http://at.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://gh.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://id.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://xv.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zd.nszjky.cn

[T06] Kotlin：集合映射
来源：http://bn.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nf.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://up.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tl.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://nz.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://zl.colortex.cn

[T09] Kotlin：扩展函数
来源：http://py.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://qf.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://yf.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pq.shxzskj.cn

[T11] Kotlin：协程
来源：http://vz.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dn.hahajie.cn

[T12] Kotlin：解构声明
来源：http://ic.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://hy.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://bg.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://xi.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://yc.shxzskj.cn

for (i in 1..10) println(i)
来源：http://gr.haigaiapp.cn

[T15] Kotlin：接口
来源：http://bu.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://tv.nszjky.cn

[T16] Swift：Hello World
来源：http://kf.huixinmuqiang.cn

print("Hello")
来源：http://br.shxzukj.cn

[T17] Swift：变量与常量
来源：http://hw.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://ce.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://pt.hahajie.cn

"值: \(b)"
来源：http://dy.panjiajie.cn

[T19] Swift：可选绑定
来源：http://so.yuntaijiaju.cn

if let n = opt { print(n) }
来源：http://zd.muxihuayi.cn

[T20] Swift：数组操作
来源：http://we.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ak.huixiangedu.cn

[T21] Swift：遍历
来源：http://bu.jianghongdianzi.cn

for x in a { print(x) }
来源：http://xz.hnjuh.cn

[T22] Swift：字典
来源：http://ix.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gn.muxihuayi.cn

[T23] Swift：函数
来源：http://py.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dm.newstarts.cn

[T24] Swift：闭包
来源：http://vf.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cx.newstarts.cn

[T25] Swift：结构体
来源：http://tr.szsharing.cn

struct P { var x: Int }
来源：http://lj.521024.cn

[T26] Swift：类与重写
来源：http://bb.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://gw.szsharing.cn

[T27] Swift：错误处理
来源：http://gv.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://kr.asd995.cn

[T28] Swift：枚举
来源：http://ri.shxzukj.cn

enum Color { case red, green }
来源：http://ie.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://ae.huanxung.cn

guard let x = opt else { return }
来源：http://ci.9csxet.cn

[T30] Swift：协议
来源：http://ko.521024.cn

protocol Shape { func area() -> Double }
来源：http://mp.gzmigu.cn

[T31] Lua：Hello World
来源：http://uo.szsharing.cn

print("Hello")
来源：http://og.nicolike.cn

[T32] Lua：局部变量
来源：http://hw.lnxyls.cn

local a = 1
来源：http://ec.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://by.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mq.colortex.cn

[T34] Lua：遍历表
来源：http://du.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ye.muxihuayi.cn

[T35] Lua：字典表
来源：http://qb.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://pf.jctech888.com.cn

[T36] Lua：函数
来源：http://pb.hahajie.cn

function add(a, b) return a + b end
来源：http://sf.bjjhwx.cn

[T37] Lua：字符串拼接
来源：http://dn.newstarts.cn

"a" .. "b"
来源：http://cd.hahajie.cn

[T38] Lua：条件
来源：http://pc.szsharing.cn

if x > 0 then print("正") end
来源：http://nl.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://tz.hahajie.cn

string.find(s, "%d+")
来源：http://sg.521024.cn

[T40] Lua：元表
来源：http://yg.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://wf.asd995.cn

[T41] Perl：Hello World
来源：http://hd.hahajie.cn

print "Hello\n";
来源：http://rq.colortex.cn

[T42] Perl：变量类型
来源：http://fn.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ow.9csxet.cn

[T43] Perl：字符串插值
来源：http://nj.nszjky.cn

"值: $a"
来源：http://sg.bookmarksfly.cn

[T44] Perl：条件
来源：http://om.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://la.shxzskj.cn

[T45] Perl：数组遍历
来源：http://mc.521024.cn

for my $x (@arr) { print $x; }
来源：http://rb.yuntaijiaju.cn

[T46] Perl：哈希操作
来源：http://xg.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ny.shxzskj.cn

[T47] Perl：正则捕获
来源：http://ll.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uc.hahajie.cn

[T48] Perl：正则替换
来源：http://ub.panjiajie.cn

$s =~ s/old/new/g;
来源：http://if.9csxet.cn

[T49] Perl：函数
来源：http://yy.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ix.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://ql.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zl.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://lh.jctech888.com.cn

[T51] Scala：Hello World
来源：http://jx.yuexingan06.cn

println("Hello")
来源：http://dj.nicolike.cn

[T52] Scala：变量
来源：http://kx.9csxet.cn

val a = 1;  var b = 2
来源：http://tc.nszjky.cn

[T53] Scala：字符串插值
来源：http://la.yuexingan06.cn

s"值: $b"
来源：http://zd.521024.cn

[T54] Scala：集合映射
来源：http://du.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://ys.szxytkj.cn

[T55] Scala：集合过滤
来源：http://cb.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sa.newstarts.cn

[T56] Scala：样例类
来源：http://wg.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://nb.shxzukj.cn

[T57] Scala：模式匹配
来源：http://iw.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jb.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://ic.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ry.chemitech.net.cn

[T59] Scala：循环
来源：http://hv.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://vp.nszjky.cn

[T60] Scala：折叠
来源：http://ep.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vt.yuntaijiaju.cn

================================================================================
来源：http://wn.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hp.huanxung.cn

================================================================================
来源：http://ae.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://el.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kz.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://ya.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lr.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://yq.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fn.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://jv.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rj.huanxung.cn

[U05] Py：列表去重且保序
来源：http://gt.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://uk.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://cf.haigaiapp.cn

{**a, **b}
来源：http://eo.jianghongdianzi.cn

[U07] Py：反转字典键值
来源：http://rc.colortex.cn

{v: k for k, v in d.items()}
来源：http://zn.szsharing.cn

[U08] Py：展平二维列表
来源：http://dh.muxihuayi.cn

[y for x in nested for y in x]
来源：http://sj.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://wl.shtwfgs.cn

max(d, key=d.get)
来源：http://an.521024.cn

[U10] Py：按值排序字典
来源：http://rr.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ib.gzmigu.cn

[U11] Py：生成器表达式
来源：http://si.colortex.cn

(x * 2 for x in arr)
来源：http://mr.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ne.521024.cn

Counter(arr).most_common(3)
来源：http://mi.bjjhwx.cn

[U13] Py：固定长度队列
来源：http://fv.bjjhwx.cn

deque(maxlen=10)
来源：http://xk.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://da.shxzukj.cn

defaultdict(list)
来源：http://oc.huanxung.cn

[U15] Py：高精度计时
来源：http://zj.huanxung.cn

t = time.perf_counter()
来源：http://ce.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://kn.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ao.huixiangedu.cn

[U17] Py：初始化日志
来源：http://zo.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://ux.nszjky.cn

[U18] Py：预编译正则
来源：http://mi.shxzukj.cn

pat = re.compile(r"\d+")
来源：http://yg.asd995.cn

[U19] Py：正则替换带回调
来源：http://fn.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kt.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://ox.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://ru.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://qr.lnxyls.cn

@contextlib.contextmanager
来源：http://xw.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://nm.newstarts.cn

list(zip(*m))
来源：http://gu.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://jf.bookmarksfly.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ol.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://ew.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ep.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://pm.muxihuayi.cn

csv.DictReader(f)
来源：http://km.chemitech.net.cn

[U26] Py：并发下载
来源：http://da.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nn.521024.cn

[U27] Py：异步 HTTP
来源：http://sg.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qn.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://ns.colortex.cn

UserId = int
来源：http://ly.szxytkj.cn

[U29] Py：属性校验
来源：http://ik.bjjhwx.cn

@property 与 @x.setter 配合
来源：http://fg.hahajie.cn

[U30] Py：数据类
来源：http://ix.chemitech.net.cn

@dataclass(slots=True)
来源：http://em.shxzukj.cn

[U31] Py：单测
来源：http://im.muxihuayi.cn

python -m pytest -q
来源：http://vr.hahajie.cn

[U32] Py：代码格式化
来源：http://xv.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://kb.521024.cn

[U33] Py：打包发布
来源：http://zc.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ve.huanxung.cn

[U34] Py：判断编码
来源：http://eg.jianghongdianzi.cn

chardet.detect(raw)
来源：http://nk.nszjky.cn

[U35] Py：发送邮件
来源：http://zm.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ub.9csxet.cn

[U36] Py：定时任务
来源：http://fw.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://wv.521024.cn

[U37] Py：读写 Excel
来源：http://ky.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://go.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://ol.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://lv.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://cz.shxzukj.cn

sys.stdout.isatty()
来源：http://vl.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://ot.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://fc.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://nf.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xw.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://uo.shtwfgs.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ey.asd995.cn

[U43] PHP：声明命名空间
来源：http://xn.huanxung.cn

namespace App\Http;
来源：http://iq.nicolike.cn

[U44] PHP：开启严格类型
来源：http://cm.yuntaijiaju.cn

declare(strict_types=1);
来源：http://ch.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://ze.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pf.colortex.cn

[U46] PHP：可空类型
来源：http://tb.nszjky.cn

?string $name = null
来源：http://as.panjiajie.cn

[U47] PHP：联合类型
来源：http://ft.newstarts.cn

int|string $id
来源：http://pc.szsharing.cn

[U48] PHP：纯枚举
来源：http://qi.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xe.521024.cn

[U49] PHP：只读属性
来源：http://bl.colortex.cn

public readonly string $name
来源：http://dk.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://ft.gzmigu.cn

public function __construct(private int $id) {}
来源：http://dx.colortex.cn

[U51] PHP：数组解构
来源：http://bh.asd995.cn

[$a, $b] = $arr;
来源：http://rw.huanxung.cn

[U52] PHP：箭头函数
来源：http://bi.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://dq.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://gs.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://mj.huanxung.cn

[U54] PHP：空安全调用
来源：http://wi.bookmarksfly.cn

$obj?->method()
来源：http://my.newstarts.cn

[U55] PHP：match 表达式
来源：http://pw.yuexingan06.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wu.shxzukj.cn

[U56] PHP：命名参数
来源：http://uj.yuexingan06.cn

f(a: 1, b: 2)
来源：http://kd.9csxet.cn

[U57] PHP：字符串插值
来源：http://ws.colortex.cn

"值: {$a}"
来源：http://lk.huanxung.cn

[U58] PHP：数组三件套
来源：http://et.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bl.shxzukj.cn

[U59] PHP：自定义排序
来源：http://kc.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mn.521024.cn

[U60] PHP：JSON 编解码
来源：http://ix.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kn.shxzskj.cn

[U61] PHP：正则
来源：http://zx.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ik.hahajie.cn

[U62] PHP：日期对象
来源：http://al.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vm.shxzukj.cn

[U63] PHP：文件读写
来源：http://qo.colortex.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iy.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://kt.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://yc.asd995.cn

[U65] PHP：会话
来源：http://nj.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ve.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://yf.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iu.nicolike.cn

[U67] PHP：处理文件上传
来源：http://yq.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ur.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://to.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sf.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://jw.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fq.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://lm.colortex.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uh.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://ux.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://hy.nicolike.cn

[U72] PHP：写错误日志
来源：http://wo.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://cg.521024.cn


<!-- 参考信息 -->