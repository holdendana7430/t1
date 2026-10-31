代发 wailian999

[S33] C++：vector 增删
来源：http://sm.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zx.colortex.cn

[S34] C++：遍历 vector
来源：http://ne.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://ln.chemitech.net.cn

[S35] C++：map
来源：http://yr.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jl.521024.cn

[S36] C++：unordered_map
来源：http://jf.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nd.shxzukj.cn

[S37] C++：set
来源：http://tk.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hh.asd995.cn

[S38] C++：排序
来源：http://th.colortex.cn

std::sort(v.begin(), v.end());
来源：http://tr.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://da.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gz.nicolike.cn

[S40] C++：查找元素
来源：http://hw.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vv.hnjuh.cn

[S41] C++：类与构造函数
来源：http://np.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ul.szsharing.cn

[S42] C++：继承与虚函数
来源：http://kr.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://gc.bjjhwx.cn

[S43] C++：智能指针
来源：http://ih.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://wz.panjiajie.cn

[S44] C++：引用传参
来源：http://gu.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://me.muxihuayi.cn

[S45] C++：lambda
来源：http://sk.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vs.9csxet.cn

[S46] C++：函数模板
来源：http://ol.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ia.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ir.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ub.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://eh.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jc.huanxung.cn

while (std::getline(in, line)) { }
来源：http://em.hahajie.cn

[S49] C++：写文件
来源：http://xu.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ll.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://ts.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gb.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://db.newstarts.cn

static_cast<double>(a) / b
来源：http://vm.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://iv.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://gw.yuexingan06.cn

[S53] C++：移动语义
来源：http://us.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://an.nicolike.cn

[S54] C++：异常处理
来源：http://hr.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jx.asd995.cn

[S55] C++：结构化绑定
来源：http://yz.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bu.huixinmuqiang.cn

[S56] C++：optional
来源：http://xn.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iq.shxzskj.cn

[S57] C++：编译期常量
来源：http://vm.panjiajie.cn

constexpr int N = 10;
来源：http://wu.9csxet.cn

[S58] C++：命名空间
来源：http://hw.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://dd.colortex.cn

[S59] C++：静态断言
来源：http://hb.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yy.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://lj.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hp.bjjhwx.cn

================================================================================
来源：http://pq.wgjwhj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fd.shxzskj.cn

================================================================================
来源：http://ch.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://zc.haigaiapp.cn

println("Hello")
来源：http://ft.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://jd.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aw.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://jl.panjiajie.cn

"值: $b"
来源：http://yd.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://ee.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://qe.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://zi.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kp.521024.cn

[T06] Kotlin：集合映射
来源：http://rl.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oa.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://wg.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yr.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://io.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://yk.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://wq.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://kv.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://zf.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fn.shxzukj.cn

[T11] Kotlin：协程
来源：http://vf.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nb.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://xh.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://jv.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://hz.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://tf.bookmarksfly.cn

[T14] Kotlin：循环
来源：http://ii.asd995.cn

for (i in 1..10) println(i)
来源：http://kq.muxihuayi.cn

[T15] Kotlin：接口
来源：http://vs.9csxet.cn

interface Shape { fun area(): Double }
来源：http://kb.colortex.cn

[T16] Swift：Hello World
来源：http://jm.jctech888.com.cn

print("Hello")
来源：http://if.huanxung.cn

[T17] Swift：变量与常量
来源：http://dx.colortex.cn

var a = 1;  let b = 2
来源：http://ra.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://pd.muxihuayi.cn

"值: \(b)"
来源：http://nd.9csxet.cn

[T19] Swift：可选绑定
来源：http://pz.asd995.cn

if let n = opt { print(n) }
来源：http://qt.panjiajie.cn

[T20] Swift：数组操作
来源：http://fw.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uu.hnjuh.cn

[T21] Swift：遍历
来源：http://ac.9csxet.cn

for x in a { print(x) }
来源：http://hf.huixinmuqiang.cn

[T22] Swift：字典
来源：http://mo.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yd.huixiangedu.cn

[T23] Swift：函数
来源：http://yk.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bp.wgjwhj.cn

[T24] Swift：闭包
来源：http://uy.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yr.bjjhwx.cn

[T25] Swift：结构体
来源：http://mg.colortex.cn

