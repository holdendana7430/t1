代发 wailian999

[S37] C++：set
来源：http://rg.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bz.bookmarksfly.cn

[S38] C++：排序
来源：http://yi.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://fe.521024.cn

[S39] C++：自定义比较器排序
来源：http://wj.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zy.chemitech.net.cn

[S40] C++：查找元素
来源：http://ku.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mc.nicolike.cn

[S41] C++：类与构造函数
来源：http://mk.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sr.szsharing.cn

[S42] C++：继承与虚函数
来源：http://xw.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://id.521024.cn

[S43] C++：智能指针
来源：http://bw.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://tn.521024.cn

[S44] C++：引用传参
来源：http://gn.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://ut.bookmarksfly.cn

[S45] C++：lambda
来源：http://yv.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tu.521024.cn

[S46] C++：函数模板
来源：http://eq.huanxung.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pt.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://vc.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uw.huanxung.cn

[S48] C++：逐行读文件
来源：http://ak.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bj.newstarts.cn

while (std::getline(in, line)) { }
来源：http://ix.huanxung.cn

[S49] C++：写文件
来源：http://vi.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pf.hahajie.cn

[S50] C++：格式化数字
来源：http://zb.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yu.hnjuh.cn

[S51] C++：显式类型转换
来源：http://cm.shxzskj.cn

static_cast<double>(a) / b
来源：http://zn.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://zm.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://sc.hnjuh.cn

[S53] C++：移动语义
来源：http://xi.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://dw.wgjwhj.cn

[S54] C++：异常处理
来源：http://ds.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xq.gzmigu.cn

[S55] C++：结构化绑定
来源：http://xk.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gf.wgjwhj.cn

[S56] C++：optional
来源：http://io.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://av.gzmigu.cn

[S57] C++：编译期常量
来源：http://em.nszjky.cn

constexpr int N = 10;
来源：http://sb.yuexingan06.cn

[S58] C++：命名空间
来源：http://ws.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://xq.jctech888.com.cn

[S59] C++：静态断言
来源：http://hs.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wc.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://up.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ev.shtwfgs.cn

================================================================================
来源：http://vs.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://je.jianghongdianzi.cn

================================================================================
来源：http://pn.newstarts.cn

[T01] Kotlin：Hello World
来源：http://od.jctech888.com.cn

println("Hello")
来源：http://qc.huanxung.cn

[T02] Kotlin：变量
来源：http://cy.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ov.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://zb.muxihuayi.cn

"值: $b"
来源：http://oj.szsharing.cn

[T04] Kotlin：空安全
来源：http://vm.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://zx.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://ni.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fx.szsharing.cn

[T06] Kotlin：集合映射
来源：http://vl.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cc.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://aw.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://st.nszjky.cn

[T08] Kotlin：数据类
来源：http://nc.asd995.cn

data class User(val name: String, val age: Int)
来源：http://tu.521024.cn

[T09] Kotlin：扩展函数
来源：http://mi.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://iu.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://co.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yw.nicolike.cn

[T11] Kotlin：协程
来源：http://kj.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oi.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://zu.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://qs.chemitech.net.cn

[T13] Kotlin：只读 Map
来源：http://go.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://hm.nszjky.cn

[T14] Kotlin：循环
来源：http://sd.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://zv.huanxung.cn

[T15] Kotlin：接口
来源：http://yk.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://ir.nszjky.cn

[T16] Swift：Hello World
来源：http://kf.shxzskj.cn

print("Hello")
来源：http://cu.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://rd.szsharing.cn

var a = 1;  let b = 2
来源：http://wj.nicolike.cn

[T18] Swift：字符串插值
来源：http://kv.szxytkj.cn

"值: \(b)"
来源：http://fv.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://qf.asd995.cn

if let n = opt { print(n) }
来源：http://hj.haigaiapp.cn

[T20] Swift：数组操作
来源：http://xe.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ni.shxzskj.cn

[T21] Swift：遍历
来源：http://pd.gzmigu.cn

for x in a { print(x) }
来源：http://xi.asd995.cn

[T22] Swift：字典
来源：http://yf.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ej.shxzskj.cn

[T23] Swift：函数
来源：http://ft.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nk.panjiajie.cn

[T24] Swift：闭包
来源：http://if.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ka.521024.cn

[T25] Swift：结构体
来源：http://bm.9csxet.cn

struct P { var x: Int }
来源：http://de.nicolike.cn

[T26] Swift：类与重写
来源：http://sn.nicolike.cn

class A: Base { override func f() {} }
来源：http://eo.asd995.cn

[T27] Swift：错误处理
来源：http://ii.9csxet.cn

do { try f() } catch { print(error) }
来源：http://gv.lnxyls.cn

