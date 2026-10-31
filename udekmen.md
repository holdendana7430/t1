代发 wailian999

[S33] C++：vector 增删
来源：http://eh.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dg.colortex.cn

[S34] C++：遍历 vector
来源：http://bj.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://vo.9csxet.cn

[S35] C++：map
来源：http://cz.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xq.haigaiapp.cn

[S36] C++：unordered_map
来源：http://ox.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://je.huixiangedu.cn

[S37] C++：set
来源：http://wd.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cg.haigaiapp.cn

[S38] C++：排序
来源：http://ao.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://rc.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://uj.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vt.yuexingan06.cn

[S40] C++：查找元素
来源：http://qx.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qg.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://fs.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uh.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://qb.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://xw.huixiangedu.cn

[S43] C++：智能指针
来源：http://rd.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://vw.huixiangedu.cn

[S44] C++：引用传参
来源：http://qi.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://hh.jctech888.com.cn

[S45] C++：lambda
来源：http://nr.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://re.nicolike.cn

[S46] C++：函数模板
来源：http://qj.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wj.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://km.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ly.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://to.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zt.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ve.9csxet.cn

[S49] C++：写文件
来源：http://kt.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://co.chemitech.net.cn

[S50] C++：格式化数字
来源：http://hw.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rw.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://mm.gzmigu.cn

static_cast<double>(a) / b
来源：http://vy.asd995.cn

[S52] C++：const 与 noexcept
来源：http://bc.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://fk.huixiangedu.cn

[S53] C++：移动语义
来源：http://jh.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://gd.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://uu.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tw.521024.cn

[S55] C++：结构化绑定
来源：http://wl.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lp.nszjky.cn

[S56] C++：optional
来源：http://ry.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yi.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://je.colortex.cn

constexpr int N = 10;
来源：http://qd.panjiajie.cn

[S58] C++：命名空间
来源：http://gw.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://uh.521024.cn

[S59] C++：静态断言
来源：http://cc.bjjhwx.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aa.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://xm.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wg.huixiangedu.cn

================================================================================
来源：http://qf.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bj.shxzskj.cn

================================================================================
来源：http://tm.nicolike.cn

[T01] Kotlin：Hello World
来源：http://et.chemitech.net.cn

println("Hello")
来源：http://gk.panjiajie.cn

[T02] Kotlin：变量
来源：http://zg.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qz.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://ww.bjjhwx.cn

"值: $b"
来源：http://uy.yuexingan06.cn

[T04] Kotlin：空安全
来源：http://ju.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://mx.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://nz.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uk.szsharing.cn

[T06] Kotlin：集合映射
来源：http://oi.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dl.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://wt.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qj.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://dk.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://do.asd995.cn

[T09] Kotlin：扩展函数
来源：http://qc.521024.cn

fun String.exclaim() = this + "!"
来源：http://kq.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://qg.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kd.hnjuh.cn

[T11] Kotlin：协程
来源：http://on.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hi.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://vl.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://hy.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://tn.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://tc.hnjuh.cn

[T14] Kotlin：循环
来源：http://tx.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://us.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://sx.newstarts.cn

interface Shape { fun area(): Double }
来源：http://qq.muxihuayi.cn

[T16] Swift：Hello World
来源：http://qw.shtwfgs.cn

print("Hello")
来源：http://ei.panjiajie.cn

[T17] Swift：变量与常量
来源：http://ii.bookmarksfly.cn

var a = 1;  let b = 2
来源：http://xc.newstarts.cn

[T18] Swift：字符串插值
来源：http://lo.colortex.cn

"值: \(b)"
来源：http://qt.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://bx.panjiajie.cn

if let n = opt { print(n) }
来源：http://wy.haigaiapp.cn

[T20] Swift：数组操作
来源：http://qt.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uj.hnjuh.cn

[T21] Swift：遍历
来源：http://op.asd995.cn

for x in a { print(x) }
来源：http://on.huanxung.cn

[T22] Swift：字典
来源：http://ye.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hu.szsharing.cn

[T23] Swift：函数
来源：http://db.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nn.9csxet.cn

[T24] Swift：闭包
来源：http://jc.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://if.newstarts.cn

[T25] Swift：结构体
来源：http://ab.nicolike.cn

struct P { var x: Int }
来源：http://cw.huanxung.cn

