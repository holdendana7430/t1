代发 wailian999

[S35] C++：map
来源：http://jh.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://st.nicolike.cn

[S36] C++：unordered_map
来源：http://zw.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zt.chemitech.net.cn

[S37] C++：set
来源：http://pi.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://de.asd995.cn

[S38] C++：排序
来源：http://vw.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://gb.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://ru.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qf.gzmigu.cn

[S40] C++：查找元素
来源：http://fh.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wp.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://sr.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yi.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://nj.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ps.hnjuh.cn

[S43] C++：智能指针
来源：http://ls.521024.cn

auto p = std::make_unique<int>(5);
来源：http://pr.szxytkj.cn

[S44] C++：引用传参
来源：http://ys.asd995.cn

void inc(int &x) { ++x; }
来源：http://gz.nszjky.cn

[S45] C++：lambda
来源：http://pp.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rb.wgjwhj.cn

[S46] C++：函数模板
来源：http://xm.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iu.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ex.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bn.shxzukj.cn

[S48] C++：逐行读文件
来源：http://gu.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vz.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://eb.jianghongdianzi.cn

[S49] C++：写文件
来源：http://cc.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hr.colortex.cn

[S50] C++：格式化数字
来源：http://ik.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jp.nicolike.cn

[S51] C++：显式类型转换
来源：http://mq.hahajie.cn

static_cast<double>(a) / b
来源：http://zi.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://ru.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://uh.gzmigu.cn

[S53] C++：移动语义
来源：http://dd.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://wl.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://xi.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zi.9csxet.cn

[S55] C++：结构化绑定
来源：http://ad.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fc.521024.cn

[S56] C++：optional
来源：http://bj.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vz.yuexingan06.cn

[S57] C++：编译期常量
来源：http://uf.newstarts.cn

constexpr int N = 10;
来源：http://mn.szsharing.cn

[S58] C++：命名空间
来源：http://oi.521024.cn

namespace ns { int f() { return 1; } }
来源：http://im.huanxung.cn

[S59] C++：静态断言
来源：http://qc.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tf.colortex.cn

[S60] C++：遍历并删除元素
来源：http://cr.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cq.shxzukj.cn

================================================================================
来源：http://bl.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zn.jianghongdianzi.cn

================================================================================
来源：http://qn.521024.cn

[T01] Kotlin：Hello World
来源：http://op.hnjuh.cn

println("Hello")
来源：http://tq.huixiangedu.cn

[T02] Kotlin：变量
来源：http://ac.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jb.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://oe.521024.cn

"值: $b"
来源：http://uy.hahajie.cn

[T04] Kotlin：空安全
来源：http://yz.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://ii.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://dd.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jl.huanxung.cn

[T06] Kotlin：集合映射
来源：http://xa.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nl.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://gb.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oj.nicolike.cn

[T08] Kotlin：数据类
来源：http://ke.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://zi.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://at.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://vj.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://fu.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kw.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ev.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vi.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://fn.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://sn.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://ud.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://cm.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://ek.shxzukj.cn

for (i in 1..10) println(i)
来源：http://mk.gzmigu.cn

[T15] Kotlin：接口
来源：http://yk.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ux.chemitech.net.cn

[T16] Swift：Hello World
来源：http://yb.hnjuh.cn

print("Hello")
来源：http://up.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://ef.bjjhwx.cn

var a = 1;  let b = 2
来源：http://pd.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://wu.yuntaijiaju.cn

"值: \(b)"
来源：http://yr.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://go.wgjwhj.cn

if let n = opt { print(n) }
来源：http://wt.gzmigu.cn

[T20] Swift：数组操作
来源：http://wo.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ep.huixiangedu.cn

[T21] Swift：遍历
来源：http://fb.jianghongdianzi.cn

for x in a { print(x) }
来源：http://nx.huanxung.cn

[T22] Swift：字典
来源：http://xj.nicolike.cn

var d = ["a": 1];  d["b"] = 2
来源：http://be.colortex.cn

[T23] Swift：函数
来源：http://sp.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yb.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://cd.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bb.lnxyls.cn

[T25] Swift：结构体
来源：http://qy.yuexingan06.cn

struct P { var x: Int }
来源：http://hu.chemitech.net.cn

[T26] Swift：类与重写
来源：http://tj.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://nz.shxzskj.cn

[T27] Swift：错误处理
来源：http://vd.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://rn.szsharing.cn

[T28] Swift：枚举
来源：http://po.szxytkj.cn

enum Color { case red, green }
来源：http://jo.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://su.nicolike.cn

