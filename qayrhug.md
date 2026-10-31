代发 wailian999

[S33] C++：vector 增删
来源：http://ad.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tl.panjiajie.cn

[S34] C++：遍历 vector
来源：http://ta.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://ah.haigaiapp.cn

[S35] C++：map
来源：http://oj.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zq.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://bt.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tl.asd995.cn

[S37] C++：set
来源：http://bh.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fu.yuexingan06.cn

[S38] C++：排序
来源：http://qx.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ep.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://bh.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ke.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://wq.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oo.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://xh.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zf.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://zi.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://bp.shxzukj.cn

[S43] C++：智能指针
来源：http://hz.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://qx.shtwfgs.cn

[S44] C++：引用传参
来源：http://pg.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://bq.huixiangedu.cn

[S45] C++：lambda
来源：http://bz.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mz.huixiangedu.cn

[S46] C++：函数模板
来源：http://qx.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://na.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://ki.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lo.panjiajie.cn

[S48] C++：逐行读文件
来源：http://dc.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oq.szsharing.cn

while (std::getline(in, line)) { }
来源：http://nq.muxihuayi.cn

[S49] C++：写文件
来源：http://lm.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hn.jctech888.com.cn

[S50] C++：格式化数字
来源：http://mn.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nx.hnjuh.cn

[S51] C++：显式类型转换
来源：http://ci.wgjwhj.cn

static_cast<double>(a) / b
来源：http://vk.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://bl.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://vm.jctech888.com.cn

[S53] C++：移动语义
来源：http://xv.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://wh.panjiajie.cn

[S54] C++：异常处理
来源：http://zs.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qv.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://wz.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ik.newstarts.cn

[S56] C++：optional
来源：http://ap.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xv.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ym.huanxung.cn

constexpr int N = 10;
来源：http://da.nszjky.cn

[S58] C++：命名空间
来源：http://hw.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://cg.szsharing.cn

[S59] C++：静态断言
来源：http://cw.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bb.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://do.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ep.newstarts.cn

================================================================================
来源：http://rz.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pj.szsharing.cn

================================================================================
来源：http://rc.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://od.nszjky.cn

println("Hello")
来源：http://ob.szsharing.cn

[T02] Kotlin：变量
来源：http://xb.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xz.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://bg.jctech888.com.cn

"值: $b"
来源：http://dr.lnxyls.cn

[T04] Kotlin：空安全
来源：http://jb.szxytkj.cn

val n: String? = null;  n?.length
来源：http://ie.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://bh.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://am.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://pp.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rf.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://to.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://et.asd995.cn

[T08] Kotlin：数据类
来源：http://vw.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://dn.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://qq.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://cp.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://nj.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vw.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://vp.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://os.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://no.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://tu.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://jy.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://ce.asd995.cn

[T14] Kotlin：循环
来源：http://pv.shxzskj.cn

for (i in 1..10) println(i)
来源：http://ga.521024.cn

[T15] Kotlin：接口
来源：http://dy.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ph.hnjuh.cn

[T16] Swift：Hello World
来源：http://qd.huanxung.cn

print("Hello")
来源：http://ip.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://uh.szxytkj.cn

var a = 1;  let b = 2
来源：http://sb.huanxung.cn

[T18] Swift：字符串插值
来源：http://rj.chemitech.net.cn

"值: \(b)"
来源：http://xy.panjiajie.cn

[T19] Swift：可选绑定
来源：http://em.9csxet.cn

if let n = opt { print(n) }
来源：http://vk.newstarts.cn

[T20] Swift：数组操作
来源：http://rr.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jx.colortex.cn

[T21] Swift：遍历
来源：http://qn.haigaiapp.cn

for x in a { print(x) }
来源：http://hw.hnjuh.cn

[T22] Swift：字典
来源：http://ru.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ie.nszjky.cn

[T23] Swift：函数
来源：http://jr.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://af.9csxet.cn

[T24] Swift：闭包
来源：http://ze.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vp.shxzskj.cn

[T25] Swift：结构体
来源：http://jz.yuexingan06.cn

struct P { var x: Int }
来源：http://ht.shxzskj.cn

[T26] Swift：类与重写
来源：http://bp.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ww.521024.cn

