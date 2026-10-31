代发 wailian999

#include <iostream>
来源：http://nw.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ng.bjjhwx.cn

[S32] C++：字符串
来源：http://mv.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://uw.muxihuayi.cn

[S33] C++：vector 增删
来源：http://rp.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ck.521024.cn

[S34] C++：遍历 vector
来源：http://kp.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://yz.panjiajie.cn

[S35] C++：map
来源：http://dd.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ya.panjiajie.cn

[S36] C++：unordered_map
来源：http://iz.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://im.szxytkj.cn

[S37] C++：set
来源：http://xt.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sk.huixinmuqiang.cn

[S38] C++：排序
来源：http://my.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://cv.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://wn.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bd.nicolike.cn

[S40] C++：查找元素
来源：http://vp.9csxet.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hx.hahajie.cn

[S41] C++：类与构造函数
来源：http://ri.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yo.nszjky.cn

[S42] C++：继承与虚函数
来源：http://jy.521024.cn

class B : public Base { public: void f() override {} };
来源：http://gk.jctech888.com.cn

[S43] C++：智能指针
来源：http://bu.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://fg.colortex.cn

[S44] C++：引用传参
来源：http://na.521024.cn

void inc(int &x) { ++x; }
来源：http://yu.szxytkj.cn

[S45] C++：lambda
来源：http://db.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bh.muxihuayi.cn

[S46] C++：函数模板
来源：http://cm.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qu.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://uq.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gk.szxytkj.cn

[S48] C++：逐行读文件
来源：http://qo.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://af.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://sv.bjjhwx.cn

[S49] C++：写文件
来源：http://yx.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fd.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://vf.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bc.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://rs.hahajie.cn

static_cast<double>(a) / b
来源：http://od.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://vu.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://da.hahajie.cn

[S53] C++：移动语义
来源：http://kr.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://ht.9csxet.cn

[S54] C++：异常处理
来源：http://sq.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cm.shxzukj.cn

[S55] C++：结构化绑定
来源：http://zz.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zm.huixinmuqiang.cn

[S56] C++：optional
来源：http://pn.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mv.colortex.cn

[S57] C++：编译期常量
来源：http://ai.nszjky.cn

constexpr int N = 10;
来源：http://ly.colortex.cn

[S58] C++：命名空间
来源：http://lw.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://bk.jctech888.com.cn

[S59] C++：静态断言
来源：http://oy.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lk.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://lk.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qo.jianghongdianzi.cn

================================================================================
来源：http://qh.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ji.panjiajie.cn

================================================================================
来源：http://oo.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://mf.shxzskj.cn

println("Hello")
来源：http://kp.jctech888.com.cn

[T02] Kotlin：变量
来源：http://mn.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tl.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://wq.newstarts.cn

"值: $b"
来源：http://dd.nszjky.cn

[T04] Kotlin：空安全
来源：http://kj.asd995.cn

val n: String? = null;  n?.length
来源：http://bc.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://zw.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jk.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://pn.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fa.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://dr.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ek.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://jx.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://xr.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://mi.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://gh.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://aw.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wb.szsharing.cn

[T11] Kotlin：协程
来源：http://ur.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uu.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://oh.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://pv.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://hj.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://ep.shxzukj.cn

[T14] Kotlin：循环
来源：http://pg.9csxet.cn

for (i in 1..10) println(i)
来源：http://zv.bjjhwx.cn

[T15] Kotlin：接口
来源：http://ec.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://yh.szxytkj.cn

[T16] Swift：Hello World
来源：http://ev.szxytkj.cn

print("Hello")
来源：http://ho.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://ja.gzmigu.cn

var a = 1;  let b = 2
来源：http://bw.colortex.cn

[T18] Swift：字符串插值
来源：http://es.shtwfgs.cn

"值: \(b)"
来源：http://jt.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://ea.gzmigu.cn

if let n = opt { print(n) }
来源：http://iv.nicolike.cn

[T20] Swift：数组操作
来源：http://au.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://le.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://jd.szsharing.cn

for x in a { print(x) }
来源：http://ql.asd995.cn

[T22] Swift：字典
来源：http://jp.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zy.yuntaijiaju.cn

[T23] Swift：函数
来源：http://ly.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ci.bjjhwx.cn

[T24] Swift：闭包
来源：http://cl.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zs.nicolike.cn

[T25] Swift：结构体
来源：http://tj.wgjwhj.cn

struct P { var x: Int }
来源：http://my.bjjhwx.cn

[T26] Swift：类与重写
来源：http://qy.muxihuayi.cn

