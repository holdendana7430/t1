代发 wailian999

[S35] C++：map
来源：http://ib.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cd.asd995.cn

[S36] C++：unordered_map
来源：http://vr.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yt.hahajie.cn

[S37] C++：set
来源：http://rv.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oi.bookmarksfly.cn

[S38] C++：排序
来源：http://ff.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://eo.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://pa.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jn.9csxet.cn

[S40] C++：查找元素
来源：http://wb.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xp.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://ms.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ae.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://ly.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://lv.muxihuayi.cn

[S43] C++：智能指针
来源：http://up.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://nk.hahajie.cn

[S44] C++：引用传参
来源：http://in.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://af.bookmarksfly.cn

[S45] C++：lambda
来源：http://kf.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jj.bjjhwx.cn

[S46] C++：函数模板
来源：http://nz.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hd.521024.cn

[S47] C++：结构化绑定遍历
来源：http://wo.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ln.lnxyls.cn

[S48] C++：逐行读文件
来源：http://eo.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vt.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://zc.yuexingan06.cn

[S49] C++：写文件
来源：http://cl.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ta.haigaiapp.cn

[S50] C++：格式化数字
来源：http://vb.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fg.hnjuh.cn

[S51] C++：显式类型转换
来源：http://lz.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://sn.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://ac.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ph.shtwfgs.cn

[S53] C++：移动语义
来源：http://od.shxzukj.cn

std::vector<int> w = std::move(v);
来源：http://nf.asd995.cn

[S54] C++：异常处理
来源：http://kt.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qb.nicolike.cn

[S55] C++：结构化绑定
来源：http://tc.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fe.jctech888.com.cn

[S56] C++：optional
来源：http://gr.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ns.shxzskj.cn

[S57] C++：编译期常量
来源：http://rx.szxytkj.cn

constexpr int N = 10;
来源：http://ci.asd995.cn

[S58] C++：命名空间
来源：http://wt.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://nt.9csxet.cn

[S59] C++：静态断言
来源：http://ad.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ht.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://vt.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://da.shxzukj.cn

================================================================================
来源：http://pa.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pr.bjjhwx.cn

================================================================================
来源：http://ns.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://xy.szsharing.cn

println("Hello")
来源：http://qh.bjjhwx.cn

[T02] Kotlin：变量
来源：http://tk.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sh.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://sb.huanxung.cn

"值: $b"
来源：http://xb.szsharing.cn

[T04] Kotlin：空安全
来源：http://cu.huanxung.cn

val n: String? = null;  n?.length
来源：http://bi.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://jw.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ov.9csxet.cn

[T06] Kotlin：集合映射
来源：http://de.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://am.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ri.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dp.hnjuh.cn

[T08] Kotlin：数据类
来源：http://pt.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ud.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://ly.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://pn.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://qz.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uz.lnxyls.cn

[T11] Kotlin：协程
来源：http://go.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kw.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://mn.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://gb.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://zb.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://vt.szxytkj.cn

[T14] Kotlin：循环
来源：http://om.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://zo.9csxet.cn

[T15] Kotlin：接口
来源：http://ly.colortex.cn

interface Shape { fun area(): Double }
来源：http://oq.chemitech.net.cn

[T16] Swift：Hello World
来源：http://ma.huixiangedu.cn

print("Hello")
来源：http://jk.panjiajie.cn

[T17] Swift：变量与常量
来源：http://wa.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://ux.huanxung.cn

[T18] Swift：字符串插值
来源：http://lu.nszjky.cn

"值: \(b)"
来源：http://wq.nszjky.cn

[T19] Swift：可选绑定
来源：http://vj.bjjhwx.cn

if let n = opt { print(n) }
来源：http://we.yuexingan06.cn

[T20] Swift：数组操作
来源：http://ir.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uh.wgjwhj.cn

[T21] Swift：遍历
来源：http://gy.bjjhwx.cn

for x in a { print(x) }
来源：http://ev.9csxet.cn

[T22] Swift：字典
来源：http://cp.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jj.jianghongdianzi.cn

[T23] Swift：函数
来源：http://yk.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vd.521024.cn

[T24] Swift：闭包
来源：http://xa.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vq.szsharing.cn

[T25] Swift：结构体
来源：http://qp.szxytkj.cn

struct P { var x: Int }
来源：http://ys.szsharing.cn

[T26] Swift：类与重写
来源：http://ge.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://ci.chemitech.net.cn