[T28] Swift：枚举
来源：http://km.yuntaijiaju.cn

enum Color { case red, green }
来源：http://sn.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://tz.bookmarksfly.cn

guard let x = opt else { return }
来源：http://ez.521024.cn

[T30] Swift：协议
来源：http://lz.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://uc.gzmigu.cn

[T31] Lua：Hello World
来源：http://dw.huixinmuqiang.cn

print("Hello")
来源：http://oc.huanxung.cn

[T32] Lua：局部变量
来源：http://xa.huanxung.cn

local a = 1
来源：http://jk.newstarts.cn

[T33] Lua：表（数组）
来源：http://ai.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yo.huixiangedu.cn

[T34] Lua：遍历表
来源：http://ei.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dm.lnxyls.cn

[T35] Lua：字典表
来源：http://bh.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://ub.szxytkj.cn

[T36] Lua：函数
来源：http://oa.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://us.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://uc.jianghongdianzi.cn

"a" .. "b"
来源：http://sq.huixiangedu.cn

[T38] Lua：条件
来源：http://ji.lnxyls.cn

if x > 0 then print("正") end
来源：http://ie.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://rx.colortex.cn

string.find(s, "%d+")
来源：http://sr.521024.cn

[T40] Lua：元表
来源：http://ed.asd995.cn

setmetatable({}, { __index = base })
来源：http://kj.gzmigu.cn

[T41] Perl：Hello World
来源：http://hz.jianghongdianzi.cn

print "Hello\n";
来源：http://gj.9csxet.cn

[T42] Perl：变量类型
来源：http://jf.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fv.nszjky.cn

[T43] Perl：字符串插值
来源：http://xc.huanxung.cn

"值: $a"
来源：http://xf.nicolike.cn

[T44] Perl：条件
来源：http://av.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://ug.asd995.cn

[T45] Perl：数组遍历
来源：http://sa.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://rt.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://vh.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sq.9csxet.cn

[T47] Perl：正则捕获
来源：http://cj.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://db.jctech888.com.cn

[T48] Perl：正则替换
来源：http://vg.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://qv.nicolike.cn

[T49] Perl：函数
来源：http://de.shxzukj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ij.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://mr.panjiajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qt.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ul.szsharing.cn

[T51] Scala：Hello World
来源：http://kb.wgjwhj.cn

println("Hello")
来源：http://nx.haigaiapp.cn

[T52] Scala：变量
来源：http://wr.9csxet.cn

val a = 1;  var b = 2
来源：http://ed.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://ks.hahajie.cn

s"值: $b"
来源：http://fn.muxihuayi.cn

[T54] Scala：集合映射
来源：http://hn.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://zz.newstarts.cn

[T55] Scala：集合过滤
来源：http://qt.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vh.panjiajie.cn

[T56] Scala：样例类
来源：http://fy.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://bq.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://ff.wgjwhj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ji.huanxung.cn

[T58] Scala：函数定义
来源：http://mc.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tp.muxihuayi.cn

[T59] Scala：循环
来源：http://jg.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://cq.szsharing.cn

[T60] Scala：折叠
来源：http://jv.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jj.9csxet.cn

================================================================================
来源：http://bq.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xp.huixinmuqiang.cn

================================================================================
来源：http://du.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://vi.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pm.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://yp.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vp.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://ii.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ib.szxytkj.cn

[U04] Py：变量调试打印
来源：http://nz.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gk.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://qf.gzmigu.cn

list(dict.fromkeys(arr))
来源：http://vr.nszjky.cn

[U06] Py：合并两个字典
来源：http://lh.shxzukj.cn

{**a, **b}
来源：http://rc.9csxet.cn

[U07] Py：反转字典键值
来源：http://kp.yuexingan06.cn

{v: k for k, v in d.items()}
来源：http://uw.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://nv.shxzskj.cn

[y for x in nested for y in x]
来源：http://gn.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://nl.lnxyls.cn

max(d, key=d.get)
来源：http://wy.szsharing.cn

[U10] Py：按值排序字典
来源：http://xz.colortex.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fn.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://ih.hahajie.cn

(x * 2 for x in arr)
来源：http://dy.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xc.hahajie.cn

Counter(arr).most_common(3)
来源：http://si.newstarts.cn

[U13] Py：固定长度队列
来源：http://pe.szsharing.cn

deque(maxlen=10)
来源：http://lh.bjjhwx.cn

[U14] Py：分组收集到列表
来源：http://eu.bjjhwx.cn

defaultdict(list)
来源：http://mp.szsharing.cn

[U15] Py：高精度计时
来源：http://ti.haigaiapp.cn