class A: Base { override func f() {} }
来源：http://ng.lnxyls.cn

[T27] Swift：错误处理
来源：http://qf.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://gr.haigaiapp.cn

[T28] Swift：枚举
来源：http://pj.panjiajie.cn

enum Color { case red, green }
来源：http://gt.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://rz.shxzskj.cn

guard let x = opt else { return }
来源：http://bv.nicolike.cn

[T30] Swift：协议
来源：http://wr.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://ir.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://yn.muxihuayi.cn

print("Hello")
来源：http://ov.yuexingan06.cn

[T32] Lua：局部变量
来源：http://rf.bjjhwx.cn

local a = 1
来源：http://ex.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://mz.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vz.muxihuayi.cn

[T34] Lua：遍历表
来源：http://ac.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vc.gzmigu.cn

[T35] Lua：字典表
来源：http://rd.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://qm.colortex.cn

[T36] Lua：函数
来源：http://bb.szsharing.cn

function add(a, b) return a + b end
来源：http://ay.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://uo.szsharing.cn

"a" .. "b"
来源：http://vu.521024.cn

[T38] Lua：条件
来源：http://mf.9csxet.cn

if x > 0 then print("正") end
来源：http://yr.huanxung.cn

[T39] Lua：模式匹配
来源：http://nc.asd995.cn

string.find(s, "%d+")
来源：http://hk.shxzskj.cn

[T40] Lua：元表
来源：http://lq.hahajie.cn

setmetatable({}, { __index = base })
来源：http://xd.huixiangedu.cn

[T41] Perl：Hello World
来源：http://cj.colortex.cn

print "Hello\n";
来源：http://hb.szsharing.cn

[T42] Perl：变量类型
来源：http://tl.huanxung.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jp.szxytkj.cn

[T43] Perl：字符串插值
来源：http://jt.bjjhwx.cn

"值: $a"
来源：http://sh.chemitech.net.cn

[T44] Perl：条件
来源：http://em.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://bu.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://sn.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://cs.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://dx.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pd.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ix.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bu.jctech888.com.cn

[T48] Perl：正则替换
来源：http://qk.nszjky.cn

$s =~ s/old/new/g;
来源：http://uj.gzmigu.cn

[T49] Perl：函数
来源：http://cz.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jr.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://yn.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://or.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://bl.jctech888.com.cn

[T51] Scala：Hello World
来源：http://rh.panjiajie.cn

println("Hello")
来源：http://te.newstarts.cn

[T52] Scala：变量
来源：http://yk.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://by.hahajie.cn

[T53] Scala：字符串插值
来源：http://iw.shxzskj.cn

s"值: $b"
来源：http://tv.hahajie.cn

[T54] Scala：集合映射
来源：http://pv.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://rf.hnjuh.cn

[T55] Scala：集合过滤
来源：http://dq.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hb.gzmigu.cn

[T56] Scala：样例类
来源：http://fk.hnjuh.cn

case class User(name: String, age: Int)
来源：http://qa.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://rn.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yp.bjjhwx.cn

[T58] Scala：函数定义
来源：http://qz.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kl.haigaiapp.cn

[T59] Scala：循环
来源：http://it.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://hd.gzmigu.cn

[T60] Scala：折叠
来源：http://ws.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ec.jctech888.com.cn

================================================================================
来源：http://go.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gf.chemitech.net.cn

================================================================================
来源：http://wc.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://vy.jianghongdianzi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kp.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://mz.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yq.asd995.cn

[U03] Py：加载 .env 配置
来源：http://xg.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fv.shxzskj.cn

[U04] Py：变量调试打印
来源：http://og.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vy.huanxung.cn

[U05] Py：列表去重且保序
来源：http://ng.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://io.gzmigu.cn

[U06] Py：合并两个字典
来源：http://vf.nicolike.cn

{**a, **b}
来源：http://sx.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://db.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://yc.lnxyls.cn

[U08] Py：展平二维列表
来源：http://wy.panjiajie.cn

[y for x in nested for y in x]
来源：http://qu.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://cc.shtwfgs.cn

max(d, key=d.get)
来源：http://wz.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://dn.szsharing.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ys.shxzskj.cn

[U11] Py：生成器表达式
来源：http://fb.panjiajie.cn

(x * 2 for x in arr)
来源：http://mj.bjjhwx.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ti.yuntaijiaju.cn

Counter(arr).most_common(3)
来源：http://vq.panjiajie.cn

[U13] Py：固定长度队列
来源：http://jr.chemitech.net.cn