[T27] Swift：错误处理
来源：http://pj.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://ah.colortex.cn

[T28] Swift：枚举
来源：http://yr.szsharing.cn

enum Color { case red, green }
来源：http://is.521024.cn

[T29] Swift：guard 提前返回
来源：http://dv.bookmarksfly.cn

guard let x = opt else { return }
来源：http://yg.szsharing.cn

[T30] Swift：协议
来源：http://cq.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://js.gzmigu.cn

[T31] Lua：Hello World
来源：http://vx.wgjwhj.cn

print("Hello")
来源：http://kb.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://iv.asd995.cn

local a = 1
来源：http://ko.szxytkj.cn

[T33] Lua：表（数组）
来源：http://wt.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wk.colortex.cn

[T34] Lua：遍历表
来源：http://pu.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rs.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://ub.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://ls.lnxyls.cn

[T36] Lua：函数
来源：http://cr.huixiangedu.cn

function add(a, b) return a + b end
来源：http://tv.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://cq.jctech888.com.cn

"a" .. "b"
来源：http://dg.yuntaijiaju.cn

[T38] Lua：条件
来源：http://cq.haigaiapp.cn

if x > 0 then print("正") end
来源：http://og.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://jg.nicolike.cn

string.find(s, "%d+")
来源：http://iz.hnjuh.cn

[T40] Lua：元表
来源：http://pc.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ov.521024.cn

[T41] Perl：Hello World
来源：http://us.newstarts.cn

print "Hello\n";
来源：http://cu.colortex.cn

[T42] Perl：变量类型
来源：http://tz.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fl.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://jg.shtwfgs.cn

"值: $a"
来源：http://na.lnxyls.cn

[T44] Perl：条件
来源：http://yq.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://ne.shxzskj.cn

[T45] Perl：数组遍历
来源：http://ff.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://ax.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://ul.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qk.shxzukj.cn

[T47] Perl：正则捕获
来源：http://ns.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dm.gzmigu.cn

[T48] Perl：正则替换
来源：http://pn.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://me.szsharing.cn

[T49] Perl：函数
来源：http://bb.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ea.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://km.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yv.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://dq.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://up.lnxyls.cn

println("Hello")
来源：http://hu.lnxyls.cn

[T52] Scala：变量
来源：http://ip.newstarts.cn

val a = 1;  var b = 2
来源：http://ie.huanxung.cn

[T53] Scala：字符串插值
来源：http://tb.521024.cn

s"值: $b"
来源：http://ih.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://pl.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://dl.szxytkj.cn

[T55] Scala：集合过滤
来源：http://fz.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ml.bjjhwx.cn

[T56] Scala：样例类
来源：http://vi.huanxung.cn

case class User(name: String, age: Int)
来源：http://tj.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://no.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aw.colortex.cn

[T58] Scala：函数定义
来源：http://bq.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bb.jianghongdianzi.cn

[T59] Scala：循环
来源：http://cr.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://ni.hnjuh.cn

[T60] Scala：折叠
来源：http://ov.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zl.newstarts.cn

================================================================================
来源：http://jd.huanxung.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://db.panjiajie.cn

================================================================================
来源：http://rh.huixiangedu.cn

[U01] Py：创建虚拟环境
来源：http://rf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bm.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://xi.jianghongdianzi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ex.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://sh.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://up.newstarts.cn

[U04] Py：变量调试打印
来源：http://lu.szxytkj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zf.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://cs.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://fg.huanxung.cn

[U06] Py：合并两个字典
来源：http://rn.shxzukj.cn

{**a, **b}
来源：http://ky.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://cx.9csxet.cn

{v: k for k, v in d.items()}
来源：http://ba.colortex.cn

[U08] Py：展平二维列表
来源：http://iz.huanxung.cn

[y for x in nested for y in x]
来源：http://jd.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://yf.asd995.cn

max(d, key=d.get)
来源：http://km.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://vl.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ed.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://cu.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://fx.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mt.nszjky.cn

Counter(arr).most_common(3)
来源：http://xk.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://lg.szxytkj.cn

deque(maxlen=10)
来源：http://ce.szsharing.cn