[T27] Swift：错误处理
来源：http://nq.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://iq.huanxung.cn

[T28] Swift：枚举
来源：http://si.asd995.cn

enum Color { case red, green }
来源：http://tt.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://le.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://dy.shxzskj.cn

[T30] Swift：协议
来源：http://ns.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://kg.jctech888.com.cn

[T31] Lua：Hello World
来源：http://sy.huanxung.cn

print("Hello")
来源：http://me.bjjhwx.cn

[T32] Lua：局部变量
来源：http://kc.9csxet.cn

local a = 1
来源：http://um.521024.cn

[T33] Lua：表（数组）
来源：http://ch.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qw.shtwfgs.cn

[T34] Lua：遍历表
来源：http://an.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://to.colortex.cn

[T35] Lua：字典表
来源：http://jj.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://lb.colortex.cn

[T36] Lua：函数
来源：http://aq.asd995.cn

function add(a, b) return a + b end
来源：http://rv.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://zf.huixiangedu.cn

"a" .. "b"
来源：http://sk.szxytkj.cn

[T38] Lua：条件
来源：http://pe.9csxet.cn

if x > 0 then print("正") end
来源：http://xs.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://au.shxzukj.cn

string.find(s, "%d+")
来源：http://eu.huixinmuqiang.cn

[T40] Lua：元表
来源：http://yl.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://de.hahajie.cn

[T41] Perl：Hello World
来源：http://oq.huixinmuqiang.cn

print "Hello\n";
来源：http://fb.jctech888.com.cn

[T42] Perl：变量类型
来源：http://aa.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bd.asd995.cn

[T43] Perl：字符串插值
来源：http://yy.chemitech.net.cn

"值: $a"
来源：http://hb.panjiajie.cn

[T44] Perl：条件
来源：http://jw.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://wv.szxytkj.cn

[T45] Perl：数组遍历
来源：http://va.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://dr.bjjhwx.cn

[T46] Perl：哈希操作
来源：http://jb.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cv.shxzukj.cn

[T47] Perl：正则捕获
来源：http://cn.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ij.asd995.cn

[T48] Perl：正则替换
来源：http://zk.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://gh.shtwfgs.cn

[T49] Perl：函数
来源：http://oc.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jd.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://al.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gq.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://vb.shtwfgs.cn

[T51] Scala：Hello World
来源：http://wj.yuntaijiaju.cn

println("Hello")
来源：http://br.bookmarksfly.cn

[T52] Scala：变量
来源：http://ik.asd995.cn

val a = 1;  var b = 2
来源：http://bz.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://bv.hahajie.cn

s"值: $b"
来源：http://tn.shxzukj.cn

[T54] Scala：集合映射
来源：http://ee.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://xr.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://ky.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uz.shxzukj.cn

[T56] Scala：样例类
来源：http://qu.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://gl.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://el.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xh.9csxet.cn

[T58] Scala：函数定义
来源：http://jn.huanxung.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cv.szxytkj.cn

[T59] Scala：循环
来源：http://tw.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://wm.bjjhwx.cn

[T60] Scala：折叠
来源：http://wz.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gg.bookmarksfly.cn

================================================================================
来源：http://wj.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xy.haigaiapp.cn

================================================================================
来源：http://qj.521024.cn

[U01] Py：创建虚拟环境
来源：http://jy.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fb.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://yh.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hv.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://px.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ug.hahajie.cn

[U04] Py：变量调试打印
来源：http://yr.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lb.yuntaijiaju.cn

[U05] Py：列表去重且保序
来源：http://ze.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://hb.hnjuh.cn

[U06] Py：合并两个字典
来源：http://lc.wgjwhj.cn

{**a, **b}
来源：http://iq.hahajie.cn

[U07] Py：反转字典键值
来源：http://tl.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://su.nicolike.cn

[U08] Py：展平二维列表
来源：http://dh.huanxung.cn

[y for x in nested for y in x]
来源：http://xw.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ly.panjiajie.cn

max(d, key=d.get)
来源：http://st.colortex.cn

[U10] Py：按值排序字典
来源：http://ab.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zk.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://ju.gzmigu.cn

(x * 2 for x in arr)
来源：http://xz.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uk.newstarts.cn

Counter(arr).most_common(3)
来源：http://lf.nicolike.cn

[U13] Py：固定长度队列
来源：http://ol.bookmarksfly.cn

