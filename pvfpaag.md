代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://lt.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oh.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://sv.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lx.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://hz.lnxyls.cn

[S49] C++：写文件
来源：http://xx.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://td.yuexingan06.cn

[S50] C++：格式化数字
来源：http://xv.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tu.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://zk.lnxyls.cn

static_cast<double>(a) / b
来源：http://rv.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://hs.szsharing.cn

int size() const noexcept { return n_; }
来源：http://nc.bjjhwx.cn

[S53] C++：移动语义
来源：http://qv.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://ol.hnjuh.cn

[S54] C++：异常处理
来源：http://zp.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vi.9csxet.cn

[S55] C++：结构化绑定
来源：http://tw.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hm.shxzskj.cn

[S56] C++：optional
来源：http://xk.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qb.huanxung.cn

[S57] C++：编译期常量
来源：http://qn.haigaiapp.cn

constexpr int N = 10;
来源：http://kc.nszjky.cn

[S58] C++：命名空间
来源：http://ci.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://fv.asd995.cn

[S59] C++：静态断言
来源：http://wi.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yx.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://ky.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ke.huixinmuqiang.cn

================================================================================
来源：http://uw.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ny.bjjhwx.cn

================================================================================
来源：http://cb.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://dc.szxytkj.cn

println("Hello")
来源：http://eh.panjiajie.cn

[T02] Kotlin：变量
来源：http://it.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hd.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://dk.huanxung.cn

"值: $b"
来源：http://an.521024.cn

[T04] Kotlin：空安全
来源：http://ps.521024.cn

val n: String? = null;  n?.length
来源：http://uy.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://xz.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gf.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://te.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cy.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://bb.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ff.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://rg.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://wu.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://hw.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://we.asd995.cn

[T10] Kotlin：默认参数
来源：http://xx.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ew.shtwfgs.cn

[T11] Kotlin：协程
来源：http://sy.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ky.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://ko.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://hd.521024.cn

[T13] Kotlin：只读 Map
来源：http://dh.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://dq.panjiajie.cn

[T14] Kotlin：循环
来源：http://dd.huanxung.cn

for (i in 1..10) println(i)
来源：http://zg.hnjuh.cn

[T15] Kotlin：接口
来源：http://dd.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://to.nszjky.cn

[T16] Swift：Hello World
来源：http://ct.shtwfgs.cn

print("Hello")
来源：http://tp.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://mp.shxzukj.cn

var a = 1;  let b = 2
来源：http://mx.shxzukj.cn

[T18] Swift：字符串插值
来源：http://zk.muxihuayi.cn

"值: \(b)"
来源：http://cs.szsharing.cn

[T19] Swift：可选绑定
来源：http://by.hahajie.cn

if let n = opt { print(n) }
来源：http://ae.shtwfgs.cn

[T20] Swift：数组操作
来源：http://vf.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vq.shxzukj.cn

[T21] Swift：遍历
来源：http://vm.hnjuh.cn

for x in a { print(x) }
来源：http://mv.szxytkj.cn

[T22] Swift：字典
来源：http://lw.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ui.hahajie.cn

[T23] Swift：函数
来源：http://hb.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nu.haigaiapp.cn

[T24] Swift：闭包
来源：http://kx.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pz.haigaiapp.cn

[T25] Swift：结构体
来源：http://xv.nicolike.cn

struct P { var x: Int }
来源：http://rz.haigaiapp.cn

[T26] Swift：类与重写
来源：http://ug.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://dc.shxzskj.cn

[T27] Swift：错误处理
来源：http://ra.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://ow.colortex.cn

[T28] Swift：枚举
来源：http://vd.huanxung.cn

enum Color { case red, green }
来源：http://uc.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://dr.lnxyls.cn

guard let x = opt else { return }
来源：http://po.gzmigu.cn

[T30] Swift：协议
来源：http://wl.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://re.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://sg.huixiangedu.cn

print("Hello")
来源：http://qw.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://tt.szsharing.cn

local a = 1
来源：http://bo.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://hw.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oq.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://ie.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zf.nszjky.cn

[T35] Lua：字典表
来源：http://bl.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://ky.9csxet.cn

[T36] Lua：函数
来源：http://ru.nicolike.cn

