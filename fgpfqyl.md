代发 wailian999

#include <iostream>
来源：http://uk.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://sk.wgjwhj.cn

[S32] C++：字符串
来源：http://rd.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://qw.shtwfgs.cn

[S33] C++：vector 增删
来源：http://vg.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jx.panjiajie.cn

[S34] C++：遍历 vector
来源：http://dw.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://cq.szsharing.cn

[S35] C++：map
来源：http://pk.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uf.huanxung.cn

[S36] C++：unordered_map
来源：http://er.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tl.hnjuh.cn

[S37] C++：set
来源：http://xc.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sb.521024.cn

[S38] C++：排序
来源：http://aq.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://zq.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://qe.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vo.nszjky.cn

[S40] C++：查找元素
来源：http://tf.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xz.szxytkj.cn

[S41] C++：类与构造函数
来源：http://ye.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://za.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://zi.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://sx.newstarts.cn

[S43] C++：智能指针
来源：http://fo.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://qi.hnjuh.cn

[S44] C++：引用传参
来源：http://fl.521024.cn

void inc(int &x) { ++x; }
来源：http://rl.newstarts.cn

[S45] C++：lambda
来源：http://pb.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ra.hahajie.cn

[S46] C++：函数模板
来源：http://su.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qr.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://hg.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jv.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://jz.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gj.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://oq.haigaiapp.cn

[S49] C++：写文件
来源：http://qq.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rv.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://yx.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fp.9csxet.cn

[S51] C++：显式类型转换
来源：http://tv.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://fl.yuntaijiaju.cn

[S52] C++：const 与 noexcept
来源：http://pk.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://nh.haigaiapp.cn

[S53] C++：移动语义
来源：http://rm.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://pj.huanxung.cn

[S54] C++：异常处理
来源：http://im.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ts.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://js.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cd.huanxung.cn

[S56] C++：optional
来源：http://lh.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wj.panjiajie.cn

[S57] C++：编译期常量
来源：http://ku.asd995.cn

constexpr int N = 10;
来源：http://pf.shxzukj.cn

[S58] C++：命名空间
来源：http://ju.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://vf.bookmarksfly.cn

[S59] C++：静态断言
来源：http://ma.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zl.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://hj.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ha.szsharing.cn

================================================================================
来源：http://vg.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://re.shxzskj.cn

================================================================================
来源：http://xy.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://jr.shxzukj.cn

println("Hello")
来源：http://fs.haigaiapp.cn

[T02] Kotlin：变量
来源：http://ys.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rm.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://db.szxytkj.cn

"值: $b"
来源：http://mx.521024.cn

[T04] Kotlin：空安全
来源：http://tv.9csxet.cn

val n: String? = null;  n?.length
来源：http://sm.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://ww.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ej.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://et.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vq.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://qz.jianghongdianzi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rq.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://bj.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://ei.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://as.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://wp.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://xu.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://po.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://sg.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tk.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://rl.jianghongdianzi.cn

val (a, b) = Pair(1, 2)
来源：http://xi.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://tv.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://ak.bjjhwx.cn

[T14] Kotlin：循环
来源：http://ol.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://fl.hahajie.cn

[T15] Kotlin：接口
来源：http://jb.nicolike.cn

interface Shape { fun area(): Double }
来源：http://kc.newstarts.cn

[T16] Swift：Hello World
来源：http://ys.nszjky.cn

print("Hello")
来源：http://fp.colortex.cn

[T17] Swift：变量与常量
来源：http://ec.yuexingan06.cn

var a = 1;  let b = 2
来源：http://mv.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://dp.newstarts.cn

"值: \(b)"
来源：http://co.asd995.cn

[T19] Swift：可选绑定
来源：http://iw.colortex.cn

if let n = opt { print(n) }
来源：http://ap.huixiangedu.cn

[T20] Swift：数组操作
来源：http://vl.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mq.521024.cn

[T21] Swift：遍历
来源：http://ho.nicolike.cn

for x in a { print(x) }
来源：http://hu.szxytkj.cn

[T22] Swift：字典
来源：http://pr.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gs.yuexingan06.cn

[T23] Swift：函数
来源：http://zg.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wc.9csxet.cn

[T24] Swift：闭包
来源：http://yp.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rn.521024.cn

[T25] Swift：结构体
来源：http://rd.bjjhwx.cn

struct P { var x: Int }
来源：http://ji.bjjhwx.cn

[T26] Swift：类与重写
来源：http://tt.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://gt.szxytkj.cn