guard let x = opt else { return }
来源：http://od.gzmigu.cn

[T30] Swift：协议
来源：http://vv.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://as.muxihuayi.cn

[T31] Lua：Hello World
来源：http://pu.jctech888.com.cn

print("Hello")
来源：http://iy.shxzskj.cn

[T32] Lua：局部变量
来源：http://nr.gzmigu.cn

local a = 1
来源：http://gt.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://vd.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fk.wgjwhj.cn

[T34] Lua：遍历表
来源：http://tr.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ln.huanxung.cn

[T35] Lua：字典表
来源：http://vt.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://gh.muxihuayi.cn

[T36] Lua：函数
来源：http://vm.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://gj.nicolike.cn

[T37] Lua：字符串拼接
来源：http://gc.nszjky.cn

"a" .. "b"
来源：http://sh.gzmigu.cn

[T38] Lua：条件
来源：http://vb.asd995.cn

if x > 0 then print("正") end
来源：http://bs.newstarts.cn

[T39] Lua：模式匹配
来源：http://fg.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://et.jctech888.com.cn

[T40] Lua：元表
来源：http://ym.nszjky.cn

setmetatable({}, { __index = base })
来源：http://ol.hahajie.cn

[T41] Perl：Hello World
来源：http://zj.chemitech.net.cn

print "Hello\n";
来源：http://ia.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://qo.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://de.colortex.cn

[T43] Perl：字符串插值
来源：http://bh.yuntaijiaju.cn

"值: $a"
来源：http://rf.gzmigu.cn

[T44] Perl：条件
来源：http://iw.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://sv.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://ir.asd995.cn

for my $x (@arr) { print $x; }
来源：http://ue.hnjuh.cn

[T46] Perl：哈希操作
来源：http://nx.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://da.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://ra.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yp.newstarts.cn

[T48] Perl：正则替换
来源：http://zu.huanxung.cn

$s =~ s/old/new/g;
来源：http://jo.gzmigu.cn

[T49] Perl：函数
来源：http://pd.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ix.huanxung.cn

[T50] Perl：逐行读文件
来源：http://yn.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ac.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://hu.shxzskj.cn

[T51] Scala：Hello World
来源：http://cf.yuexingan06.cn

println("Hello")
来源：http://dm.chemitech.net.cn

[T52] Scala：变量
来源：http://ef.shxzukj.cn

val a = 1;  var b = 2
来源：http://te.nszjky.cn

[T53] Scala：字符串插值
来源：http://mw.nicolike.cn

s"值: $b"
来源：http://yg.9csxet.cn

[T54] Scala：集合映射
来源：http://pi.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://iu.huanxung.cn

[T55] Scala：集合过滤
来源：http://qo.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fd.shtwfgs.cn

[T56] Scala：样例类
来源：http://ed.szxytkj.cn

case class User(name: String, age: Int)
来源：http://jz.nicolike.cn

[T57] Scala：模式匹配
来源：http://hr.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ex.yuexingan06.cn

[T58] Scala：函数定义
来源：http://cs.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rw.shtwfgs.cn

[T59] Scala：循环
来源：http://bv.hnjuh.cn

for (i <- 1 to 10) println(i)
来源：http://uc.huanxung.cn

[T60] Scala：折叠
来源：http://ys.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qj.wgjwhj.cn

================================================================================
来源：http://ae.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vq.szxytkj.cn

================================================================================
来源：http://md.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://hf.shxzskj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vx.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ie.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yh.521024.cn

[U03] Py：加载 .env 配置
来源：http://nu.gzmigu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sk.9csxet.cn

[U04] Py：变量调试打印
来源：http://pq.lnxyls.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eb.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://iy.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://uo.nicolike.cn

[U06] Py：合并两个字典
来源：http://xj.szsharing.cn

{**a, **b}
来源：http://zh.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://de.hahajie.cn

{v: k for k, v in d.items()}
来源：http://vc.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://yd.lnxyls.cn

[y for x in nested for y in x]
来源：http://jc.asd995.cn

[U09] Py：字典取最大值的键
来源：http://pp.hahajie.cn

max(d, key=d.get)
来源：http://mh.shxzukj.cn

[U10] Py：按值排序字典
来源：http://fa.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yi.lnxyls.cn

[U11] Py：生成器表达式
来源：http://kj.shtwfgs.cn

(x * 2 for x in arr)
来源：http://zl.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qv.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://pc.szxytkj.cn

[U13] Py：固定长度队列
来源：http://jt.nszjky.cn

