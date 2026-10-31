代发 wailian999

[S39] C++：自定义比较器排序
来源：http://yr.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vv.shtwfgs.cn

[S40] C++：查找元素
来源：http://rn.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ns.colortex.cn

[S41] C++：类与构造函数
来源：http://jx.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wo.521024.cn

[S42] C++：继承与虚函数
来源：http://zh.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://zi.hahajie.cn

[S43] C++：智能指针
来源：http://aw.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://ma.bjjhwx.cn

[S44] C++：引用传参
来源：http://cx.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://yl.huixinmuqiang.cn

[S45] C++：lambda
来源：http://ds.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vq.shxzukj.cn

[S46] C++：函数模板
来源：http://vp.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bq.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://vk.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jx.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://bh.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vz.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://oh.hahajie.cn

[S49] C++：写文件
来源：http://tf.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rv.521024.cn

[S50] C++：格式化数字
来源：http://ds.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tc.lnxyls.cn

[S51] C++：显式类型转换
来源：http://sx.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://sq.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://ah.521024.cn

int size() const noexcept { return n_; }
来源：http://ct.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://tb.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://xs.gzmigu.cn

[S54] C++：异常处理
来源：http://bm.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://on.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://uf.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qx.shxzukj.cn

[S56] C++：optional
来源：http://lh.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eo.9csxet.cn

[S57] C++：编译期常量
来源：http://ae.yuexingan06.cn

constexpr int N = 10;
来源：http://gy.huanxung.cn

[S58] C++：命名空间
来源：http://so.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://tx.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://en.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jm.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://zf.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vo.huanxung.cn

================================================================================
来源：http://za.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ap.szsharing.cn

================================================================================
来源：http://iw.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://cy.huixiangedu.cn

println("Hello")
来源：http://pz.asd995.cn

[T02] Kotlin：变量
来源：http://ay.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sg.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://lt.hnjuh.cn

"值: $b"
来源：http://ws.szsharing.cn

[T04] Kotlin：空安全
来源：http://ws.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://tq.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://ap.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hx.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://ju.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vk.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://dz.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://up.asd995.cn

[T08] Kotlin：数据类
来源：http://vu.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://gr.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://kt.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://or.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://tg.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://os.haigaiapp.cn

[T11] Kotlin：协程
来源：http://te.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pi.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://uw.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://ua.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://pr.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://xg.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://pc.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://ih.muxihuayi.cn

[T15] Kotlin：接口
来源：http://rs.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://hn.yuexingan06.cn

[T16] Swift：Hello World
来源：http://fy.nicolike.cn

print("Hello")
来源：http://gc.gzmigu.cn

[T17] Swift：变量与常量
来源：http://ta.huanxung.cn

var a = 1;  let b = 2
来源：http://bu.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://pi.shtwfgs.cn

"值: \(b)"
来源：http://jq.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://xb.lnxyls.cn

if let n = opt { print(n) }
来源：http://ij.9csxet.cn

[T20] Swift：数组操作
来源：http://dq.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fy.szxytkj.cn

[T21] Swift：遍历
来源：http://js.szsharing.cn

for x in a { print(x) }
来源：http://ib.shxzskj.cn

[T22] Swift：字典
来源：http://bv.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ru.jctech888.com.cn

[T23] Swift：函数
来源：http://rs.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rv.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://vs.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ny.nszjky.cn

[T25] Swift：结构体
来源：http://pu.szsharing.cn

struct P { var x: Int }
来源：http://xq.huixiangedu.cn

[T26] Swift：类与重写
来源：http://md.9csxet.cn

class A: Base { override func f() {} }
来源：http://mh.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://ap.521024.cn

do { try f() } catch { print(error) }
来源：http://mv.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://mh.huanxung.cn

enum Color { case red, green }
来源：http://gv.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://fl.shxzskj.cn

guard let x = opt else { return }
来源：http://wt.newstarts.cn

[T30] Swift：协议
来源：http://rr.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://hv.nszjky.cn

[T31] Lua：Hello World
来源：http://eq.muxihuayi.cn

print("Hello")
来源：http://pg.shtwfgs.cn

[T32] Lua：局部变量
来源：http://oe.nszjky.cn

