代发 wailian999

[S35] C++：map
来源：http://uw.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hw.nicolike.cn

[S36] C++：unordered_map
来源：http://zv.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hq.haigaiapp.cn

[S37] C++：set
来源：http://ok.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gs.panjiajie.cn

[S38] C++：排序
来源：http://ck.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://ux.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ry.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ll.panjiajie.cn

[S40] C++：查找元素
来源：http://re.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fk.szxytkj.cn

[S41] C++：类与构造函数
来源：http://rd.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sb.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://wx.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://vu.bjjhwx.cn

[S43] C++：智能指针
来源：http://do.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://pk.haigaiapp.cn

[S44] C++：引用传参
来源：http://do.jianghongdianzi.cn

void inc(int &x) { ++x; }
来源：http://hf.huanxung.cn

[S45] C++：lambda
来源：http://av.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://co.yuexingan06.cn

[S46] C++：函数模板
来源：http://vz.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xv.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://xt.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mr.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://pq.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://od.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://rs.chemitech.net.cn

[S49] C++：写文件
来源：http://vf.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ok.jctech888.com.cn

[S50] C++：格式化数字
来源：http://ne.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dh.szsharing.cn

[S51] C++：显式类型转换
来源：http://hc.shxzukj.cn

static_cast<double>(a) / b
来源：http://wq.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://bg.nicolike.cn

int size() const noexcept { return n_; }
来源：http://st.bookmarksfly.cn

[S53] C++：移动语义
来源：http://ua.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://so.yuexingan06.cn

[S54] C++：异常处理
来源：http://aw.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mx.hnjuh.cn

[S55] C++：结构化绑定
来源：http://rf.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ny.hnjuh.cn

[S56] C++：optional
来源：http://rj.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://la.huanxung.cn

[S57] C++：编译期常量
来源：http://sv.huixinmuqiang.cn

constexpr int N = 10;
来源：http://kb.nszjky.cn

[S58] C++：命名空间
来源：http://fe.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://wy.nicolike.cn

[S59] C++：静态断言
来源：http://ct.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jj.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://wi.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jg.asd995.cn

================================================================================
来源：http://ab.huixinmuqiang.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pl.huixiangedu.cn

================================================================================
来源：http://sv.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://lk.huixiangedu.cn

println("Hello")
来源：http://gy.panjiajie.cn

[T02] Kotlin：变量
来源：http://iz.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yz.muxihuayi.cn

[T03] Kotlin：字符串模板
来源：http://pm.nszjky.cn

"值: $b"
来源：http://dg.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://pc.lnxyls.cn

val n: String? = null;  n?.length
来源：http://xw.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://nr.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ry.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://yg.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cj.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://zm.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gi.hahajie.cn

[T08] Kotlin：数据类
来源：http://mm.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://wr.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://wl.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://nv.nicolike.cn

[T10] Kotlin：默认参数
来源：http://va.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qv.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://qn.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uo.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://vl.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://hp.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://uf.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://nk.szxytkj.cn

[T14] Kotlin：循环
来源：http://fj.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://zv.haigaiapp.cn

[T15] Kotlin：接口
来源：http://lg.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://up.shxzskj.cn

[T16] Swift：Hello World
来源：http://nk.colortex.cn

print("Hello")
来源：http://hr.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ad.szsharing.cn

var a = 1;  let b = 2
来源：http://px.szsharing.cn

[T18] Swift：字符串插值
来源：http://xp.colortex.cn

"值: \(b)"
来源：http://ls.szsharing.cn

[T19] Swift：可选绑定
来源：http://fl.chemitech.net.cn

if let n = opt { print(n) }
来源：http://ys.szxytkj.cn

[T20] Swift：数组操作
来源：http://lw.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ma.hahajie.cn

[T21] Swift：遍历
来源：http://kc.lnxyls.cn

for x in a { print(x) }
来源：http://je.521024.cn

[T22] Swift：字典
来源：http://mm.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kr.shxzukj.cn

[T23] Swift：函数
来源：http://jk.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tg.gzmigu.cn

[T24] Swift：闭包
来源：http://og.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sj.nicolike.cn

[T25] Swift：结构体
来源：http://rw.szxytkj.cn

struct P { var x: Int }
来源：http://qg.haigaiapp.cn

[T26] Swift：类与重写
来源：http://bb.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://xy.nicolike.cn

[T27] Swift：错误处理
来源：http://kh.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ob.gzmigu.cn

