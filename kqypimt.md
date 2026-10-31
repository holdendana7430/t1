代发 wailian999

[S35] C++：map
来源：http://sx.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wh.shxzskj.cn

[S36] C++：unordered_map
来源：http://ia.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aa.lnxyls.cn

[S37] C++：set
来源：http://jv.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rq.colortex.cn

[S38] C++：排序
来源：http://vd.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://ih.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://de.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yf.chemitech.net.cn

[S40] C++：查找元素
来源：http://do.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://af.lnxyls.cn

[S41] C++：类与构造函数
来源：http://qf.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gc.nicolike.cn

[S42] C++：继承与虚函数
来源：http://qg.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://so.shxzukj.cn

[S43] C++：智能指针
来源：http://so.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://zj.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://xs.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ss.shxzskj.cn

[S45] C++：lambda
来源：http://ue.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wp.szxytkj.cn

[S46] C++：函数模板
来源：http://cx.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zs.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://wm.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qw.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://nj.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gb.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://ga.panjiajie.cn

[S49] C++：写文件
来源：http://li.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pa.9csxet.cn

[S50] C++：格式化数字
来源：http://rl.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zi.huanxung.cn

[S51] C++：显式类型转换
来源：http://re.yuexingan06.cn

static_cast<double>(a) / b
来源：http://ch.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://cg.huanxung.cn

int size() const noexcept { return n_; }
来源：http://tv.chemitech.net.cn

[S53] C++：移动语义
来源：http://gf.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://bh.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://lw.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uh.gzmigu.cn

[S55] C++：结构化绑定
来源：http://bl.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ut.szsharing.cn

[S56] C++：optional
来源：http://lg.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tk.shxzukj.cn

[S57] C++：编译期常量
来源：http://qf.hahajie.cn

constexpr int N = 10;
来源：http://jn.bookmarksfly.cn

[S58] C++：命名空间
来源：http://nv.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://yf.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ii.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gw.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://wd.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yj.haigaiapp.cn

================================================================================
来源：http://ox.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vb.hnjuh.cn

================================================================================
来源：http://hj.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://de.colortex.cn

println("Hello")
来源：http://ax.shtwfgs.cn

[T02] Kotlin：变量
来源：http://gw.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wr.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://rn.szxytkj.cn

"值: $b"
来源：http://fy.shxzskj.cn

[T04] Kotlin：空安全
来源：http://uq.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://xs.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://ql.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wu.nicolike.cn

[T06] Kotlin：集合映射
来源：http://km.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zp.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://xs.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vv.gzmigu.cn

[T08] Kotlin：数据类
来源：http://et.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://it.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://du.521024.cn

fun String.exclaim() = this + "!"
来源：http://gf.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://fu.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tc.panjiajie.cn

[T11] Kotlin：协程
来源：http://bw.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qx.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://lz.haigaiapp.cn

val (a, b) = Pair(1, 2)
来源：http://gk.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://ba.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://mx.9csxet.cn

[T14] Kotlin：循环
来源：http://mv.nszjky.cn

for (i in 1..10) println(i)
来源：http://vf.chemitech.net.cn

[T15] Kotlin：接口
来源：http://xt.colortex.cn

interface Shape { fun area(): Double }
来源：http://es.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://bi.9csxet.cn

print("Hello")
来源：http://iq.gzmigu.cn

[T17] Swift：变量与常量
来源：http://zq.wgjwhj.cn

var a = 1;  let b = 2
来源：http://vk.lnxyls.cn

[T18] Swift：字符串插值
来源：http://yv.asd995.cn

"值: \(b)"
来源：http://py.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ft.huixiangedu.cn

if let n = opt { print(n) }
来源：http://fm.huixiangedu.cn

[T20] Swift：数组操作
来源：http://re.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://si.shxzskj.cn

[T21] Swift：遍历
来源：http://lh.shtwfgs.cn

for x in a { print(x) }
来源：http://eh.haigaiapp.cn

[T22] Swift：字典
来源：http://sj.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vm.asd995.cn

[T23] Swift：函数
来源：http://uk.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hj.shtwfgs.cn

[T24] Swift：闭包
来源：http://uu.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ho.lnxyls.cn

[T25] Swift：结构体
来源：http://st.hnjuh.cn

struct P { var x: Int }
来源：http://lq.521024.cn

[T26] Swift：类与重写
来源：http://sh.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://jq.szxytkj.cn

