代发 wailian999

[S33] C++：vector 增删
来源：http://mb.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zv.szsharing.cn

[S34] C++：遍历 vector
来源：http://gu.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://um.colortex.cn

[S35] C++：map
来源：http://zj.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pn.shxzskj.cn

[S36] C++：unordered_map
来源：http://fa.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oi.yuntaijiaju.cn

[S37] C++：set
来源：http://qn.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://is.jctech888.com.cn

[S38] C++：排序
来源：http://sh.521024.cn

std::sort(v.begin(), v.end());
来源：http://ku.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://yd.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ev.shxzskj.cn

[S40] C++：查找元素
来源：http://wo.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xh.panjiajie.cn

[S41] C++：类与构造函数
来源：http://gd.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ei.newstarts.cn

[S42] C++：继承与虚函数
来源：http://hr.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://kr.newstarts.cn

[S43] C++：智能指针
来源：http://pi.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://wi.shxzskj.cn

[S44] C++：引用传参
来源：http://se.9csxet.cn

void inc(int &x) { ++x; }
来源：http://wm.yuntaijiaju.cn

[S45] C++：lambda
来源：http://ur.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zq.wgjwhj.cn

[S46] C++：函数模板
来源：http://rz.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tx.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://di.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://af.hahajie.cn

[S48] C++：逐行读文件
来源：http://jv.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cc.colortex.cn

while (std::getline(in, line)) { }
来源：http://ka.panjiajie.cn

[S49] C++：写文件
来源：http://rv.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vs.shxzukj.cn

[S50] C++：格式化数字
来源：http://vz.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ux.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://yj.asd995.cn

static_cast<double>(a) / b
来源：http://xs.shxzukj.cn

[S52] C++：const 与 noexcept
来源：http://tg.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://uz.huanxung.cn

[S53] C++：移动语义
来源：http://bn.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://rh.asd995.cn

[S54] C++：异常处理
来源：http://dp.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qo.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://dd.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zm.newstarts.cn

[S56] C++：optional
来源：http://wc.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yu.wgjwhj.cn

[S57] C++：编译期常量
来源：http://vz.jianghongdianzi.cn

constexpr int N = 10;
来源：http://ni.huixiangedu.cn

[S58] C++：命名空间
来源：http://xi.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://xi.nicolike.cn

[S59] C++：静态断言
来源：http://bl.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cb.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://rl.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wb.nicolike.cn

================================================================================
来源：http://gg.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oz.shxzukj.cn

================================================================================
来源：http://lo.huanxung.cn

[T01] Kotlin：Hello World
来源：http://ct.nicolike.cn

println("Hello")
来源：http://yy.jctech888.com.cn

[T02] Kotlin：变量
来源：http://uc.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yd.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://rs.bookmarksfly.cn

"值: $b"
来源：http://ud.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://qh.shxzskj.cn

val n: String? = null;  n?.length
来源：http://jj.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://um.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rg.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://ac.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vk.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://nc.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tt.colortex.cn

[T08] Kotlin：数据类
来源：http://mw.521024.cn

data class User(val name: String, val age: Int)
来源：http://zy.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://mf.asd995.cn

fun String.exclaim() = this + "!"
来源：http://bl.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://ad.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wf.muxihuayi.cn

[T11] Kotlin：协程
来源：http://ac.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zh.szsharing.cn

[T12] Kotlin：解构声明
来源：http://gc.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://fn.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://lh.9csxet.cn

val m = mapOf("a" to 1)
来源：http://ct.9csxet.cn

[T14] Kotlin：循环
来源：http://tg.wgjwhj.cn

for (i in 1..10) println(i)
来源：http://df.chemitech.net.cn

[T15] Kotlin：接口
来源：http://qc.hahajie.cn

interface Shape { fun area(): Double }
来源：http://sb.szsharing.cn

[T16] Swift：Hello World
来源：http://qs.huixiangedu.cn

print("Hello")
来源：http://wd.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://xl.panjiajie.cn

var a = 1;  let b = 2
来源：http://da.szsharing.cn

[T18] Swift：字符串插值
来源：http://oa.521024.cn

"值: \(b)"
来源：http://nm.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://er.szsharing.cn

if let n = opt { print(n) }
来源：http://tj.nszjky.cn

[T20] Swift：数组操作
来源：http://yz.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bk.9csxet.cn

[T21] Swift：遍历
来源：http://ue.szsharing.cn

for x in a { print(x) }
来源：http://ui.szsharing.cn

[T22] Swift：字典
来源：http://hl.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gj.colortex.cn