function add(a, b) return a + b end
来源：http://mr.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://os.jianghongdianzi.cn

"a" .. "b"
来源：http://pm.chemitech.net.cn

[T38] Lua：条件
来源：http://no.panjiajie.cn

if x > 0 then print("正") end
来源：http://ru.asd995.cn

[T39] Lua：模式匹配
来源：http://xe.shxzukj.cn

string.find(s, "%d+")
来源：http://ms.hnjuh.cn

[T40] Lua：元表
来源：http://jb.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://ly.bjjhwx.cn

[T41] Perl：Hello World
来源：http://gy.huanxung.cn

print "Hello\n";
来源：http://iz.szsharing.cn

[T42] Perl：变量类型
来源：http://rp.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ll.asd995.cn

[T43] Perl：字符串插值
来源：http://ca.huixinmuqiang.cn

"值: $a"
来源：http://ee.wgjwhj.cn

[T44] Perl：条件
来源：http://hq.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://ls.lnxyls.cn

[T45] Perl：数组遍历
来源：http://fg.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://dj.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://ty.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vr.hahajie.cn

[T47] Perl：正则捕获
来源：http://mc.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hu.nszjky.cn

[T48] Perl：正则替换
来源：http://om.hnjuh.cn

$s =~ s/old/new/g;
来源：http://iv.huixinmuqiang.cn

[T49] Perl：函数
来源：http://wr.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://to.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://xt.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nx.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://bz.szsharing.cn

[T51] Scala：Hello World
来源：http://xp.lnxyls.cn

println("Hello")
来源：http://iy.lnxyls.cn

[T52] Scala：变量
来源：http://ld.9csxet.cn

val a = 1;  var b = 2
来源：http://oq.521024.cn

[T53] Scala：字符串插值
来源：http://os.huixiangedu.cn

s"值: $b"
来源：http://ug.521024.cn

[T54] Scala：集合映射
来源：http://iq.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://zp.gzmigu.cn

[T55] Scala：集合过滤
来源：http://of.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://at.nicolike.cn

[T56] Scala：样例类
来源：http://ry.nszjky.cn

case class User(name: String, age: Int)
来源：http://wd.hnjuh.cn

[T57] Scala：模式匹配
来源：http://at.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ci.szxytkj.cn

[T58] Scala：函数定义
来源：http://fz.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yv.huixiangedu.cn

[T59] Scala：循环
来源：http://rw.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://kf.shxzukj.cn

[T60] Scala：折叠
来源：http://gu.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aa.szxytkj.cn

================================================================================
来源：http://ns.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hj.gzmigu.cn

================================================================================
来源：http://nh.asd995.cn

[U01] Py：创建虚拟环境
来源：http://qx.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bn.hnjuh.cn

[U02] Py：导出 / 安装依赖
来源：http://np.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yq.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://nx.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://el.colortex.cn

[U04] Py：变量调试打印
来源：http://fk.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://re.asd995.cn

[U05] Py：列表去重且保序
来源：http://wu.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://bb.hnjuh.cn

[U06] Py：合并两个字典
来源：http://te.9csxet.cn

{**a, **b}
来源：http://iw.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://ac.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://gk.newstarts.cn

[U08] Py：展平二维列表
来源：http://ev.nicolike.cn

[y for x in nested for y in x]
来源：http://ln.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://vx.huixinmuqiang.cn

max(d, key=d.get)
来源：http://kh.hnjuh.cn

[U10] Py：按值排序字典
来源：http://vo.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sj.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://kf.gzmigu.cn

(x * 2 for x in arr)
来源：http://hd.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yw.newstarts.cn

Counter(arr).most_common(3)
来源：http://oy.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://nh.nicolike.cn

deque(maxlen=10)
来源：http://kb.colortex.cn

[U14] Py：分组收集到列表
来源：http://iv.asd995.cn

defaultdict(list)
来源：http://ud.521024.cn

[U15] Py：高精度计时
来源：http://xd.newstarts.cn

t = time.perf_counter()
来源：http://xv.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://of.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dl.huixiangedu.cn

[U17] Py：初始化日志
来源：http://jv.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://xh.muxihuayi.cn