[T27] Swift：错误处理
来源：http://vj.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://xg.9csxet.cn

[T28] Swift：枚举
来源：http://yj.chemitech.net.cn

enum Color { case red, green }
来源：http://hi.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://ss.nszjky.cn

guard let x = opt else { return }
来源：http://ug.jianghongdianzi.cn

[T30] Swift：协议
来源：http://op.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://lg.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://ia.hnjuh.cn

print("Hello")
来源：http://rg.nszjky.cn

[T32] Lua：局部变量
来源：http://xg.yuntaijiaju.cn

local a = 1
来源：http://fi.newstarts.cn

[T33] Lua：表（数组）
来源：http://gh.newstarts.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kz.bjjhwx.cn

[T34] Lua：遍历表
来源：http://gc.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jc.9csxet.cn

[T35] Lua：字典表
来源：http://ya.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://ld.panjiajie.cn

[T36] Lua：函数
来源：http://bx.hahajie.cn

function add(a, b) return a + b end
来源：http://nc.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://zt.huanxung.cn

"a" .. "b"
来源：http://wa.shxzukj.cn

[T38] Lua：条件
来源：http://iu.wgjwhj.cn

if x > 0 then print("正") end
来源：http://mo.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://ue.newstarts.cn

string.find(s, "%d+")
来源：http://yy.huixiangedu.cn

[T40] Lua：元表
来源：http://nq.9csxet.cn

setmetatable({}, { __index = base })
来源：http://es.shxzskj.cn

[T41] Perl：Hello World
来源：http://bu.nszjky.cn

print "Hello\n";
来源：http://rp.colortex.cn

[T42] Perl：变量类型
来源：http://rb.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yn.szsharing.cn

[T43] Perl：字符串插值
来源：http://bb.colortex.cn

"值: $a"
来源：http://wh.yuntaijiaju.cn

[T44] Perl：条件
来源：http://ek.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://wn.szsharing.cn

[T45] Perl：数组遍历
来源：http://ok.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://oo.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://ul.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://er.shxzukj.cn

[T47] Perl：正则捕获
来源：http://pm.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://iq.nicolike.cn

[T48] Perl：正则替换
来源：http://yd.521024.cn

$s =~ s/old/new/g;
来源：http://qq.huanxung.cn

[T49] Perl：函数
来源：http://ux.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fi.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://ds.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://av.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://tj.szsharing.cn

[T51] Scala：Hello World
来源：http://yd.asd995.cn

println("Hello")
来源：http://qk.gzmigu.cn

[T52] Scala：变量
来源：http://mu.asd995.cn

val a = 1;  var b = 2
来源：http://so.huixiangedu.cn

[T53] Scala：字符串插值
来源：http://cp.huixinmuqiang.cn

s"值: $b"
来源：http://xk.9csxet.cn

[T54] Scala：集合映射
来源：http://hv.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://st.521024.cn

[T55] Scala：集合过滤
来源：http://og.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ww.newstarts.cn

[T56] Scala：样例类
来源：http://yx.hahajie.cn

case class User(name: String, age: Int)
来源：http://nv.panjiajie.cn

[T57] Scala：模式匹配
来源：http://ol.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rj.wgjwhj.cn

[T58] Scala：函数定义
来源：http://ul.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fv.huanxung.cn

[T59] Scala：循环
来源：http://kj.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://dd.9csxet.cn

[T60] Scala：折叠
来源：http://ph.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fm.lnxyls.cn

================================================================================
来源：http://rz.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hv.bookmarksfly.cn

================================================================================
来源：http://yh.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://io.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cj.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://za.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ri.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://ez.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jj.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://lb.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vc.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://hu.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://je.huanxung.cn

[U06] Py：合并两个字典
来源：http://nz.colortex.cn

{**a, **b}
来源：http://xk.nicolike.cn

[U07] Py：反转字典键值
来源：http://ks.521024.cn

{v: k for k, v in d.items()}
来源：http://qa.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://jq.huanxung.cn

[y for x in nested for y in x]
来源：http://pr.yuntaijiaju.cn

[U09] Py：字典取最大值的键
来源：http://yb.haigaiapp.cn

max(d, key=d.get)
来源：http://td.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://gr.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ll.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://ji.521024.cn

(x * 2 for x in arr)
来源：http://ap.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bl.lnxyls.cn

Counter(arr).most_common(3)
来源：http://nh.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://qy.nszjky.cn