[T23] Swift：函数
来源：http://zx.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xb.shxzukj.cn

[T24] Swift：闭包
来源：http://vl.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qf.asd995.cn

[T25] Swift：结构体
来源：http://dt.panjiajie.cn

struct P { var x: Int }
来源：http://es.jctech888.com.cn

[T26] Swift：类与重写
来源：http://fk.colortex.cn

class A: Base { override func f() {} }
来源：http://sf.chemitech.net.cn

[T27] Swift：错误处理
来源：http://qd.nicolike.cn

do { try f() } catch { print(error) }
来源：http://ri.nszjky.cn

[T28] Swift：枚举
来源：http://tz.hnjuh.cn

enum Color { case red, green }
来源：http://qv.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://cz.gzmigu.cn

guard let x = opt else { return }
来源：http://pg.colortex.cn

[T30] Swift：协议
来源：http://ti.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://ie.panjiajie.cn

[T31] Lua：Hello World
来源：http://ax.shxzskj.cn

print("Hello")
来源：http://fn.hnjuh.cn

[T32] Lua：局部变量
来源：http://jz.huanxung.cn

local a = 1
来源：http://jc.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://df.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hb.hnjuh.cn

[T34] Lua：遍历表
来源：http://li.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zz.jctech888.com.cn

[T35] Lua：字典表
来源：http://wp.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://xh.jianghongdianzi.cn

[T36] Lua：函数
来源：http://de.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://hd.asd995.cn

[T37] Lua：字符串拼接
来源：http://sk.nicolike.cn

"a" .. "b"
来源：http://mh.jianghongdianzi.cn

[T38] Lua：条件
来源：http://pm.jctech888.com.cn

if x > 0 then print("正") end
来源：http://yt.nicolike.cn

[T39] Lua：模式匹配
来源：http://ei.szxytkj.cn

string.find(s, "%d+")
来源：http://mo.wgjwhj.cn

[T40] Lua：元表
来源：http://ck.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://td.szsharing.cn

[T41] Perl：Hello World
来源：http://hl.newstarts.cn

print "Hello\n";
来源：http://dc.chemitech.net.cn

[T42] Perl：变量类型
来源：http://fm.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yf.szsharing.cn

[T43] Perl：字符串插值
来源：http://oo.colortex.cn

"值: $a"
来源：http://sg.yuexingan06.cn

[T44] Perl：条件
来源：http://qt.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://vv.panjiajie.cn

[T45] Perl：数组遍历
来源：http://rf.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://tt.521024.cn

[T46] Perl：哈希操作
来源：http://ec.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xh.shxzskj.cn

[T47] Perl：正则捕获
来源：http://us.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rv.shxzukj.cn

[T48] Perl：正则替换
来源：http://vi.521024.cn

$s =~ s/old/new/g;
来源：http://oq.nicolike.cn

[T49] Perl：函数
来源：http://dl.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vf.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://kh.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eb.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://fb.huixiangedu.cn

[T51] Scala：Hello World
来源：http://kv.newstarts.cn

println("Hello")
来源：http://fn.muxihuayi.cn

[T52] Scala：变量
来源：http://vb.newstarts.cn

val a = 1;  var b = 2
来源：http://rz.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://xs.yuexingan06.cn

s"值: $b"
来源：http://pf.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://of.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://wd.szsharing.cn

[T55] Scala：集合过滤
来源：http://dc.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xm.9csxet.cn

[T56] Scala：样例类
来源：http://nb.9csxet.cn

case class User(name: String, age: Int)
来源：http://eu.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://mf.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xk.colortex.cn

[T58] Scala：函数定义
来源：http://zv.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bx.bookmarksfly.cn

[T59] Scala：循环
来源：http://lq.bjjhwx.cn

for (i <- 1 to 10) println(i)
来源：http://on.shxzukj.cn

[T60] Scala：折叠
来源：http://nd.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xh.521024.cn

================================================================================
来源：http://do.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://li.asd995.cn

================================================================================
来源：http://gq.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://eg.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bo.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://yk.huixinmuqiang.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://em.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://bk.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sd.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://yu.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gg.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://rl.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://xd.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://on.asd995.cn

{**a, **b}
来源：http://cy.hnjuh.cn

[U07] Py：反转字典键值
来源：http://ec.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://mp.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://fd.chemitech.net.cn

[y for x in nested for y in x]
来源：http://tg.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://qv.hahajie.cn

max(d, key=d.get)
来源：http://uc.shxzukj.cn