[T26] Swift：类与重写
来源：http://wk.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://fs.chemitech.net.cn

[T27] Swift：错误处理
来源：http://rc.521024.cn

do { try f() } catch { print(error) }
来源：http://kv.szsharing.cn

[T28] Swift：枚举
来源：http://ts.521024.cn

enum Color { case red, green }
来源：http://rt.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://fd.shxzskj.cn

guard let x = opt else { return }
来源：http://tr.szxytkj.cn

[T30] Swift：协议
来源：http://xn.asd995.cn

protocol Shape { func area() -> Double }
来源：http://mu.hahajie.cn

[T31] Lua：Hello World
来源：http://di.muxihuayi.cn

print("Hello")
来源：http://sc.colortex.cn

[T32] Lua：局部变量
来源：http://wm.chemitech.net.cn

local a = 1
来源：http://tb.hahajie.cn

[T33] Lua：表（数组）
来源：http://un.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nm.bjjhwx.cn

[T34] Lua：遍历表
来源：http://cz.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iu.lnxyls.cn

[T35] Lua：字典表
来源：http://ug.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://dc.haigaiapp.cn

[T36] Lua：函数
来源：http://nb.521024.cn

function add(a, b) return a + b end
来源：http://el.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://jp.szxytkj.cn

"a" .. "b"
来源：http://wu.muxihuayi.cn

[T38] Lua：条件
来源：http://ki.shxzukj.cn

if x > 0 then print("正") end
来源：http://nh.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://qp.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://pv.panjiajie.cn

[T40] Lua：元表
来源：http://lj.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://ik.chemitech.net.cn

[T41] Perl：Hello World
来源：http://bb.yuntaijiaju.cn

print "Hello\n";
来源：http://lj.muxihuayi.cn

[T42] Perl：变量类型
来源：http://pp.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xl.9csxet.cn

[T43] Perl：字符串插值
来源：http://az.shxzskj.cn

"值: $a"
来源：http://kk.muxihuayi.cn

[T44] Perl：条件
来源：http://vx.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://mx.lnxyls.cn

[T45] Perl：数组遍历
来源：http://nh.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://xe.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://ty.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://na.nicolike.cn

[T47] Perl：正则捕获
来源：http://cp.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pi.asd995.cn

[T48] Perl：正则替换
来源：http://mf.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://xu.jctech888.com.cn

[T49] Perl：函数
来源：http://ep.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sp.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://uo.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://my.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ra.haigaiapp.cn

[T51] Scala：Hello World
来源：http://gk.nszjky.cn

println("Hello")
来源：http://gr.haigaiapp.cn

[T52] Scala：变量
来源：http://sy.lnxyls.cn

val a = 1;  var b = 2
来源：http://bw.huanxung.cn

[T53] Scala：字符串插值
来源：http://er.521024.cn

s"值: $b"
来源：http://pi.nszjky.cn

[T54] Scala：集合映射
来源：http://rx.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://fn.shxzukj.cn

[T55] Scala：集合过滤
来源：http://rb.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lq.shtwfgs.cn

[T56] Scala：样例类
来源：http://xl.panjiajie.cn

case class User(name: String, age: Int)
来源：http://la.panjiajie.cn

[T57] Scala：模式匹配
来源：http://wx.lnxyls.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vx.muxihuayi.cn

[T58] Scala：函数定义
来源：http://aw.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uy.szxytkj.cn

[T59] Scala：循环
来源：http://om.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://bw.bjjhwx.cn

[T60] Scala：折叠
来源：http://mx.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mf.muxihuayi.cn

================================================================================
来源：http://mc.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hk.521024.cn

================================================================================
来源：http://lm.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://je.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cl.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://jo.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://af.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://nt.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sr.panjiajie.cn

[U04] Py：变量调试打印
来源：http://nr.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ti.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://wn.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://tv.hnjuh.cn

[U06] Py：合并两个字典
来源：http://vd.gzmigu.cn

{**a, **b}
来源：http://tb.chemitech.net.cn

[U07] Py：反转字典键值
来源：http://ur.nszjky.cn

{v: k for k, v in d.items()}
来源：http://jq.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://rh.shtwfgs.cn

[y for x in nested for y in x]
来源：http://wy.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://gs.shxzukj.cn

max(d, key=d.get)
来源：http://dt.colortex.cn

[U10] Py：按值排序字典
来源：http://sk.nszjky.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qy.hnjuh.cn