[T27] Swift：错误处理
来源：http://rt.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://xt.szxytkj.cn

[T28] Swift：枚举
来源：http://yq.gzmigu.cn

enum Color { case red, green }
来源：http://hq.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://xx.hnjuh.cn

guard let x = opt else { return }
来源：http://st.nicolike.cn

[T30] Swift：协议
来源：http://yq.colortex.cn

protocol Shape { func area() -> Double }
来源：http://ei.wgjwhj.cn

[T31] Lua：Hello World
来源：http://uj.gzmigu.cn

print("Hello")
来源：http://xe.gzmigu.cn

[T32] Lua：局部变量
来源：http://hf.nicolike.cn

local a = 1
来源：http://ro.lnxyls.cn

[T33] Lua：表（数组）
来源：http://oe.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://om.muxihuayi.cn

[T34] Lua：遍历表
来源：http://un.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yj.szsharing.cn

[T35] Lua：字典表
来源：http://sc.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ur.shxzukj.cn

[T36] Lua：函数
来源：http://du.gzmigu.cn

function add(a, b) return a + b end
来源：http://rs.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://zk.shxzskj.cn

"a" .. "b"
来源：http://wy.huixinmuqiang.cn

[T38] Lua：条件
来源：http://fx.hnjuh.cn

if x > 0 then print("正") end
来源：http://vl.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://hx.nicolike.cn

string.find(s, "%d+")
来源：http://or.nicolike.cn

[T40] Lua：元表
来源：http://ir.colortex.cn

setmetatable({}, { __index = base })
来源：http://ot.szsharing.cn

[T41] Perl：Hello World
来源：http://sn.jianghongdianzi.cn

print "Hello\n";
来源：http://sa.chemitech.net.cn

[T42] Perl：变量类型
来源：http://rp.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lt.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://ax.huixiangedu.cn

"值: $a"
来源：http://oa.gzmigu.cn

[T44] Perl：条件
来源：http://kr.colortex.cn

if ($a > 0) { print "正"; }
来源：http://ny.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://uw.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://fc.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://zt.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xk.szsharing.cn

[T47] Perl：正则捕获
来源：http://rz.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fe.lnxyls.cn

[T48] Perl：正则替换
来源：http://fq.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://we.bookmarksfly.cn

[T49] Perl：函数
来源：http://qv.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wh.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://fa.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ax.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://uq.yuexingan06.cn

[T51] Scala：Hello World
来源：http://fu.gzmigu.cn

println("Hello")
来源：http://xz.muxihuayi.cn

[T52] Scala：变量
来源：http://if.asd995.cn

val a = 1;  var b = 2
来源：http://vh.szxytkj.cn

[T53] Scala：字符串插值
来源：http://nc.colortex.cn

s"值: $b"
来源：http://uj.9csxet.cn

[T54] Scala：集合映射
来源：http://py.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://ue.panjiajie.cn

[T55] Scala：集合过滤
来源：http://dl.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qv.yuntaijiaju.cn

[T56] Scala：样例类
来源：http://bo.gzmigu.cn

case class User(name: String, age: Int)
来源：http://if.shxzskj.cn

[T57] Scala：模式匹配
来源：http://fq.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rd.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://cn.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jc.panjiajie.cn

[T59] Scala：循环
来源：http://zk.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://jn.bjjhwx.cn

[T60] Scala：折叠
来源：http://rs.521024.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dz.9csxet.cn

================================================================================
来源：http://au.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lk.asd995.cn

================================================================================
来源：http://ko.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://yc.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cl.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ls.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uc.asd995.cn

[U03] Py：加载 .env 配置
来源：http://gg.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qt.newstarts.cn

[U04] Py：变量调试打印
来源：http://af.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uw.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://gn.nszjky.cn

list(dict.fromkeys(arr))
来源：http://jt.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://sz.muxihuayi.cn

{**a, **b}
来源：http://hp.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://so.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://de.hahajie.cn

[U08] Py：展平二维列表
来源：http://aj.szxytkj.cn

[y for x in nested for y in x]
来源：http://fh.nicolike.cn

[U09] Py：字典取最大值的键
来源：http://eq.nszjky.cn

max(d, key=d.get)
来源：http://fb.bjjhwx.cn

[U10] Py：按值排序字典
来源：http://jb.haigaiapp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rf.hnjuh.cn

[U11] Py：生成器表达式
来源：http://rd.huixiangedu.cn

(x * 2 for x in arr)
来源：http://el.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gx.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://sf.jianghongdianzi.cn