t = time.perf_counter()
来源：http://eq.9csxet.cn

[U16] Py：命令行参数解析
来源：http://yh.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rp.szxytkj.cn

[U17] Py：初始化日志
来源：http://vc.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://fu.gzmigu.cn

[U18] Py：预编译正则
来源：http://qa.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://ov.jctech888.com.cn

[U19] Py：正则替换带回调
来源：http://kz.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://di.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://yc.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://pe.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://on.hahajie.cn

@contextlib.contextmanager
来源：http://kn.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://gx.shtwfgs.cn

list(zip(*m))
来源：http://mp.nszjky.cn

[U23] Py：分块读取大文件
来源：http://ai.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rw.szxytkj.cn

[U24] Py：路径操作
来源：http://uf.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fu.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://ui.panjiajie.cn

csv.DictReader(f)
来源：http://co.haigaiapp.cn

[U26] Py：并发下载
来源：http://ka.huixiangedu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vh.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://gl.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://jq.yuexingan06.cn

[U28] Py：类型别名
来源：http://xx.521024.cn

UserId = int
来源：http://te.szsharing.cn

[U29] Py：属性校验
来源：http://bl.nicolike.cn

@property 与 @x.setter 配合
来源：http://yy.chemitech.net.cn

[U30] Py：数据类
来源：http://qv.asd995.cn

@dataclass(slots=True)
来源：http://hh.jctech888.com.cn

[U31] Py：单测
来源：http://vl.muxihuayi.cn

python -m pytest -q
来源：http://hv.chemitech.net.cn

[U32] Py：代码格式化
来源：http://zy.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://en.gzmigu.cn

[U33] Py：打包发布
来源：http://wm.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://gv.shxzukj.cn

[U34] Py：判断编码
来源：http://xl.lnxyls.cn

chardet.detect(raw)
来源：http://kr.szxytkj.cn

[U35] Py：发送邮件
来源：http://hj.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yi.shtwfgs.cn

[U36] Py：定时任务
来源：http://eb.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://sz.gzmigu.cn

[U37] Py：读写 Excel
来源：http://ib.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hl.huanxung.cn

[U38] Py：获取脚本所在目录
来源：http://oe.szxytkj.cn

Path(__file__).resolve().parent
来源：http://le.haigaiapp.cn

[U39] Py：判断是否在交互环境
来源：http://mx.9csxet.cn

sys.stdout.isatty()
来源：http://sf.bookmarksfly.cn

[U40] Py：打印到标准错误
来源：http://ya.szxytkj.cn

print("err", file=sys.stderr)
来源：http://tn.szxytkj.cn

[U41] PHP：初始化 Composer 项目
来源：http://no.newstarts.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yj.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://ei.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aq.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://cq.jianghongdianzi.cn

namespace App\Http;
来源：http://wu.yuntaijiaju.cn

[U44] PHP：开启严格类型
来源：http://jf.bookmarksfly.cn

declare(strict_types=1);
来源：http://qd.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://zw.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://er.9csxet.cn

[U46] PHP：可空类型
来源：http://ar.hahajie.cn

?string $name = null
来源：http://xl.huixiangedu.cn

[U47] PHP：联合类型
来源：http://ca.haigaiapp.cn

int|string $id
来源：http://me.hnjuh.cn

[U48] PHP：纯枚举
来源：http://fm.huixiangedu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vq.panjiajie.cn

[U49] PHP：只读属性
来源：http://ah.nszjky.cn

public readonly string $name
来源：http://kp.jctech888.com.cn

[U50] PHP：构造器属性提升
来源：http://gi.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://kx.asd995.cn

[U51] PHP：数组解构
来源：http://ek.nicolike.cn

[$a, $b] = $arr;
来源：http://tz.hnjuh.cn

[U52] PHP：箭头函数
来源：http://om.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://vi.huanxung.cn

[U53] PHP：空合并运算符
来源：http://ho.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://zm.bookmarksfly.cn

[U54] PHP：空安全调用
来源：http://ih.jctech888.com.cn

$obj?->method()
来源：http://tr.shxzskj.cn

[U55] PHP：match 表达式
来源：http://un.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ek.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://gx.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://pi.gzmigu.cn

[U57] PHP：字符串插值
来源：http://as.gzmigu.cn

"值: {$a}"
来源：http://rj.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://ko.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oq.9csxet.cn

[U59] PHP：自定义排序
来源：http://mj.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zk.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://aq.lnxyls.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tn.bjjhwx.cn

[U61] PHP：正则
来源：http://ex.shtwfgs.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fk.hahajie.cn

[U62] PHP：日期对象
来源：http://dx.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cg.shtwfgs.cn


<!-- 参考信息 -->