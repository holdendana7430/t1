代发 wailian999

[S41] C++：类与构造函数
来源：http://ux.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bo.nszjky.cn

[S42] C++：继承与虚函数
来源：http://ar.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://gv.wgjwhj.cn

[S43] C++：智能指针
来源：http://xv.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://hz.huanxung.cn

[S44] C++：引用传参
来源：http://hf.jctech888.com.cn

void inc(int &x) { ++x; }
来源：http://xd.shxzukj.cn

[S45] C++：lambda
来源：http://jb.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kn.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://be.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yv.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://oq.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dz.newstarts.cn

[S48] C++：逐行读文件
来源：http://zf.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ye.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://by.szxytkj.cn

[S49] C++：写文件
来源：http://ay.nszjky.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sz.shxzukj.cn

[S50] C++：格式化数字
来源：http://of.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mq.shxzukj.cn

[S51] C++：显式类型转换
来源：http://rw.wgjwhj.cn

static_cast<double>(a) / b
来源：http://wb.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://jj.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://pm.shxzskj.cn

[S53] C++：移动语义
来源：http://yr.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://iz.panjiajie.cn

[S54] C++：异常处理
来源：http://ua.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vk.shxzukj.cn

[S55] C++：结构化绑定
来源：http://od.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wn.lnxyls.cn

[S56] C++：optional
来源：http://pm.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ld.gzmigu.cn

[S57] C++：编译期常量
来源：http://kk.9csxet.cn

constexpr int N = 10;
来源：http://mm.haigaiapp.cn

[S58] C++：命名空间
来源：http://gr.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://ze.yuexingan06.cn

[S59] C++：静态断言
来源：http://cn.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://td.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://aj.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pl.jctech888.com.cn

================================================================================
来源：http://cc.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mo.huixiangedu.cn

================================================================================
来源：http://lf.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://bw.nszjky.cn

println("Hello")
来源：http://tt.szsharing.cn

[T02] Kotlin：变量
来源：http://rw.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qb.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://wo.9csxet.cn

"值: $b"
来源：http://tl.huanxung.cn

[T04] Kotlin：空安全
来源：http://bf.colortex.cn

val n: String? = null;  n?.length
来源：http://ii.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://yp.521024.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nn.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://jv.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kt.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://pe.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bv.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://nw.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://yk.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://ni.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://yc.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://cy.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dc.colortex.cn

[T11] Kotlin：协程
来源：http://do.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qr.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://xa.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://nb.colortex.cn

[T13] Kotlin：只读 Map
来源：http://hs.521024.cn

val m = mapOf("a" to 1)
来源：http://rf.szsharing.cn

[T14] Kotlin：循环
来源：http://dy.jctech888.com.cn

for (i in 1..10) println(i)
来源：http://tc.bjjhwx.cn

[T15] Kotlin：接口
来源：http://bb.9csxet.cn

interface Shape { fun area(): Double }
来源：http://qe.chemitech.net.cn

[T16] Swift：Hello World
来源：http://ok.521024.cn

print("Hello")
来源：http://id.asd995.cn

[T17] Swift：变量与常量
来源：http://yj.wgjwhj.cn

var a = 1;  let b = 2
来源：http://vf.lnxyls.cn

[T18] Swift：字符串插值
来源：http://zg.wgjwhj.cn

"值: \(b)"
来源：http://yo.gzmigu.cn

[T19] Swift：可选绑定
来源：http://uo.asd995.cn

if let n = opt { print(n) }
来源：http://gg.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://sn.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gq.panjiajie.cn

[T21] Swift：遍历
来源：http://hy.chemitech.net.cn

for x in a { print(x) }
来源：http://lb.yuexingan06.cn

[T22] Swift：字典
来源：http://lk.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kj.colortex.cn

[T23] Swift：函数
来源：http://fa.lnxyls.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nj.huixiangedu.cn

[T24] Swift：闭包
来源：http://at.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gb.shtwfgs.cn

[T25] Swift：结构体
来源：http://dz.yuntaijiaju.cn

struct P { var x: Int }
来源：http://hz.asd995.cn

[T26] Swift：类与重写
来源：http://fo.nicolike.cn

class A: Base { override func f() {} }
来源：http://au.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://qc.nicolike.cn

do { try f() } catch { print(error) }
来源：http://lg.yuexingan06.cn

[T28] Swift：枚举
来源：http://tp.9csxet.cn

enum Color { case red, green }
来源：http://ct.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://ee.huixiangedu.cn

guard let x = opt else { return }
来源：http://gn.yuexingan06.cn