[U13] Py：固定长度队列
来源：http://sh.huixinmuqiang.cn

deque(maxlen=10)
来源：http://dk.lnxyls.cn

[U14] Py：分组收集到列表
来源：http://ez.szsharing.cn

defaultdict(list)
来源：http://py.hahajie.cn

[U15] Py：高精度计时
来源：http://vj.huanxung.cn

t = time.perf_counter()
来源：http://kc.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://rk.chemitech.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ib.muxihuayi.cn

[U17] Py：初始化日志
来源：http://sr.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://tt.panjiajie.cn

[U18] Py：预编译正则
来源：http://gn.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://xp.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://nz.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zm.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://wt.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://mu.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://wf.shtwfgs.cn

@contextlib.contextmanager
来源：http://be.szxytkj.cn

[U22] Py：矩阵转置
来源：http://wf.yuntaijiaju.cn

list(zip(*m))
来源：http://sj.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://gc.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://od.newstarts.cn

[U24] Py：路径操作
来源：http://vb.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bi.colortex.cn

[U25] Py：CSV 按字典读
来源：http://cg.bookmarksfly.cn

csv.DictReader(f)
来源：http://ke.muxihuayi.cn

[U26] Py：并发下载
来源：http://ni.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cq.shxzukj.cn

[U27] Py：异步 HTTP
来源：http://gn.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://iu.gzmigu.cn

[U28] Py：类型别名
来源：http://yp.szsharing.cn

UserId = int
来源：http://rq.gzmigu.cn

[U29] Py：属性校验
来源：http://eb.huanxung.cn

@property 与 @x.setter 配合
来源：http://ny.nicolike.cn

[U30] Py：数据类
来源：http://hz.huanxung.cn

@dataclass(slots=True)
来源：http://et.huanxung.cn

[U31] Py：单测
来源：http://jo.bookmarksfly.cn

python -m pytest -q
来源：http://tu.nszjky.cn

[U32] Py：代码格式化
来源：http://hj.nicolike.cn

ruff format . && ruff check --fix .
来源：http://tk.huixiangedu.cn

[U33] Py：打包发布
来源：http://mh.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://yq.jctech888.com.cn

[U34] Py：判断编码
来源：http://qx.nszjky.cn

chardet.detect(raw)
来源：http://ev.lnxyls.cn

[U35] Py：发送邮件
来源：http://tu.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zo.huanxung.cn

[U36] Py：定时任务
来源：http://da.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://dv.szxytkj.cn

[U37] Py：读写 Excel
来源：http://xt.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ni.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://ye.szsharing.cn

Path(__file__).resolve().parent
来源：http://ox.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://jy.asd995.cn

sys.stdout.isatty()
来源：http://sc.shxzukj.cn

[U40] Py：打印到标准错误
来源：http://nj.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://nv.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://jg.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qf.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://tf.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://op.asd995.cn

[U43] PHP：声明命名空间
来源：http://vv.jianghongdianzi.cn

namespace App\Http;
来源：http://dl.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://cm.lnxyls.cn

declare(strict_types=1);
来源：http://pz.hahajie.cn

[U45] PHP：类型声明与返回类型
来源：http://qq.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xa.newstarts.cn

[U46] PHP：可空类型
来源：http://qn.chemitech.net.cn

?string $name = null
来源：http://ps.hahajie.cn

[U47] PHP：联合类型
来源：http://ms.hnjuh.cn

int|string $id
来源：http://ta.yuexingan06.cn

[U48] PHP：纯枚举
来源：http://px.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://au.panjiajie.cn

[U49] PHP：只读属性
来源：http://tk.newstarts.cn

public readonly string $name
来源：http://lp.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://eb.newstarts.cn

public function __construct(private int $id) {}
来源：http://hh.shxzskj.cn

[U51] PHP：数组解构
来源：http://at.nszjky.cn

[$a, $b] = $arr;
来源：http://ts.shxzskj.cn

[U52] PHP：箭头函数
来源：http://jg.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://vc.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://rz.szsharing.cn

$v = $a ?? $b ?? "default";
来源：http://hn.nszjky.cn

[U54] PHP：空安全调用
来源：http://dt.muxihuayi.cn

$obj?->method()
来源：http://nf.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://yb.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fq.hahajie.cn

[U56] PHP：命名参数
来源：http://lp.bookmarksfly.cn

f(a: 1, b: 2)
来源：http://kl.bjjhwx.cn


<!-- 参考信息 -->