[U11] Py：生成器表达式
来源：http://yz.shxzukj.cn

(x * 2 for x in arr)
来源：http://xy.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nq.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://wf.newstarts.cn

[U13] Py：固定长度队列
来源：http://ky.huanxung.cn

deque(maxlen=10)
来源：http://rm.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://xs.hahajie.cn

defaultdict(list)
来源：http://uq.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://dn.shxzukj.cn

t = time.perf_counter()
来源：http://ec.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://eo.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nj.bjjhwx.cn

[U17] Py：初始化日志
来源：http://dp.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://vj.huanxung.cn

[U18] Py：预编译正则
来源：http://kg.nicolike.cn

pat = re.compile(r"\d+")
来源：http://jf.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://tk.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://me.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://wl.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://bm.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://sn.bookmarksfly.cn

@contextlib.contextmanager
来源：http://yv.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://fu.huixiangedu.cn

list(zip(*m))
来源：http://ul.hahajie.cn

[U23] Py：分块读取大文件
来源：http://ld.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://av.jctech888.com.cn

[U24] Py：路径操作
来源：http://ij.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xy.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://wh.szsharing.cn

csv.DictReader(f)
来源：http://qb.gzmigu.cn

[U26] Py：并发下载
来源：http://lj.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://du.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://lb.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://or.wgjwhj.cn

[U28] Py：类型别名
来源：http://df.jctech888.com.cn

UserId = int
来源：http://dr.bjjhwx.cn

[U29] Py：属性校验
来源：http://ey.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://db.szsharing.cn

[U30] Py：数据类
来源：http://rl.bjjhwx.cn

@dataclass(slots=True)
来源：http://ss.haigaiapp.cn

[U31] Py：单测
来源：http://rd.yuexingan06.cn

python -m pytest -q
来源：http://sw.9csxet.cn

[U32] Py：代码格式化
来源：http://qc.shtwfgs.cn

ruff format . && ruff check --fix .
来源：http://dp.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://rl.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://vo.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://es.bookmarksfly.cn

chardet.detect(raw)
来源：http://ex.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://ud.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tq.newstarts.cn

[U36] Py：定时任务
来源：http://il.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://np.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://gt.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ql.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://xy.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://jd.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://xy.lnxyls.cn

sys.stdout.isatty()
来源：http://la.9csxet.cn

[U40] Py：打印到标准错误
来源：http://ou.gzmigu.cn

print("err", file=sys.stderr)
来源：http://lf.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://se.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hb.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ry.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qq.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://mn.jianghongdianzi.cn

namespace App\Http;
来源：http://ie.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://sw.nszjky.cn

declare(strict_types=1);
来源：http://cm.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://ct.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nu.muxihuayi.cn

[U46] PHP：可空类型
来源：http://ee.jianghongdianzi.cn

?string $name = null
来源：http://le.nicolike.cn

[U47] PHP：联合类型
来源：http://dx.jianghongdianzi.cn

int|string $id
来源：http://ee.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://sm.panjiajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vm.9csxet.cn

[U49] PHP：只读属性
来源：http://oa.bookmarksfly.cn

public readonly string $name
来源：http://un.muxihuayi.cn

[U50] PHP：构造器属性提升
来源：http://oz.gzmigu.cn

public function __construct(private int $id) {}
来源：http://zk.huixiangedu.cn

[U51] PHP：数组解构
来源：http://li.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://bg.asd995.cn

[U52] PHP：箭头函数
来源：http://tx.hahajie.cn

$double = fn($x) => $x * 2;
来源：http://ma.huanxung.cn

[U53] PHP：空合并运算符
来源：http://tq.521024.cn

$v = $a ?? $b ?? "default";
来源：http://nv.nszjky.cn

[U54] PHP：空安全调用
来源：http://nu.huanxung.cn

$obj?->method()
来源：http://av.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://pt.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gr.muxihuayi.cn

[U56] PHP：命名参数
来源：http://yr.jctech888.com.cn

f(a: 1, b: 2)
来源：http://cg.asd995.cn

[U57] PHP：字符串插值
来源：http://uz.szxytkj.cn

"值: {$a}"
来源：http://nd.huixiangedu.cn

[U58] PHP：数组三件套
来源：http://hx.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nq.hahajie.cn


<!-- 参考信息 -->