[T30] Swift：协议
来源：http://xb.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://eg.shtwfgs.cn

[T31] Lua：Hello World
来源：http://xa.shxzskj.cn

print("Hello")
来源：http://st.wgjwhj.cn

[T32] Lua：局部变量
来源：http://kl.wgjwhj.cn

local a = 1
来源：http://kb.szxytkj.cn

[T33] Lua：表（数组）
来源：http://lp.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nm.9csxet.cn

[T34] Lua：遍历表
来源：http://oe.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kv.bjjhwx.cn

[T35] Lua：字典表
来源：http://rr.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://op.521024.cn

[T36] Lua：函数
来源：http://sr.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://kv.hahajie.cn

[T37] Lua：字符串拼接
来源：http://cz.9csxet.cn

"a" .. "b"
来源：http://hr.huixinmuqiang.cn

[T38] Lua：条件
来源：http://ex.haigaiapp.cn

if x > 0 then print("正") end
来源：http://dj.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://ak.huanxung.cn

string.find(s, "%d+")
来源：http://ma.nicolike.cn

[T40] Lua：元表
来源：http://qp.hnjuh.cn

setmetatable({}, { __index = base })
来源：http://lj.gzmigu.cn

[T41] Perl：Hello World
来源：http://kg.colortex.cn

print "Hello\n";
来源：http://gr.shxzskj.cn

[T42] Perl：变量类型
来源：http://kh.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ta.9csxet.cn

[T43] Perl：字符串插值
来源：http://sf.shtwfgs.cn

"值: $a"
来源：http://vz.bjjhwx.cn

[T44] Perl：条件
来源：http://ig.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://mz.hnjuh.cn

[T45] Perl：数组遍历
来源：http://vh.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://vb.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://ou.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qa.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://qw.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ot.yuexingan06.cn

[T48] Perl：正则替换
来源：http://ce.szxytkj.cn

$s =~ s/old/new/g;
来源：http://cl.huixinmuqiang.cn

[T49] Perl：函数
来源：http://ql.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ql.newstarts.cn

[T50] Perl：逐行读文件
来源：http://kq.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ti.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://oj.nszjky.cn

[T51] Scala：Hello World
来源：http://iu.colortex.cn

println("Hello")
来源：http://hd.jctech888.com.cn

[T52] Scala：变量
来源：http://wh.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://ce.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://hf.muxihuayi.cn

s"值: $b"
来源：http://pg.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://id.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://tv.nszjky.cn

[T55] Scala：集合过滤
来源：http://ou.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bi.shxzskj.cn

[T56] Scala：样例类
来源：http://po.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://gq.hnjuh.cn

[T57] Scala：模式匹配
来源：http://ma.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pi.nicolike.cn

[T58] Scala：函数定义
来源：http://sn.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ii.huanxung.cn

[T59] Scala：循环
来源：http://lb.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://lr.muxihuayi.cn

[T60] Scala：折叠
来源：http://sd.panjiajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nt.panjiajie.cn

================================================================================
来源：http://uv.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mn.huixinmuqiang.cn

================================================================================
来源：http://sv.huanxung.cn

[U01] Py：创建虚拟环境
来源：http://pz.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gr.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://ob.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lr.hnjuh.cn

[U03] Py：加载 .env 配置
来源：http://bc.yuntaijiaju.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ca.wgjwhj.cn

[U04] Py：变量调试打印
来源：http://bw.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xj.shxzukj.cn

[U05] Py：列表去重且保序
来源：http://bn.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://qt.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://hi.shxzukj.cn

{**a, **b}
来源：http://om.newstarts.cn

[U07] Py：反转字典键值
来源：http://zr.huanxung.cn

{v: k for k, v in d.items()}
来源：http://mp.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://dw.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://wr.asd995.cn

[U09] Py：字典取最大值的键
来源：http://si.szsharing.cn

max(d, key=d.get)
来源：http://eh.shxzukj.cn

[U10] Py：按值排序字典
来源：http://ub.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ei.huanxung.cn

[U11] Py：生成器表达式
来源：http://yi.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://yo.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nh.shtwfgs.cn

Counter(arr).most_common(3)
来源：http://tc.panjiajie.cn

[U13] Py：固定长度队列
来源：http://et.521024.cn

deque(maxlen=10)
来源：http://je.szsharing.cn

[U14] Py：分组收集到列表
来源：http://yu.asd995.cn

defaultdict(list)
来源：http://qv.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://nu.9csxet.cn