[T28] Swift：枚举
来源：http://gc.jianghongdianzi.cn

enum Color { case red, green }
来源：http://cd.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://zy.asd995.cn

guard let x = opt else { return }
来源：http://mh.muxihuayi.cn

[T30] Swift：协议
来源：http://cr.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://ha.huixiangedu.cn

[T31] Lua：Hello World
来源：http://fv.jctech888.com.cn

print("Hello")
来源：http://dc.chemitech.net.cn

[T32] Lua：局部变量
来源：http://xu.nicolike.cn

local a = 1
来源：http://fu.521024.cn

[T33] Lua：表（数组）
来源：http://ox.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hc.lnxyls.cn

[T34] Lua：遍历表
来源：http://fj.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yt.yuexingan06.cn

[T35] Lua：字典表
来源：http://zl.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://qm.chemitech.net.cn

[T36] Lua：函数
来源：http://it.521024.cn

function add(a, b) return a + b end
来源：http://ru.colortex.cn

[T37] Lua：字符串拼接
来源：http://mt.wgjwhj.cn

"a" .. "b"
来源：http://uk.bjjhwx.cn

[T38] Lua：条件
来源：http://nw.panjiajie.cn

if x > 0 then print("正") end
来源：http://vx.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://rr.bookmarksfly.cn

string.find(s, "%d+")
来源：http://fi.huanxung.cn

[T40] Lua：元表
来源：http://cs.asd995.cn

setmetatable({}, { __index = base })
来源：http://hq.szxytkj.cn

[T41] Perl：Hello World
来源：http://nx.bookmarksfly.cn

print "Hello\n";
来源：http://yw.wgjwhj.cn

[T42] Perl：变量类型
来源：http://vg.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xj.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://kc.bjjhwx.cn

"值: $a"
来源：http://te.newstarts.cn

[T44] Perl：条件
来源：http://mr.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://uc.colortex.cn

[T45] Perl：数组遍历
来源：http://yy.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://gb.colortex.cn

[T46] Perl：哈希操作
来源：http://kw.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ao.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://or.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://em.szxytkj.cn

[T48] Perl：正则替换
来源：http://sn.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://tu.huixiangedu.cn

[T49] Perl：函数
来源：http://uh.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ow.nszjky.cn

[T50] Perl：逐行读文件
来源：http://ka.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kj.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://un.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://qq.chemitech.net.cn

println("Hello")
来源：http://up.huixinmuqiang.cn

[T52] Scala：变量
来源：http://av.colortex.cn

val a = 1;  var b = 2
来源：http://wq.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://qx.yuntaijiaju.cn

s"值: $b"
来源：http://qr.newstarts.cn

[T54] Scala：集合映射
来源：http://vf.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://tl.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://hi.shtwfgs.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pn.gzmigu.cn

[T56] Scala：样例类
来源：http://ld.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://dm.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://gi.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wk.521024.cn

[T58] Scala：函数定义
来源：http://oj.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wv.shxzukj.cn

[T59] Scala：循环
来源：http://al.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://ki.wgjwhj.cn

[T60] Scala：折叠
来源：http://hr.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pb.szsharing.cn

================================================================================
来源：http://hy.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://na.panjiajie.cn

================================================================================
来源：http://wj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://dw.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xt.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://ct.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xr.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://ni.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zy.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://qd.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dy.521024.cn

[U05] Py：列表去重且保序
来源：http://gg.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://yk.shxzskj.cn

[U06] Py：合并两个字典
来源：http://xi.huixiangedu.cn

{**a, **b}
来源：http://ns.szxytkj.cn

[U07] Py：反转字典键值
来源：http://bq.hnjuh.cn

{v: k for k, v in d.items()}
来源：http://uv.gzmigu.cn

[U08] Py：展平二维列表
来源：http://lq.521024.cn

[y for x in nested for y in x]
来源：http://fc.asd995.cn

[U09] Py：字典取最大值的键
来源：http://uz.haigaiapp.cn

max(d, key=d.get)
来源：http://nz.521024.cn

[U10] Py：按值排序字典
来源：http://gn.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nr.newstarts.cn

[U11] Py：生成器表达式
来源：http://ci.nszjky.cn

(x * 2 for x in arr)
来源：http://de.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uy.shxzukj.cn

Counter(arr).most_common(3)
来源：http://pm.panjiajie.cn