deque(maxlen=10)
来源：http://yx.521024.cn

[U14] Py：分组收集到列表
来源：http://np.asd995.cn

defaultdict(list)
来源：http://fz.9csxet.cn

[U15] Py：高精度计时
来源：http://bt.9csxet.cn

t = time.perf_counter()
来源：http://rs.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://uq.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pw.shxzskj.cn

[U17] Py：初始化日志
来源：http://ou.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://in.nszjky.cn

[U18] Py：预编译正则
来源：http://hr.panjiajie.cn

pat = re.compile(r"\d+")
来源：http://fz.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://mj.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wu.nszjky.cn

[U20] Py：缓存函数结果
来源：http://og.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://qr.bjjhwx.cn

[U21] Py：自定义上下文管理器
来源：http://mo.bookmarksfly.cn

@contextlib.contextmanager
来源：http://cu.szsharing.cn

[U22] Py：矩阵转置
来源：http://ql.yuexingan06.cn

list(zip(*m))
来源：http://jz.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://lu.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qh.colortex.cn

[U24] Py：路径操作
来源：http://tg.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ws.colortex.cn

[U25] Py：CSV 按字典读
来源：http://wf.gzmigu.cn

csv.DictReader(f)
来源：http://gw.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://jj.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vj.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://vg.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://vl.jctech888.com.cn

[U28] Py：类型别名
来源：http://vu.huixinmuqiang.cn

UserId = int
来源：http://ii.lnxyls.cn

[U29] Py：属性校验
来源：http://ir.shxzukj.cn

@property 与 @x.setter 配合
来源：http://pr.huixinmuqiang.cn

[U30] Py：数据类
来源：http://qn.bjjhwx.cn

@dataclass(slots=True)
来源：http://dr.huanxung.cn

[U31] Py：单测
来源：http://ao.wgjwhj.cn

python -m pytest -q
来源：http://si.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://fr.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://mq.shtwfgs.cn

[U33] Py：打包发布
来源：http://nd.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://qy.shxzukj.cn

[U34] Py：判断编码
来源：http://cf.jctech888.com.cn

chardet.detect(raw)
来源：http://bs.9csxet.cn

[U35] Py：发送邮件
来源：http://ap.muxihuayi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wk.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://cz.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://xl.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://fp.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pa.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://py.colortex.cn

Path(__file__).resolve().parent
来源：http://vm.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://xc.szxytkj.cn

sys.stdout.isatty()
来源：http://fo.nszjky.cn

[U40] Py：打印到标准错误
来源：http://yy.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://of.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://bf.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oq.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://ax.521024.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fk.nicolike.cn

[U43] PHP：声明命名空间
来源：http://ab.huixinmuqiang.cn

namespace App\Http;
来源：http://ax.newstarts.cn

[U44] PHP：开启严格类型
来源：http://gj.hahajie.cn

declare(strict_types=1);
来源：http://kq.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://tf.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rf.szsharing.cn

[U46] PHP：可空类型
来源：http://ss.nszjky.cn

?string $name = null
来源：http://fo.huixiangedu.cn

[U47] PHP：联合类型
来源：http://dg.colortex.cn

int|string $id
来源：http://le.lnxyls.cn

[U48] PHP：纯枚举
来源：http://jz.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yq.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://dv.huixiangedu.cn

public readonly string $name
来源：http://hk.jianghongdianzi.cn

[U50] PHP：构造器属性提升
来源：http://bt.jctech888.com.cn

public function __construct(private int $id) {}
来源：http://sk.asd995.cn

[U51] PHP：数组解构
来源：http://kj.panjiajie.cn

[$a, $b] = $arr;
来源：http://wu.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://ie.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://or.bookmarksfly.cn

[U53] PHP：空合并运算符
来源：http://nv.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://so.521024.cn

[U54] PHP：空安全调用
来源：http://cj.colortex.cn

$obj?->method()
来源：http://sv.gzmigu.cn

[U55] PHP：match 表达式
来源：http://ik.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tv.shxzukj.cn

[U56] PHP：命名参数
来源：http://pr.asd995.cn

f(a: 1, b: 2)
来源：http://js.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://fs.bjjhwx.cn

"值: {$a}"
来源：http://qw.bookmarksfly.cn

[U58] PHP：数组三件套
来源：http://wa.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://md.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://ib.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mw.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://xj.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ss.colortex.cn


<!-- 参考信息 -->