local a = 1
来源：http://et.huanxung.cn

[T33] Lua：表（数组）
来源：http://yr.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wc.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ii.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ra.bookmarksfly.cn

[T35] Lua：字典表
来源：http://tk.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://pz.lnxyls.cn

[T36] Lua：函数
来源：http://bc.shxzskj.cn

function add(a, b) return a + b end
来源：http://qo.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://le.lnxyls.cn

"a" .. "b"
来源：http://ra.szsharing.cn

[T38] Lua：条件
来源：http://bn.newstarts.cn

if x > 0 then print("正") end
来源：http://qi.lnxyls.cn

[T39] Lua：模式匹配
来源：http://zr.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://ga.shxzukj.cn

[T40] Lua：元表
来源：http://kv.huanxung.cn

setmetatable({}, { __index = base })
来源：http://fk.shtwfgs.cn

[T41] Perl：Hello World
来源：http://qm.wgjwhj.cn

print "Hello\n";
来源：http://se.panjiajie.cn

[T42] Perl：变量类型
来源：http://mw.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vd.shxzukj.cn

[T43] Perl：字符串插值
来源：http://up.muxihuayi.cn

"值: $a"
来源：http://kr.huanxung.cn

[T44] Perl：条件
来源：http://ex.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://oh.hahajie.cn

[T45] Perl：数组遍历
来源：http://ko.asd995.cn

for my $x (@arr) { print $x; }
来源：http://mb.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://mn.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dd.colortex.cn

[T47] Perl：正则捕获
来源：http://du.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ha.muxihuayi.cn

[T48] Perl：正则替换
来源：http://qp.521024.cn

$s =~ s/old/new/g;
来源：http://jv.shxzukj.cn

[T49] Perl：函数
来源：http://sb.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jq.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://yx.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sg.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://xs.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://xy.bjjhwx.cn

println("Hello")
来源：http://tr.nszjky.cn

[T52] Scala：变量
来源：http://lx.nicolike.cn

val a = 1;  var b = 2
来源：http://ov.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://yb.hahajie.cn

s"值: $b"
来源：http://qb.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://fl.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://fn.hnjuh.cn

[T55] Scala：集合过滤
来源：http://hk.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://po.newstarts.cn

[T56] Scala：样例类
来源：http://gw.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://tq.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://is.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jz.nszjky.cn

[T58] Scala：函数定义
来源：http://oh.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jj.szsharing.cn

[T59] Scala：循环
来源：http://aw.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://vq.szxytkj.cn

[T60] Scala：折叠
来源：http://rv.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zy.haigaiapp.cn

================================================================================
来源：http://qw.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://id.hnjuh.cn

================================================================================
来源：http://ky.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://rs.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bf.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://jm.521024.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://um.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://dc.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sd.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://nd.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://va.panjiajie.cn

[U05] Py：列表去重且保序
来源：http://lb.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://sv.9csxet.cn

[U06] Py：合并两个字典
来源：http://jv.huixiangedu.cn

{**a, **b}
来源：http://uu.szxytkj.cn

[U07] Py：反转字典键值
来源：http://lf.hahajie.cn

{v: k for k, v in d.items()}
来源：http://vt.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://yj.shxzukj.cn

[y for x in nested for y in x]
来源：http://gq.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://ku.newstarts.cn

max(d, key=d.get)
来源：http://ik.yuexingan06.cn

[U10] Py：按值排序字典
来源：http://zq.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yb.shxzukj.cn

[U11] Py：生成器表达式
来源：http://sq.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://nn.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vh.newstarts.cn

Counter(arr).most_common(3)
来源：http://qi.gzmigu.cn

[U13] Py：固定长度队列
来源：http://xg.chemitech.net.cn

deque(maxlen=10)
来源：http://dk.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://lv.muxihuayi.cn

defaultdict(list)
来源：http://kk.huanxung.cn

[U15] Py：高精度计时
来源：http://yv.huixinmuqiang.cn

t = time.perf_counter()
来源：http://pi.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://gv.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nq.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://sa.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://sr.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://da.nszjky.cn

pat = re.compile(r"\d+")
来源：http://nz.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://be.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bu.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://ez.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://xx.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://td.bjjhwx.cn