[U13] Py：固定长度队列
来源：http://nu.nszjky.cn

deque(maxlen=10)
来源：http://pd.huanxung.cn

[U14] Py：分组收集到列表
来源：http://va.nicolike.cn

defaultdict(list)
来源：http://be.szxytkj.cn

[U15] Py：高精度计时
来源：http://li.shxzukj.cn

t = time.perf_counter()
来源：http://mr.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://st.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sp.haigaiapp.cn

[U17] Py：初始化日志
来源：http://wi.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://wn.asd995.cn

[U18] Py：预编译正则
来源：http://ia.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://qw.nszjky.cn

[U19] Py：正则替换带回调
来源：http://up.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sp.hahajie.cn

[U20] Py：缓存函数结果
来源：http://xb.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://bc.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://qy.huixinmuqiang.cn

@contextlib.contextmanager
来源：http://th.521024.cn

[U22] Py：矩阵转置
来源：http://fv.shtwfgs.cn

list(zip(*m))
来源：http://ix.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://nk.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oo.panjiajie.cn

[U24] Py：路径操作
来源：http://ws.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wv.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://xr.muxihuayi.cn

csv.DictReader(f)
来源：http://zw.colortex.cn

[U26] Py：并发下载
来源：http://wn.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qt.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://pv.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://iy.gzmigu.cn

[U28] Py：类型别名
来源：http://as.huixiangedu.cn

UserId = int
来源：http://il.szsharing.cn

[U29] Py：属性校验
来源：http://av.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://ga.yuntaijiaju.cn

[U30] Py：数据类
来源：http://pk.szsharing.cn

@dataclass(slots=True)
来源：http://yo.bookmarksfly.cn

[U31] Py：单测
来源：http://qx.panjiajie.cn

python -m pytest -q
来源：http://hr.haigaiapp.cn

[U32] Py：代码格式化
来源：http://hz.nszjky.cn

ruff format . && ruff check --fix .
来源：http://pg.hahajie.cn

[U33] Py：打包发布
来源：http://ve.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://he.szxytkj.cn

[U34] Py：判断编码
来源：http://zs.nicolike.cn

chardet.detect(raw)
来源：http://nn.gzmigu.cn

[U35] Py：发送邮件
来源：http://wm.nicolike.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://on.521024.cn

[U36] Py：定时任务
来源：http://yg.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://ks.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://qm.szsharing.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fz.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://ct.shxzskj.cn

Path(__file__).resolve().parent
来源：http://yx.bjjhwx.cn

[U39] Py：判断是否在交互环境
来源：http://jw.chemitech.net.cn

sys.stdout.isatty()
来源：http://zl.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://ev.521024.cn

print("err", file=sys.stderr)
来源：http://ie.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://le.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://db.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://jh.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ib.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://dh.hnjuh.cn

namespace App\Http;
来源：http://af.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://ex.nicolike.cn

declare(strict_types=1);
来源：http://gc.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://pd.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://it.szxytkj.cn

[U46] PHP：可空类型
来源：http://xd.bookmarksfly.cn

?string $name = null
来源：http://vk.colortex.cn

[U47] PHP：联合类型
来源：http://xg.hahajie.cn

int|string $id
来源：http://zz.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://uu.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mi.colortex.cn

[U49] PHP：只读属性
来源：http://oq.huanxung.cn

public readonly string $name
来源：http://kf.hnjuh.cn

[U50] PHP：构造器属性提升
来源：http://ia.yuntaijiaju.cn

public function __construct(private int $id) {}
来源：http://rb.jctech888.com.cn

[U51] PHP：数组解构
来源：http://ae.bjjhwx.cn

[$a, $b] = $arr;
来源：http://xo.hahajie.cn

[U52] PHP：箭头函数
来源：http://hd.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://gm.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://pp.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://xw.szxytkj.cn

[U54] PHP：空安全调用
来源：http://xv.lnxyls.cn

$obj?->method()
来源：http://vp.panjiajie.cn

[U55] PHP：match 表达式
来源：http://eq.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fk.gzmigu.cn

[U56] PHP：命名参数
来源：http://rv.huixiangedu.cn

f(a: 1, b: 2)
来源：http://xd.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://ok.shxzukj.cn

"值: {$a}"
来源：http://no.panjiajie.cn

[U58] PHP：数组三件套
来源：http://ny.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gx.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ck.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iz.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://er.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ia.521024.cn


<!-- 参考信息 -->