deque(maxlen=10)
来源：http://na.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://an.hahajie.cn

defaultdict(list)
来源：http://ce.bjjhwx.cn

[U15] Py：高精度计时
来源：http://lb.huixinmuqiang.cn

t = time.perf_counter()
来源：http://tk.bookmarksfly.cn

[U16] Py：命令行参数解析
来源：http://fd.jianghongdianzi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://st.wgjwhj.cn

[U17] Py：初始化日志
来源：http://ay.hnjuh.cn

logging.basicConfig(level=logging.INFO)
来源：http://ds.haigaiapp.cn

[U18] Py：预编译正则
来源：http://xg.9csxet.cn

pat = re.compile(r"\d+")
来源：http://os.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://pw.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xp.huanxung.cn

[U20] Py：缓存函数结果
来源：http://jy.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://kx.521024.cn

[U21] Py：自定义上下文管理器
来源：http://px.panjiajie.cn

@contextlib.contextmanager
来源：http://js.jianghongdianzi.cn

[U22] Py：矩阵转置
来源：http://de.asd995.cn

list(zip(*m))
来源：http://xe.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://kw.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ni.bjjhwx.cn

[U24] Py：路径操作
来源：http://yu.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lf.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://hx.jctech888.com.cn

csv.DictReader(f)
来源：http://le.bjjhwx.cn

[U26] Py：并发下载
来源：http://gz.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nz.nszjky.cn

[U27] Py：异步 HTTP
来源：http://ps.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ui.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://co.szsharing.cn

UserId = int
来源：http://je.nicolike.cn

[U29] Py：属性校验
来源：http://im.hahajie.cn

@property 与 @x.setter 配合
来源：http://jq.panjiajie.cn

[U30] Py：数据类
来源：http://rw.521024.cn

@dataclass(slots=True)
来源：http://yw.chemitech.net.cn

[U31] Py：单测
来源：http://rm.hnjuh.cn

python -m pytest -q
来源：http://az.asd995.cn

[U32] Py：代码格式化
来源：http://ic.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://vv.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://yy.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://xj.lnxyls.cn

[U34] Py：判断编码
来源：http://mc.shtwfgs.cn

chardet.detect(raw)
来源：http://zr.hahajie.cn

[U35] Py：发送邮件
来源：http://uq.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mi.asd995.cn

[U36] Py：定时任务
来源：http://jt.521024.cn

schedule.every(10).minutes.do(job)
来源：http://aw.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://gf.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ob.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://vz.szxytkj.cn

Path(__file__).resolve().parent
来源：http://hb.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://bb.muxihuayi.cn

sys.stdout.isatty()
来源：http://vl.muxihuayi.cn

[U40] Py：打印到标准错误
来源：http://qw.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://hd.bookmarksfly.cn

[U41] PHP：初始化 Composer 项目
来源：http://ll.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://za.szsharing.cn

[U42] PHP：PSR-4 自动加载
来源：http://ej.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ko.bjjhwx.cn

[U43] PHP：声明命名空间
来源：http://rx.shtwfgs.cn

namespace App\Http;
来源：http://xi.muxihuayi.cn

[U44] PHP：开启严格类型
来源：http://bq.shxzukj.cn

declare(strict_types=1);
来源：http://iy.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://vi.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xl.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://cx.jianghongdianzi.cn

?string $name = null
来源：http://ei.szxytkj.cn

[U47] PHP：联合类型
来源：http://sy.newstarts.cn

int|string $id
来源：http://ul.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://ox.hnjuh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vz.newstarts.cn

[U49] PHP：只读属性
来源：http://rm.shxzukj.cn

public readonly string $name
来源：http://cx.lnxyls.cn

[U50] PHP：构造器属性提升
来源：http://mn.hahajie.cn

public function __construct(private int $id) {}
来源：http://ht.szsharing.cn

[U51] PHP：数组解构
来源：http://dd.colortex.cn

[$a, $b] = $arr;
来源：http://fh.huanxung.cn

[U52] PHP：箭头函数
来源：http://ok.hnjuh.cn

$double = fn($x) => $x * 2;
来源：http://qm.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://jk.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://mg.colortex.cn

[U54] PHP：空安全调用
来源：http://or.colortex.cn

$obj?->method()
来源：http://di.gzmigu.cn

[U55] PHP：match 表达式
来源：http://gz.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tu.nszjky.cn

[U56] PHP：命名参数
来源：http://wy.panjiajie.cn

f(a: 1, b: 2)
来源：http://nm.hahajie.cn


<!-- 参考信息 -->