[U10] Py：按值排序字典
来源：http://zm.newstarts.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vb.hahajie.cn

[U11] Py：生成器表达式
来源：http://bp.nszjky.cn

(x * 2 for x in arr)
来源：http://oa.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tl.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://om.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://se.gzmigu.cn

deque(maxlen=10)
来源：http://ko.huanxung.cn

[U14] Py：分组收集到列表
来源：http://vs.huixinmuqiang.cn

defaultdict(list)
来源：http://uy.shtwfgs.cn

[U15] Py：高精度计时
来源：http://ds.asd995.cn

t = time.perf_counter()
来源：http://lx.huixiangedu.cn

[U16] Py：命令行参数解析
来源：http://za.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oy.521024.cn

[U17] Py：初始化日志
来源：http://rb.lnxyls.cn

logging.basicConfig(level=logging.INFO)
来源：http://ee.lnxyls.cn

[U18] Py：预编译正则
来源：http://fk.newstarts.cn

pat = re.compile(r"\d+")
来源：http://qn.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://dy.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dh.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://en.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://tr.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://ol.shxzukj.cn

@contextlib.contextmanager
来源：http://ca.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://hg.hnjuh.cn

list(zip(*m))
来源：http://of.bookmarksfly.cn

[U23] Py：分块读取大文件
来源：http://gb.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nt.bjjhwx.cn

[U24] Py：路径操作
来源：http://ql.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gc.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://rp.szsharing.cn

csv.DictReader(f)
来源：http://rb.nicolike.cn

[U26] Py：并发下载
来源：http://dy.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kg.huanxung.cn

[U27] Py：异步 HTTP
来源：http://px.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://po.huanxung.cn

[U28] Py：类型别名
来源：http://pc.shxzukj.cn

UserId = int
来源：http://ib.asd995.cn

[U29] Py：属性校验
来源：http://yh.szsharing.cn

@property 与 @x.setter 配合
来源：http://pf.huixinmuqiang.cn

[U30] Py：数据类
来源：http://td.panjiajie.cn

@dataclass(slots=True)
来源：http://rt.nszjky.cn

[U31] Py：单测
来源：http://vj.szsharing.cn

python -m pytest -q
来源：http://qn.panjiajie.cn

[U32] Py：代码格式化
来源：http://to.nicolike.cn

ruff format . && ruff check --fix .
来源：http://jg.lnxyls.cn

[U33] Py：打包发布
来源：http://ud.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://ye.nicolike.cn

[U34] Py：判断编码
来源：http://tz.hahajie.cn

chardet.detect(raw)
来源：http://kw.shxzukj.cn

[U35] Py：发送邮件
来源：http://fg.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sd.bjjhwx.cn

[U36] Py：定时任务
来源：http://os.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://js.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://rx.panjiajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xu.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://zk.panjiajie.cn

Path(__file__).resolve().parent
来源：http://ng.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://bh.haigaiapp.cn

sys.stdout.isatty()
来源：http://wk.colortex.cn

[U40] Py：打印到标准错误
来源：http://ax.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://tu.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://am.huixinmuqiang.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dz.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://ph.yuexingan06.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tc.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://km.lnxyls.cn

namespace App\Http;
来源：http://ib.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://rm.bjjhwx.cn

declare(strict_types=1);
来源：http://oi.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://ql.hahajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sz.521024.cn

[U46] PHP：可空类型
来源：http://hs.szsharing.cn

?string $name = null
来源：http://pp.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://se.nicolike.cn

int|string $id
来源：http://wk.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://so.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gc.asd995.cn

[U49] PHP：只读属性
来源：http://ep.lnxyls.cn

public readonly string $name
来源：http://oc.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://zy.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://as.newstarts.cn

[U51] PHP：数组解构
来源：http://mf.nicolike.cn

[$a, $b] = $arr;
来源：http://fb.yuntaijiaju.cn

[U52] PHP：箭头函数
来源：http://mg.szxytkj.cn

$double = fn($x) => $x * 2;
来源：http://jc.jianghongdianzi.cn

[U53] PHP：空合并运算符
来源：http://ta.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://sg.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://iq.yuntaijiaju.cn

$obj?->method()
来源：http://pt.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://sz.colortex.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nn.panjiajie.cn

[U56] PHP：命名参数
来源：http://ju.shtwfgs.cn

f(a: 1, b: 2)
来源：http://dc.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://mo.szsharing.cn

"值: {$a}"
来源：http://vo.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://gn.shtwfgs.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xg.gzmigu.cn


<!-- 参考信息 -->