struct P { var x: Int }
来源：http://sb.bjjhwx.cn

[T26] Swift：类与重写
来源：http://xd.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://rt.newstarts.cn

[T27] Swift：错误处理
来源：http://wh.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://fy.bookmarksfly.cn

[T28] Swift：枚举
来源：http://og.muxihuayi.cn

enum Color { case red, green }
来源：http://oz.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://ox.panjiajie.cn

guard let x = opt else { return }
来源：http://fs.bjjhwx.cn

[T30] Swift：协议
来源：http://ve.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://wy.huanxung.cn

[T31] Lua：Hello World
来源：http://ns.huixinmuqiang.cn

print("Hello")
来源：http://br.gzmigu.cn

[T32] Lua：局部变量
来源：http://qa.chemitech.net.cn

local a = 1
来源：http://qj.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://ol.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ec.chemitech.net.cn

[T34] Lua：遍历表
来源：http://uj.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rj.shxzukj.cn

[T35] Lua：字典表
来源：http://hz.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://gv.asd995.cn

[T36] Lua：函数
来源：http://vw.shtwfgs.cn

function add(a, b) return a + b end
来源：http://wf.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://ro.shtwfgs.cn

"a" .. "b"
来源：http://bo.shxzskj.cn

[T38] Lua：条件
来源：http://qa.muxihuayi.cn

if x > 0 then print("正") end
来源：http://xo.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://pq.huixiangedu.cn

string.find(s, "%d+")
来源：http://cy.huixinmuqiang.cn

[T40] Lua：元表
来源：http://ap.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://ua.asd995.cn

[T41] Perl：Hello World
来源：http://wv.shxzukj.cn

print "Hello\n";
来源：http://ip.huanxung.cn

[T42] Perl：变量类型
来源：http://tl.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ot.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://td.shxzukj.cn

"值: $a"
来源：http://qf.bookmarksfly.cn

[T44] Perl：条件
来源：http://mg.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://ut.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://vu.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://hs.panjiajie.cn

[T46] Perl：哈希操作
来源：http://mm.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mk.nicolike.cn

[T47] Perl：正则捕获
来源：http://hu.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dz.szsharing.cn

[T48] Perl：正则替换
来源：http://km.hahajie.cn

$s =~ s/old/new/g;
来源：http://vy.nszjky.cn

[T49] Perl：函数
来源：http://ww.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bn.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://uz.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.szsharing.cn

while (my $line = <$fh>) { print $line; }
来源：http://ft.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://sz.jctech888.com.cn

println("Hello")
来源：http://hc.shxzskj.cn

[T52] Scala：变量
来源：http://wk.shxzukj.cn

val a = 1;  var b = 2
来源：http://qu.asd995.cn

[T53] Scala：字符串插值
来源：http://is.gzmigu.cn

s"值: $b"
来源：http://um.hnjuh.cn

[T54] Scala：集合映射
来源：http://cf.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://yi.gzmigu.cn

[T55] Scala：集合过滤
来源：http://rw.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cf.lnxyls.cn

[T56] Scala：样例类
来源：http://pl.yuexingan06.cn

case class User(name: String, age: Int)
来源：http://hh.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://sv.shtwfgs.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fl.wgjwhj.cn

[T58] Scala：函数定义
来源：http://dg.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ua.muxihuayi.cn

[T59] Scala：循环
来源：http://kc.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://ia.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://aw.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rc.colortex.cn

================================================================================
来源：http://em.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://si.szxytkj.cn

================================================================================
来源：http://ly.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://oj.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yu.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://gd.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://am.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://fe.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pv.huanxung.cn

[U04] Py：变量调试打印
来源：http://uy.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://re.yuexingan06.cn

[U05] Py：列表去重且保序
来源：http://nk.nicolike.cn

list(dict.fromkeys(arr))
来源：http://nu.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://cf.shxzukj.cn

{**a, **b}
来源：http://yp.nicolike.cn

[U07] Py：反转字典键值
来源：http://gm.gzmigu.cn

{v: k for k, v in d.items()}
来源：http://mf.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://sq.nszjky.cn

[y for x in nested for y in x]
来源：http://hq.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://pi.521024.cn

max(d, key=d.get)
来源：http://lw.nicolike.cn

[U10] Py：按值排序字典
来源：http://ia.asd995.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dy.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://dg.szsharing.cn