deque(maxlen=10)
来源：http://lh.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://wc.huixiangedu.cn

defaultdict(list)
来源：http://pd.jianghongdianzi.cn

[U15] Py：高精度计时
来源：http://gv.huanxung.cn

t = time.perf_counter()
来源：http://pe.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://wz.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://my.colortex.cn

[U17] Py：初始化日志
来源：http://hn.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://gh.nicolike.cn

[U18] Py：预编译正则
来源：http://iq.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://bh.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://wj.huixinmuqiang.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ws.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://ul.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://rd.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://kd.jctech888.com.cn

@contextlib.contextmanager
来源：http://yp.panjiajie.cn

[U22] Py：矩阵转置
来源：http://oz.haigaiapp.cn

list(zip(*m))
来源：http://fz.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://fc.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hc.shtwfgs.cn

[U24] Py：路径操作
来源：http://kn.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ju.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://lr.bookmarksfly.cn

csv.DictReader(f)
来源：http://jl.bjjhwx.cn

[U26] Py：并发下载
来源：http://pq.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qs.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://cg.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://al.nicolike.cn

[U28] Py：类型别名
来源：http://sh.yuntaijiaju.cn

UserId = int
来源：http://ao.lnxyls.cn

[U29] Py：属性校验
来源：http://fj.szxytkj.cn

@property 与 @x.setter 配合
来源：http://db.gzmigu.cn

[U30] Py：数据类
来源：http://qx.shxzukj.cn

@dataclass(slots=True)
来源：http://ct.lnxyls.cn

[U31] Py：单测
来源：http://wj.huixiangedu.cn

python -m pytest -q
来源：http://uf.shxzskj.cn

[U32] Py：代码格式化
来源：http://oq.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://cq.haigaiapp.cn

[U33] Py：打包发布
来源：http://qu.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://rg.colortex.cn

[U34] Py：判断编码
来源：http://jj.jctech888.com.cn

chardet.detect(raw)
来源：http://zx.huanxung.cn

[U35] Py：发送邮件
来源：http://fd.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yv.hahajie.cn

[U36] Py：定时任务
来源：http://tk.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://qg.panjiajie.cn

[U37] Py：读写 Excel
来源：http://vn.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tv.9csxet.cn

[U38] Py：获取脚本所在目录
来源：http://dm.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://yj.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://fi.hahajie.cn

sys.stdout.isatty()
来源：http://ym.521024.cn

[U40] Py：打印到标准错误
来源：http://gt.newstarts.cn

print("err", file=sys.stderr)
来源：http://ly.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ng.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ka.muxihuayi.cn

[U42] PHP：PSR-4 自动加载
来源：http://uf.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ds.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://pb.asd995.cn

namespace App\Http;
来源：http://qb.lnxyls.cn

[U44] PHP：开启严格类型
来源：http://hc.shtwfgs.cn

declare(strict_types=1);
来源：http://dy.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://yv.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://my.huixinmuqiang.cn

[U46] PHP：可空类型
来源：http://lb.colortex.cn

?string $name = null
来源：http://lk.gzmigu.cn

[U47] PHP：联合类型
来源：http://dx.newstarts.cn

int|string $id
来源：http://rr.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://ds.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gk.yuexingan06.cn

[U49] PHP：只读属性
来源：http://jj.hahajie.cn

public readonly string $name
来源：http://ma.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://ar.521024.cn

public function __construct(private int $id) {}
来源：http://vx.521024.cn

[U51] PHP：数组解构
来源：http://jc.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://qj.nszjky.cn

[U52] PHP：箭头函数
来源：http://vg.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://ka.9csxet.cn

[U53] PHP：空合并运算符
来源：http://io.nszjky.cn

$v = $a ?? $b ?? "default";
来源：http://rp.asd995.cn

[U54] PHP：空安全调用
来源：http://ej.9csxet.cn

$obj?->method()
来源：http://uu.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://ii.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xc.chemitech.net.cn

[U56] PHP：命名参数
来源：http://na.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ah.szsharing.cn

[U57] PHP：字符串插值
来源：http://wv.gzmigu.cn

"值: {$a}"
来源：http://we.hnjuh.cn

[U58] PHP：数组三件套
来源：http://nm.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vz.gzmigu.cn

[U59] PHP：自定义排序
来源：http://fs.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://co.huanxung.cn

[U60] PHP：JSON 编解码
来源：http://tm.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zl.huanxung.cn


<!-- 参考信息 -->