@contextlib.contextmanager
来源：http://mg.shxzukj.cn

[U22] Py：矩阵转置
来源：http://eg.shtwfgs.cn

list(zip(*m))
来源：http://rs.szsharing.cn

[U23] Py：分块读取大文件
来源：http://cw.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fg.newstarts.cn

[U24] Py：路径操作
来源：http://go.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fo.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://lg.haigaiapp.cn

csv.DictReader(f)
来源：http://py.shxzukj.cn

[U26] Py：并发下载
来源：http://yp.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zk.szsharing.cn

[U27] Py：异步 HTTP
来源：http://yc.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://zs.521024.cn

[U28] Py：类型别名
来源：http://id.bookmarksfly.cn

UserId = int
来源：http://ty.bjjhwx.cn

[U29] Py：属性校验
来源：http://dh.newstarts.cn

@property 与 @x.setter 配合
来源：http://vy.asd995.cn

[U30] Py：数据类
来源：http://ex.lnxyls.cn

@dataclass(slots=True)
来源：http://ik.haigaiapp.cn

[U31] Py：单测
来源：http://bo.muxihuayi.cn

python -m pytest -q
来源：http://ck.9csxet.cn

[U32] Py：代码格式化
来源：http://ab.9csxet.cn

ruff format . && ruff check --fix .
来源：http://ho.9csxet.cn

[U33] Py：打包发布
来源：http://rm.szsharing.cn

python -m build  （依赖 pyproject.toml）
来源：http://rb.newstarts.cn

[U34] Py：判断编码
来源：http://bm.huixinmuqiang.cn

chardet.detect(raw)
来源：http://oe.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://xj.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ui.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://vc.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://qu.521024.cn

[U37] Py：读写 Excel
来源：http://uj.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vs.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://po.szxytkj.cn

Path(__file__).resolve().parent
来源：http://nt.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://iz.muxihuayi.cn

sys.stdout.isatty()
来源：http://af.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://ve.huanxung.cn

print("err", file=sys.stderr)
来源：http://ag.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://dq.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://st.haigaiapp.cn

[U42] PHP：PSR-4 自动加载
来源：http://yv.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xy.jianghongdianzi.cn

[U43] PHP：声明命名空间
来源：http://yd.521024.cn

namespace App\Http;
来源：http://zl.521024.cn

[U44] PHP：开启严格类型
来源：http://ey.jianghongdianzi.cn

declare(strict_types=1);
来源：http://il.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://eo.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://us.shxzskj.cn

[U46] PHP：可空类型
来源：http://rr.haigaiapp.cn

?string $name = null
来源：http://rt.bjjhwx.cn

[U47] PHP：联合类型
来源：http://cm.hahajie.cn

int|string $id
来源：http://uw.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://om.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kt.huanxung.cn

[U49] PHP：只读属性
来源：http://hx.newstarts.cn

public readonly string $name
来源：http://hd.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://wp.nszjky.cn

public function __construct(private int $id) {}
来源：http://uc.yuexingan06.cn

[U51] PHP：数组解构
来源：http://pa.colortex.cn

[$a, $b] = $arr;
来源：http://nu.gzmigu.cn

[U52] PHP：箭头函数
来源：http://ww.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://ig.panjiajie.cn

[U53] PHP：空合并运算符
来源：http://re.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://sx.521024.cn

[U54] PHP：空安全调用
来源：http://bz.jianghongdianzi.cn

$obj?->method()
来源：http://fm.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://kl.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rx.yuexingan06.cn

[U56] PHP：命名参数
来源：http://yf.wgjwhj.cn

f(a: 1, b: 2)
来源：http://ca.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://zh.yuntaijiaju.cn

"值: {$a}"
来源：http://jt.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://fw.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://si.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://sw.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rn.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://za.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nd.bjjhwx.cn

[U61] PHP：正则
来源：http://tc.szsharing.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yo.lnxyls.cn

[U62] PHP：日期对象
来源：http://yr.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://om.shtwfgs.cn

[U63] PHP：文件读写
来源：http://ml.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ib.huixiangedu.cn

[U64] PHP：目录遍历
来源：http://lk.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ul.9csxet.cn


<!-- 参考信息 -->