(x * 2 for x in arr)
来源：http://sq.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ws.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://cg.szsharing.cn

[U13] Py：固定长度队列
来源：http://lj.bookmarksfly.cn

deque(maxlen=10)
来源：http://jb.colortex.cn

[U14] Py：分组收集到列表
来源：http://or.shxzskj.cn

defaultdict(list)
来源：http://mz.szxytkj.cn

[U15] Py：高精度计时
来源：http://hk.gzmigu.cn

t = time.perf_counter()
来源：http://gj.jctech888.com.cn

[U16] Py：命令行参数解析
来源：http://lk.panjiajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hi.panjiajie.cn

[U17] Py：初始化日志
来源：http://yi.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://og.huixiangedu.cn

[U18] Py：预编译正则
来源：http://lf.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://ir.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://zf.newstarts.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pn.panjiajie.cn

[U20] Py：缓存函数结果
来源：http://uq.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://eg.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://sc.yuexingan06.cn

@contextlib.contextmanager
来源：http://jq.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://sw.muxihuayi.cn

list(zip(*m))
来源：http://go.asd995.cn

[U23] Py：分块读取大文件
来源：http://tb.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kk.lnxyls.cn

[U24] Py：路径操作
来源：http://ap.huanxung.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qz.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ht.hnjuh.cn

csv.DictReader(f)
来源：http://vd.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://ke.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://db.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://bm.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qc.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://ha.yuntaijiaju.cn

UserId = int
来源：http://np.9csxet.cn

[U29] Py：属性校验
来源：http://ww.huanxung.cn

@property 与 @x.setter 配合
来源：http://dk.panjiajie.cn

[U30] Py：数据类
来源：http://ij.muxihuayi.cn

@dataclass(slots=True)
来源：http://tx.shxzukj.cn

[U31] Py：单测
来源：http://dc.newstarts.cn

python -m pytest -q
来源：http://sn.nszjky.cn

[U32] Py：代码格式化
来源：http://ql.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://rt.colortex.cn

[U33] Py：打包发布
来源：http://gp.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ut.haigaiapp.cn

[U34] Py：判断编码
来源：http://jx.muxihuayi.cn

chardet.detect(raw)
来源：http://gp.shxzukj.cn

[U35] Py：发送邮件
来源：http://uu.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wn.shxzskj.cn

[U36] Py：定时任务
来源：http://ep.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://jk.shxzskj.cn

[U37] Py：读写 Excel
来源：http://va.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jv.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://wu.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://of.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://lc.haigaiapp.cn

sys.stdout.isatty()
来源：http://gt.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://vk.asd995.cn

print("err", file=sys.stderr)
来源：http://sm.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://cb.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jh.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://gl.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zx.asd995.cn

[U43] PHP：声明命名空间
来源：http://mw.hahajie.cn

namespace App\Http;
来源：http://do.szsharing.cn

[U44] PHP：开启严格类型
来源：http://cq.yuexingan06.cn

declare(strict_types=1);
来源：http://mp.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://wy.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wz.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://pm.newstarts.cn

?string $name = null
来源：http://rb.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://gj.haigaiapp.cn

int|string $id
来源：http://cp.newstarts.cn

[U48] PHP：纯枚举
来源：http://sc.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rm.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://gh.bookmarksfly.cn

public readonly string $name
来源：http://lc.521024.cn

[U50] PHP：构造器属性提升
来源：http://vx.nicolike.cn

public function __construct(private int $id) {}
来源：http://iv.lnxyls.cn

[U51] PHP：数组解构
来源：http://ds.colortex.cn

[$a, $b] = $arr;
来源：http://vi.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ty.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://di.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://hz.yuexingan06.cn

$v = $a ?? $b ?? "default";
来源：http://ec.yuexingan06.cn

[U54] PHP：空安全调用
来源：http://zk.shtwfgs.cn

$obj?->method()
来源：http://ns.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://mg.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xu.haigaiapp.cn

[U56] PHP：命名参数
来源：http://us.huixiangedu.cn

f(a: 1, b: 2)
来源：http://hb.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://wn.yuntaijiaju.cn

"值: {$a}"
来源：http://gr.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://nk.hnjuh.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tq.521024.cn


<!-- 参考信息 -->