[U14] Py：分组收集到列表
来源：http://wv.huanxung.cn

defaultdict(list)
来源：http://ug.521024.cn

[U15] Py：高精度计时
来源：http://bm.jctech888.com.cn

t = time.perf_counter()
来源：http://pe.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://xr.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vn.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://au.9csxet.cn

logging.basicConfig(level=logging.INFO)
来源：http://sv.hnjuh.cn

[U18] Py：预编译正则
来源：http://rx.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://dv.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://gz.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yr.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ai.lnxyls.cn

@functools.lru_cache(maxsize=None)
来源：http://qj.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://pv.nicolike.cn

@contextlib.contextmanager
来源：http://xj.lnxyls.cn

[U22] Py：矩阵转置
来源：http://ug.9csxet.cn

list(zip(*m))
来源：http://ia.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ta.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mp.shxzskj.cn

[U24] Py：路径操作
来源：http://ia.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ui.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://qy.asd995.cn

csv.DictReader(f)
来源：http://pb.panjiajie.cn

[U26] Py：并发下载
来源：http://pg.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qb.9csxet.cn

[U27] Py：异步 HTTP
来源：http://fg.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://hz.lnxyls.cn

[U28] Py：类型别名
来源：http://wi.huixiangedu.cn

UserId = int
来源：http://dv.shtwfgs.cn

[U29] Py：属性校验
来源：http://fq.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://qy.yuntaijiaju.cn

[U30] Py：数据类
来源：http://fe.521024.cn

@dataclass(slots=True)
来源：http://ze.nszjky.cn

[U31] Py：单测
来源：http://ub.panjiajie.cn

python -m pytest -q
来源：http://sh.wgjwhj.cn

[U32] Py：代码格式化
来源：http://nz.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://vg.asd995.cn

[U33] Py：打包发布
来源：http://uj.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://cf.chemitech.net.cn

[U34] Py：判断编码
来源：http://kw.newstarts.cn

chardet.detect(raw)
来源：http://bv.colortex.cn

[U35] Py：发送邮件
来源：http://wl.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ml.hahajie.cn

[U36] Py：定时任务
来源：http://oe.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://xp.huanxung.cn

[U37] Py：读写 Excel
来源：http://wt.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wf.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ev.haigaiapp.cn

Path(__file__).resolve().parent
来源：http://mu.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://et.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://nk.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://qj.szsharing.cn

print("err", file=sys.stderr)
来源：http://od.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://up.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rx.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://qr.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oc.gzmigu.cn

[U43] PHP：声明命名空间
来源：http://ni.asd995.cn

namespace App\Http;
来源：http://qf.nicolike.cn

[U44] PHP：开启严格类型
来源：http://yz.colortex.cn

declare(strict_types=1);
来源：http://du.lnxyls.cn

[U45] PHP：类型声明与返回类型
来源：http://oa.yuexingan06.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vm.szxytkj.cn

[U46] PHP：可空类型
来源：http://nl.yuexingan06.cn

?string $name = null
来源：http://em.gzmigu.cn

[U47] PHP：联合类型
来源：http://qd.jctech888.com.cn

int|string $id
来源：http://tz.newstarts.cn

[U48] PHP：纯枚举
来源：http://ye.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://id.newstarts.cn

[U49] PHP：只读属性
来源：http://gk.gzmigu.cn

public readonly string $name
来源：http://wt.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://df.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://om.shtwfgs.cn

[U51] PHP：数组解构
来源：http://lw.huanxung.cn

[$a, $b] = $arr;
来源：http://er.szsharing.cn

[U52] PHP：箭头函数
来源：http://xx.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://zd.newstarts.cn

[U53] PHP：空合并运算符
来源：http://fi.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://mb.hnjuh.cn

[U54] PHP：空安全调用
来源：http://yq.muxihuayi.cn

$obj?->method()
来源：http://ii.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://ux.huixiangedu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mq.szxytkj.cn

[U56] PHP：命名参数
来源：http://in.nicolike.cn

f(a: 1, b: 2)
来源：http://zd.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://hc.bjjhwx.cn

"值: {$a}"
来源：http://yq.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://ss.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dh.huanxung.cn


<!-- 参考信息 -->