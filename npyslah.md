代发 wailian999

[S33] C++：vector 增删
来源：http://yl.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ew.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ss.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://pe.szxytkj.cn

[S35] C++：map
来源：http://qn.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dn.huixiangedu.cn

[S36] C++：unordered_map
来源：http://lr.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xe.521024.cn

[S37] C++：set
来源：http://ob.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vi.huixinmuqiang.cn

[S38] C++：排序
来源：http://vn.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://sz.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://ia.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://js.521024.cn

[S40] C++：查找元素
来源：http://nn.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nj.521024.cn

[S41] C++：类与构造函数
来源：http://ev.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ut.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://oq.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://rh.newstarts.cn

[S43] C++：智能指针
来源：http://jm.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://nh.nicolike.cn

[S44] C++：引用传参
来源：http://vb.colortex.cn

void inc(int &x) { ++x; }
来源：http://mf.521024.cn

[S45] C++：lambda
来源：http://bs.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nw.bjjhwx.cn

[S46] C++：函数模板
来源：http://ct.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kd.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://xo.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://em.gzmigu.cn

[S48] C++：逐行读文件
来源：http://hd.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gc.szsharing.cn

while (std::getline(in, line)) { }
来源：http://ic.hahajie.cn

[S49] C++：写文件
来源：http://sd.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sa.colortex.cn

[S50] C++：格式化数字
来源：http://ya.bookmarksfly.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ss.shxzskj.cn

[S51] C++：显式类型转换
来源：http://ym.bjjhwx.cn

static_cast<double>(a) / b
来源：http://zm.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://jk.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://oe.jctech888.com.cn

[S53] C++：移动语义
来源：http://gr.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://bd.chemitech.net.cn

[S54] C++：异常处理
来源：http://kk.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uo.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://qp.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pe.asd995.cn

[S56] C++：optional
来源：http://wo.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bs.szxytkj.cn

[S57] C++：编译期常量
来源：http://fn.lnxyls.cn

constexpr int N = 10;
来源：http://cd.wgjwhj.cn

[S58] C++：命名空间
来源：http://yy.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://rv.521024.cn

[S59] C++：静态断言
来源：http://gi.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tk.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://uu.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://id.wgjwhj.cn

================================================================================
来源：http://wy.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://as.panjiajie.cn

================================================================================
来源：http://lf.nszjky.cn

[T01] Kotlin：Hello World
来源：http://vh.szxytkj.cn

println("Hello")
来源：http://ps.szxytkj.cn

[T02] Kotlin：变量
来源：http://wx.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ju.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://nr.shxzskj.cn

"值: $b"
来源：http://bk.newstarts.cn

[T04] Kotlin：空安全
来源：http://dd.lnxyls.cn

val n: String? = null;  n?.length
来源：http://om.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://wk.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ph.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://fj.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yc.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://wl.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wx.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ta.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://np.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://yi.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://vc.szsharing.cn

[T10] Kotlin：默认参数
来源：http://nk.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xe.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://ef.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xq.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://jl.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://lb.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://im.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://cx.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://nt.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://rc.yuntaijiaju.cn

[T15] Kotlin：接口
来源：http://uj.nszjky.cn

interface Shape { fun area(): Double }
来源：http://ts.hahajie.cn

[T16] Swift：Hello World
来源：http://wo.521024.cn

print("Hello")
来源：http://nu.nicolike.cn

[T17] Swift：变量与常量
来源：http://go.hahajie.cn

var a = 1;  let b = 2
来源：http://bp.szxytkj.cn

[T18] Swift：字符串插值
来源：http://yg.shxzukj.cn

"值: \(b)"
来源：http://xx.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://rt.nicolike.cn

if let n = opt { print(n) }
来源：http://ce.muxihuayi.cn

[T20] Swift：数组操作
来源：http://jt.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ad.nicolike.cn

[T21] Swift：遍历
来源：http://qg.shtwfgs.cn

for x in a { print(x) }
来源：http://fz.gzmigu.cn

[T22] Swift：字典
来源：http://ig.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vl.nicolike.cn

[T23] Swift：函数
来源：http://kx.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qd.yuexingan06.cn

[T24] Swift：闭包
来源：http://da.huixiangedu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ap.jctech888.com.cn

[T25] Swift：结构体
来源：http://gw.521024.cn

struct P { var x: Int }
来源：http://op.colortex.cn

[T26] Swift：类与重写
来源：http://vq.shxzukj.cn