deque(maxlen=10)
来源：http://wd.nicolike.cn

[U14] Py：分组收集到列表
来源：http://qe.colortex.cn

defaultdict(list)
来源：http://tp.huixiangedu.cn

[U15] Py：高精度计时
来源：http://yq.colortex.cn

t = time.perf_counter()
来源：http://aw.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://mc.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cj.shxzukj.cn

[U17] Py：初始化日志
来源：http://qr.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://wa.asd995.cn

[U18] Py：预编译正则
来源：http://gc.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://jb.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://rq.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dr.nszjky.cn

[U20] Py：缓存函数结果
来源：http://lg.huanxung.cn

@functools.lru_cache(maxsize=None)
来源：http://eo.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://wd.shtwfgs.cn

@contextlib.contextmanager
来源：http://sx.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://uc.bjjhwx.cn

list(zip(*m))
来源：http://kb.colortex.cn

[U23] Py：分块读取大文件
来源：http://my.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kt.muxihuayi.cn

[U24] Py：路径操作
来源：http://cn.jctech888.com.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yr.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://hr.jctech888.com.cn

csv.DictReader(f)
来源：http://wx.szxytkj.cn

[U26] Py：并发下载
来源：http://zd.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mz.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://eo.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://cm.szsharing.cn

[U28] Py：类型别名
来源：http://is.shtwfgs.cn

UserId = int
来源：http://gi.muxihuayi.cn

[U29] Py：属性校验
来源：http://xr.9csxet.cn

@property 与 @x.setter 配合
来源：http://aw.lnxyls.cn

[U30] Py：数据类
来源：http://vn.szxytkj.cn

@dataclass(slots=True)
来源：http://yb.gzmigu.cn

[U31] Py：单测
来源：http://jf.521024.cn

python -m pytest -q
来源：http://yt.muxihuayi.cn

[U32] Py：代码格式化
来源：http://vc.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://jw.nicolike.cn

[U33] Py：打包发布
来源：http://ew.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ru.521024.cn

[U34] Py：判断编码
来源：http://do.hnjuh.cn

chardet.detect(raw)
来源：http://xn.yuexingan06.cn

[U35] Py：发送邮件
来源：http://ue.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mi.huixiangedu.cn

[U36] Py：定时任务
来源：http://mc.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://si.newstarts.cn

[U37] Py：读写 Excel
来源：http://id.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qo.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://xo.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://sw.shxzskj.cn

[U39] Py：判断是否在交互环境
来源：http://nd.panjiajie.cn

sys.stdout.isatty()
来源：http://up.szsharing.cn

[U40] Py：打印到标准错误
来源：http://ow.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://sf.colortex.cn

[U41] PHP：初始化 Composer 项目
来源：http://eb.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sw.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://pv.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ys.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://vj.shxzukj.cn

namespace App\Http;
来源：http://jx.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://np.hnjuh.cn

declare(strict_types=1);
来源：http://bg.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://as.asd995.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://po.newstarts.cn

[U46] PHP：可空类型
来源：http://ky.9csxet.cn

?string $name = null
来源：http://sh.nszjky.cn

[U47] PHP：联合类型
来源：http://hp.shtwfgs.cn

int|string $id
来源：http://fr.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://wj.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xy.asd995.cn

[U49] PHP：只读属性
来源：http://jg.shtwfgs.cn

public readonly string $name
来源：http://oz.hahajie.cn

[U50] PHP：构造器属性提升
来源：http://bs.hahajie.cn

public function __construct(private int $id) {}
来源：http://se.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://wi.shxzukj.cn

[$a, $b] = $arr;
来源：http://bc.huixinmuqiang.cn

[U52] PHP：箭头函数
来源：http://ll.asd995.cn

$double = fn($x) => $x * 2;
来源：http://mp.asd995.cn

[U53] PHP：空合并运算符
来源：http://oj.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://re.nicolike.cn

[U54] PHP：空安全调用
来源：http://zb.jctech888.com.cn

$obj?->method()
来源：http://ez.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://he.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rf.panjiajie.cn

[U56] PHP：命名参数
来源：http://uk.haigaiapp.cn

f(a: 1, b: 2)
来源：http://tl.nszjky.cn

[U57] PHP：字符串插值
来源：http://uh.hahajie.cn

"值: {$a}"
来源：http://qw.colortex.cn

[U58] PHP：数组三件套
来源：http://kr.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ty.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://su.lnxyls.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mm.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://re.chemitech.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rg.shxzskj.cn


<!-- 参考信息 -->