[U18] Py：预编译正则
来源：http://if.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://or.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://jz.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ar.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://na.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://oz.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://ym.521024.cn

@contextlib.contextmanager
来源：http://ae.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://rp.szsharing.cn

list(zip(*m))
来源：http://dc.hahajie.cn

[U23] Py：分块读取大文件
来源：http://ra.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xx.yuexingan06.cn

[U24] Py：路径操作
来源：http://cd.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ll.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://bw.yuntaijiaju.cn

csv.DictReader(f)
来源：http://be.bjjhwx.cn

[U26] Py：并发下载
来源：http://qo.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ja.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://cd.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://kb.bookmarksfly.cn

[U28] Py：类型别名
来源：http://ji.huixinmuqiang.cn

UserId = int
来源：http://yo.gzmigu.cn

[U29] Py：属性校验
来源：http://vy.hahajie.cn

@property 与 @x.setter 配合
来源：http://qv.muxihuayi.cn

[U30] Py：数据类
来源：http://zm.huixiangedu.cn

@dataclass(slots=True)
来源：http://ra.jctech888.com.cn

[U31] Py：单测
来源：http://cy.wgjwhj.cn

python -m pytest -q
来源：http://cu.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://gm.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://rr.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://ta.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://hx.huixiangedu.cn

[U34] Py：判断编码
来源：http://on.hahajie.cn

chardet.detect(raw)
来源：http://um.colortex.cn

[U35] Py：发送邮件
来源：http://nf.newstarts.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dn.asd995.cn

[U36] Py：定时任务
来源：http://sp.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://cm.hnjuh.cn

[U37] Py：读写 Excel
来源：http://mc.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fm.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://cw.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://qb.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://kz.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://wl.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://lf.nicolike.cn

print("err", file=sys.stderr)
来源：http://ti.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://nz.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qs.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://hy.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cb.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://er.shtwfgs.cn

namespace App\Http;
来源：http://cm.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://qd.wgjwhj.cn

declare(strict_types=1);
来源：http://tt.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://kn.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hh.shxzukj.cn

[U46] PHP：可空类型
来源：http://wj.muxihuayi.cn

?string $name = null
来源：http://ij.newstarts.cn

[U47] PHP：联合类型
来源：http://zo.newstarts.cn

int|string $id
来源：http://lz.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://ss.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ht.szxytkj.cn

[U49] PHP：只读属性
来源：http://uq.shtwfgs.cn

public readonly string $name
来源：http://ib.huanxung.cn

[U50] PHP：构造器属性提升
来源：http://np.szxytkj.cn

public function __construct(private int $id) {}
来源：http://uw.chemitech.net.cn

[U51] PHP：数组解构
来源：http://lh.szxytkj.cn

[$a, $b] = $arr;
来源：http://ne.muxihuayi.cn

[U52] PHP：箭头函数
来源：http://ev.szsharing.cn

$double = fn($x) => $x * 2;
来源：http://kp.nszjky.cn

[U53] PHP：空合并运算符
来源：http://ac.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://uk.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://qe.huanxung.cn

$obj?->method()
来源：http://wg.gzmigu.cn

[U55] PHP：match 表达式
来源：http://gn.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dv.panjiajie.cn

[U56] PHP：命名参数
来源：http://vj.shtwfgs.cn

f(a: 1, b: 2)
来源：http://ps.gzmigu.cn

[U57] PHP：字符串插值
来源：http://da.huixiangedu.cn

"值: {$a}"
来源：http://dv.gzmigu.cn

[U58] PHP：数组三件套
来源：http://qu.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ow.newstarts.cn

[U59] PHP：自定义排序
来源：http://sr.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://je.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://cs.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cn.panjiajie.cn

[U61] PHP：正则
来源：http://tx.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bh.lnxyls.cn

[U62] PHP：日期对象
来源：http://el.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mw.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://pu.nszjky.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ur.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://hi.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://vp.huanxung.cn

[U65] PHP：会话
来源：http://zj.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qp.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://hs.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lu.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://zb.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zm.9csxet.cn

[U68] PHP：PDO 连接
来源：http://mo.chemitech.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ql.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://yk.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://od.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://fk.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fj.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://do.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://bk.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://la.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://xa.yuexingan06.cn


<!-- 参考信息 -->