class A: Base { override func f() {} }
来源：http://sx.colortex.cn

[T27] Swift：错误处理
来源：http://nr.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://ca.9csxet.cn

[T28] Swift：枚举
来源：http://rs.9csxet.cn

enum Color { case red, green }
来源：http://dw.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://pb.chemitech.net.cn

guard let x = opt else { return }
来源：http://lf.shxzskj.cn

[T30] Swift：协议
来源：http://mk.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://he.nicolike.cn

[T31] Lua：Hello World
来源：http://td.colortex.cn

print("Hello")
来源：http://rj.haigaiapp.cn

[T32] Lua：局部变量
来源：http://ax.nszjky.cn

local a = 1
来源：http://gv.panjiajie.cn

[T33] Lua：表（数组）
来源：http://nd.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xp.colortex.cn

[T34] Lua：遍历表
来源：http://xu.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wn.colortex.cn

[T35] Lua：字典表
来源：http://om.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://at.lnxyls.cn

[T36] Lua：函数
来源：http://jz.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://sg.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://cm.521024.cn

"a" .. "b"
来源：http://cn.521024.cn

[T38] Lua：条件
来源：http://vv.shxzukj.cn

if x > 0 then print("正") end
来源：http://ze.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://zw.hahajie.cn

string.find(s, "%d+")
来源：http://iq.asd995.cn

[T40] Lua：元表
来源：http://st.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://rw.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://nt.colortex.cn

print "Hello\n";
来源：http://wd.muxihuayi.cn

[T42] Perl：变量类型
来源：http://sj.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nv.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://ub.gzmigu.cn

"值: $a"
来源：http://ab.szxytkj.cn

[T44] Perl：条件
来源：http://lh.asd995.cn

if ($a > 0) { print "正"; }
来源：http://kd.huanxung.cn

[T45] Perl：数组遍历
来源：http://mc.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://ri.hahajie.cn

[T46] Perl：哈希操作
来源：http://bs.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://om.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://ro.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hj.gzmigu.cn

[T48] Perl：正则替换
来源：http://oo.shxzukj.cn

$s =~ s/old/new/g;
来源：http://sz.hnjuh.cn

[T49] Perl：函数
来源：http://ju.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pu.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://fq.muxihuayi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wv.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://ef.hahajie.cn

[T51] Scala：Hello World
来源：http://de.yuntaijiaju.cn

println("Hello")
来源：http://jy.szxytkj.cn

[T52] Scala：变量
来源：http://ny.jctech888.com.cn

val a = 1;  var b = 2
来源：http://mv.newstarts.cn

[T53] Scala：字符串插值
来源：http://at.chemitech.net.cn

s"值: $b"
来源：http://xf.nicolike.cn

[T54] Scala：集合映射
来源：http://av.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://qz.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://dj.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jq.haigaiapp.cn

[T56] Scala：样例类
来源：http://wq.colortex.cn

case class User(name: String, age: Int)
来源：http://ib.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://cy.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ec.shxzskj.cn

[T58] Scala：函数定义
来源：http://wb.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dn.newstarts.cn

[T59] Scala：循环
来源：http://na.yuexingan06.cn

for (i <- 1 to 10) println(i)
来源：http://ku.hahajie.cn

[T60] Scala：折叠
来源：http://af.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://be.asd995.cn

================================================================================
来源：http://kw.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://te.hahajie.cn

================================================================================
来源：http://ac.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://ov.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tk.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://gv.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fq.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://cw.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hj.lnxyls.cn

[U04] Py：变量调试打印
来源：http://jb.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qz.nicolike.cn

[U05] Py：列表去重且保序
来源：http://ob.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://dv.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://mw.jianghongdianzi.cn

{**a, **b}
来源：http://iu.lnxyls.cn

[U07] Py：反转字典键值
来源：http://mz.nszjky.cn

{v: k for k, v in d.items()}
来源：http://rf.newstarts.cn

[U08] Py：展平二维列表
来源：http://dj.yuexingan06.cn

[y for x in nested for y in x]
来源：http://uo.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://rc.chemitech.net.cn

max(d, key=d.get)
来源：http://ug.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://fn.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ik.lnxyls.cn

[U11] Py：生成器表达式
来源：http://wc.hahajie.cn

(x * 2 for x in arr)
来源：http://pv.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wh.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://ac.asd995.cn

[U13] Py：固定长度队列
来源：http://tb.newstarts.cn