t = time.perf_counter()
来源：http://cm.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://yf.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ky.yuexingan06.cn

[U17] Py：初始化日志
来源：http://dk.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://um.gzmigu.cn

[U18] Py：预编译正则
来源：http://ii.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ss.haigaiapp.cn

[U19] Py：正则替换带回调
来源：http://ap.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://by.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://js.szxytkj.cn

@functools.lru_cache(maxsize=None)
来源：http://wi.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://fb.bookmarksfly.cn

@contextlib.contextmanager
来源：http://cf.panjiajie.cn

[U22] Py：矩阵转置
来源：http://dk.huixiangedu.cn

list(zip(*m))
来源：http://wh.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://mt.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://an.colortex.cn

[U24] Py：路径操作
来源：http://pd.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ly.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://bf.colortex.cn

csv.DictReader(f)
来源：http://zw.colortex.cn

[U26] Py：并发下载
来源：http://oq.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dz.jianghongdianzi.cn

[U27] Py：异步 HTTP
来源：http://ww.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://hz.huixinmuqiang.cn

[U28] Py：类型别名
来源：http://ff.asd995.cn

UserId = int
来源：http://hl.nicolike.cn

[U29] Py：属性校验
来源：http://sc.lnxyls.cn

@property 与 @x.setter 配合
来源：http://lu.szsharing.cn

[U30] Py：数据类
来源：http://mh.521024.cn

@dataclass(slots=True)
来源：http://up.bookmarksfly.cn

[U31] Py：单测
来源：http://ag.asd995.cn

python -m pytest -q
来源：http://be.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://lf.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://ut.chemitech.net.cn

[U33] Py：打包发布
来源：http://br.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://nq.nicolike.cn

[U34] Py：判断编码
来源：http://wr.nszjky.cn

chardet.detect(raw)
来源：http://ej.szsharing.cn

[U35] Py：发送邮件
来源：http://hi.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kq.newstarts.cn

[U36] Py：定时任务
来源：http://ts.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://xp.nicolike.cn

[U37] Py：读写 Excel
来源：http://bu.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ai.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://kh.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://so.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://qf.9csxet.cn

sys.stdout.isatty()
来源：http://kp.nicolike.cn

[U40] Py：打印到标准错误
来源：http://wt.newstarts.cn

print("err", file=sys.stderr)
来源：http://du.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://bg.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://si.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://kn.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eq.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://er.lnxyls.cn

namespace App\Http;
来源：http://ek.szsharing.cn

[U44] PHP：开启严格类型
来源：http://nc.bjjhwx.cn

declare(strict_types=1);
来源：http://kt.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://rz.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qk.muxihuayi.cn

[U46] PHP：可空类型
来源：http://dv.szsharing.cn

?string $name = null
来源：http://ap.shxzskj.cn

[U47] PHP：联合类型
来源：http://cn.asd995.cn

int|string $id
来源：http://zd.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://ds.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lj.asd995.cn

[U49] PHP：只读属性
来源：http://or.lnxyls.cn

public readonly string $name
来源：http://wu.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://ne.panjiajie.cn

public function __construct(private int $id) {}
来源：http://xk.hahajie.cn

[U51] PHP：数组解构
来源：http://ww.huanxung.cn

[$a, $b] = $arr;
来源：http://ri.szsharing.cn

[U52] PHP：箭头函数
来源：http://nx.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://tm.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://gc.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://li.colortex.cn

[U54] PHP：空安全调用
来源：http://ak.haigaiapp.cn

$obj?->method()
来源：http://fa.panjiajie.cn

[U55] PHP：match 表达式
来源：http://gf.asd995.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zu.huixiangedu.cn

[U56] PHP：命名参数
来源：http://lk.asd995.cn

f(a: 1, b: 2)
来源：http://yw.gzmigu.cn

[U57] PHP：字符串插值
来源：http://pt.hnjuh.cn

"值: {$a}"
来源：http://ic.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://yb.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dx.9csxet.cn

[U59] PHP：自定义排序
来源：http://iu.shxzskj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fi.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://bp.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cr.huixinmuqiang.cn

[U61] PHP：正则
来源：http://ey.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sk.wgjwhj.cn

[U62] PHP：日期对象
来源：http://ja.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fq.szsharing.cn

[U63] PHP：文件读写
来源：http://vi.hahajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cy.bjjhwx.cn

[U64] PHP：目录遍历
来源：http://mo.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://fw.colortex.cn

[U65] PHP：会话
来源：http://fp.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yg.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://wu.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://px.bookmarksfly.cn


<!-- 参考信息 -->