deque(maxlen=10)
来源：http://os.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://mi.bookmarksfly.cn

defaultdict(list)
来源：http://zv.521024.cn

[U15] Py：高精度计时
来源：http://ek.gzmigu.cn

t = time.perf_counter()
来源：http://ro.yuntaijiaju.cn

[U16] Py：命令行参数解析
来源：http://na.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dw.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://pb.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://qe.521024.cn

[U18] Py：预编译正则
来源：http://hc.chemitech.net.cn

pat = re.compile(r"\d+")
来源：http://mz.newstarts.cn

[U19] Py：正则替换带回调
来源：http://mf.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xi.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://kt.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://oy.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://vz.huanxung.cn

@contextlib.contextmanager
来源：http://uw.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://as.shxzskj.cn

list(zip(*m))
来源：http://al.newstarts.cn

[U23] Py：分块读取大文件
来源：http://ah.shtwfgs.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zn.nszjky.cn

[U24] Py：路径操作
来源：http://vn.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hf.newstarts.cn

[U25] Py：CSV 按字典读
来源：http://ww.hnjuh.cn

csv.DictReader(f)
来源：http://zi.nicolike.cn

[U26] Py：并发下载
来源：http://nj.muxihuayi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pr.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://zd.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://lv.huixiangedu.cn

[U28] Py：类型别名
来源：http://mc.shtwfgs.cn

UserId = int
来源：http://no.nszjky.cn

[U29] Py：属性校验
来源：http://nq.huanxung.cn

@property 与 @x.setter 配合
来源：http://pc.jianghongdianzi.cn

[U30] Py：数据类
来源：http://ey.nicolike.cn

@dataclass(slots=True)
来源：http://km.wgjwhj.cn

[U31] Py：单测
来源：http://oq.lnxyls.cn

python -m pytest -q
来源：http://mr.muxihuayi.cn

[U32] Py：代码格式化
来源：http://yr.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://jd.bjjhwx.cn

[U33] Py：打包发布
来源：http://nj.jctech888.com.cn

python -m build  （依赖 pyproject.toml）
来源：http://xr.shtwfgs.cn

[U34] Py：判断编码
来源：http://bf.jctech888.com.cn

chardet.detect(raw)
来源：http://sn.nicolike.cn

[U35] Py：发送邮件
来源：http://wj.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://il.bjjhwx.cn

[U36] Py：定时任务
来源：http://ik.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://fp.nszjky.cn

[U37] Py：读写 Excel
来源：http://xn.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://to.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://qd.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://uj.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://rv.hnjuh.cn

sys.stdout.isatty()
来源：http://oe.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ou.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://mj.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://je.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jl.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://fi.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://un.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://ep.hahajie.cn

namespace App\Http;
来源：http://tl.9csxet.cn

[U44] PHP：开启严格类型
来源：http://dh.9csxet.cn

declare(strict_types=1);
来源：http://ir.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://fa.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nm.haigaiapp.cn

[U46] PHP：可空类型
来源：http://re.hnjuh.cn

?string $name = null
来源：http://ag.lnxyls.cn

[U47] PHP：联合类型
来源：http://ru.colortex.cn

int|string $id
来源：http://bp.panjiajie.cn

[U48] PHP：纯枚举
来源：http://td.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jg.lnxyls.cn

[U49] PHP：只读属性
来源：http://rz.yuntaijiaju.cn

public readonly string $name
来源：http://fo.521024.cn

[U50] PHP：构造器属性提升
来源：http://gq.shxzskj.cn

public function __construct(private int $id) {}
来源：http://dv.szsharing.cn

[U51] PHP：数组解构
来源：http://hr.wgjwhj.cn

[$a, $b] = $arr;
来源：http://ai.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://ds.huixinmuqiang.cn

$double = fn($x) => $x * 2;
来源：http://ug.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://yt.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://ap.szsharing.cn

[U54] PHP：空安全调用
来源：http://ha.shxzskj.cn

$obj?->method()
来源：http://ss.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://bb.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ev.bookmarksfly.cn

[U56] PHP：命名参数
来源：http://rz.yuexingan06.cn

f(a: 1, b: 2)
来源：http://jg.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://nq.hnjuh.cn

"值: {$a}"
来源：http://cs.colortex.cn

[U58] PHP：数组三件套
来源：http://ni.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ye.jctech888.com.cn


<!-- 参考信息 -->