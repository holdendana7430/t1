代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ur.nicolike.cn

[S25] C：内存拷贝
来源：http://rg.521024.cn

memcpy(dst, src, n);
来源：http://ax.colortex.cn

[S26] C：内存清零
来源：http://ip.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://io.huixinmuqiang.cn

[S27] C：定义常量
来源：http://it.shxzskj.cn

const double PI = 3.14159;
来源：http://sn.9csxet.cn

[S28] C：静态变量
来源：http://hc.szxytkj.cn

static int counter = 0;
来源：http://tq.chemitech.net.cn

[S29] C：变参函数
来源：http://ym.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dt.szxytkj.cn

[S30] C：头文件保护
来源：http://pc.lnxyls.cn

#ifndef X_H
来源：http://mo.colortex.cn

#define X_H
来源：http://uj.521024.cn

#endif
来源：http://xp.jctech888.com.cn

[S31] C++：Hello World
来源：http://um.bjjhwx.cn

#include <iostream>
来源：http://uj.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://xd.lnxyls.cn

[S32] C++：字符串
来源：http://vk.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://xc.lnxyls.cn

[S33] C++：vector 增删
来源：http://vr.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ec.gzmigu.cn

[S34] C++：遍历 vector
来源：http://zo.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ms.huanxung.cn

[S35] C++：map
来源：http://gf.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wp.wgjwhj.cn

[S36] C++：unordered_map
来源：http://iu.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kx.huanxung.cn

[S37] C++：set
来源：http://rs.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tl.chemitech.net.cn

[S38] C++：排序
来源：http://bo.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://le.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://hc.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ob.szsharing.cn

[S40] C++：查找元素
来源：http://pv.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zz.nicolike.cn

[S41] C++：类与构造函数
来源：http://bd.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oq.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://sm.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://yd.newstarts.cn

[S43] C++：智能指针
来源：http://gw.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://zf.muxihuayi.cn

[S44] C++：引用传参
来源：http://jn.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://ui.hnjuh.cn

[S45] C++：lambda
来源：http://ih.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jy.muxihuayi.cn

[S46] C++：函数模板
来源：http://uz.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kr.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://un.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sd.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ky.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iz.huanxung.cn

while (std::getline(in, line)) { }
来源：http://py.huixiangedu.cn

[S49] C++：写文件
来源：http://gr.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://te.shxzskj.cn

[S50] C++：格式化数字
来源：http://oz.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gk.panjiajie.cn

[S51] C++：显式类型转换
来源：http://qp.huixiangedu.cn

static_cast<double>(a) / b
来源：http://ax.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://nb.521024.cn

int size() const noexcept { return n_; }
来源：http://qt.521024.cn

[S53] C++：移动语义
来源：http://ts.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://ss.shxzukj.cn

[S54] C++：异常处理
来源：http://vm.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fo.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://qp.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://by.gzmigu.cn

[S56] C++：optional
来源：http://wu.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ly.yuexingan06.cn

[S57] C++：编译期常量
来源：http://oy.nszjky.cn

constexpr int N = 10;
来源：http://fp.asd995.cn

[S58] C++：命名空间
来源：http://vd.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://lb.muxihuayi.cn

[S59] C++：静态断言
来源：http://mk.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fq.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://hg.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ob.szsharing.cn

================================================================================
来源：http://fl.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ij.muxihuayi.cn

================================================================================
来源：http://mi.szsharing.cn

[T01] Kotlin：Hello World
来源：http://sn.yuexingan06.cn

println("Hello")
来源：http://ae.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://wu.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cq.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://jj.yuntaijiaju.cn

"值: $b"
来源：http://wu.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://ls.colortex.cn

val n: String? = null;  n?.length
来源：http://mp.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://iz.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uw.asd995.cn

[T06] Kotlin：集合映射
来源：http://xa.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kc.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://eh.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ju.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://oj.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://hg.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://zl.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://up.9csxet.cn

[T10] Kotlin：默认参数
来源：http://fw.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sk.hnjuh.cn

[T11] Kotlin：协程
来源：http://dd.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ti.szsharing.cn

[T12] Kotlin：解构声明
来源：http://oa.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://nz.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://gs.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://mq.bjjhwx.cn

[T14] Kotlin：循环
来源：http://vy.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ly.asd995.cn

[T15] Kotlin：接口
来源：http://ne.nszjky.cn

interface Shape { fun area(): Double }
来源：http://oc.colortex.cn

[T16] Swift：Hello World
来源：http://oq.shtwfgs.cn

print("Hello")
来源：http://kw.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://ev.bjjhwx.cn

var a = 1;  let b = 2
来源：http://el.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://gb.shxzskj.cn

"值: \(b)"
来源：http://nb.huanxung.cn

[T19] Swift：可选绑定
来源：http://tu.gzmigu.cn

if let n = opt { print(n) }
来源：http://vb.hahajie.cn

[T20] Swift：数组操作
来源：http://tz.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bv.chemitech.net.cn

[T21] Swift：遍历
来源：http://rw.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ke.huixinmuqiang.cn

[T22] Swift：字典
来源：http://os.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kh.haigaiapp.cn

[T23] Swift：函数
来源：http://rr.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ju.colortex.cn

[T24] Swift：闭包
来源：http://yx.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ig.szsharing.cn

[T25] Swift：结构体
来源：http://eg.colortex.cn

struct P { var x: Int }
来源：http://gm.nicolike.cn

[T26] Swift：类与重写
来源：http://ps.newstarts.cn

class A: Base { override func f() {} }
来源：http://dy.shxzukj.cn

[T27] Swift：错误处理
来源：http://fl.hahajie.cn

do { try f() } catch { print(error) }
来源：http://fj.hnjuh.cn

[T28] Swift：枚举
来源：http://gb.yuexingan06.cn

enum Color { case red, green }
来源：http://ew.colortex.cn

[T29] Swift：guard 提前返回
来源：http://yo.jctech888.com.cn

guard let x = opt else { return }
来源：http://ub.9csxet.cn

[T30] Swift：协议
来源：http://zq.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://mc.nszjky.cn

[T31] Lua：Hello World
来源：http://xj.hahajie.cn

print("Hello")
来源：http://jq.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://oh.chemitech.net.cn

local a = 1
来源：http://pb.asd995.cn

[T33] Lua：表（数组）
来源：http://pp.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gm.haigaiapp.cn

[T34] Lua：遍历表
来源：http://xn.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ol.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://td.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://wh.lnxyls.cn

[T36] Lua：函数
来源：http://fx.szsharing.cn

function add(a, b) return a + b end
来源：http://iv.asd995.cn

[T37] Lua：字符串拼接
来源：http://jj.gzmigu.cn

"a" .. "b"
来源：http://nj.szsharing.cn

[T38] Lua：条件
来源：http://ug.szxytkj.cn

if x > 0 then print("正") end
来源：http://lc.asd995.cn

[T39] Lua：模式匹配
来源：http://ai.wgjwhj.cn

string.find(s, "%d+")
来源：http://kd.colortex.cn

[T40] Lua：元表
来源：http://dr.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://vq.521024.cn

[T41] Perl：Hello World
来源：http://xh.newstarts.cn

print "Hello\n";
来源：http://mv.muxihuayi.cn

[T42] Perl：变量类型
来源：http://nn.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bi.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://tj.haigaiapp.cn

"值: $a"
来源：http://zv.shxzskj.cn

[T44] Perl：条件
来源：http://bm.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://on.hahajie.cn

[T45] Perl：数组遍历
来源：http://zc.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://bm.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://hp.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vw.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://og.jianghongdianzi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qr.gzmigu.cn

[T48] Perl：正则替换
来源：http://yi.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://ri.chemitech.net.cn

[T49] Perl：函数
来源：http://od.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pc.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://zn.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pe.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://je.wgjwhj.cn

[T51] Scala：Hello World
来源：http://pi.521024.cn

println("Hello")
来源：http://yo.haigaiapp.cn

[T52] Scala：变量
来源：http://sh.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://ha.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://fk.szxytkj.cn

s"值: $b"
来源：http://yf.muxihuayi.cn

[T54] Scala：集合映射
来源：http://hm.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://fx.nicolike.cn

[T55] Scala：集合过滤
来源：http://zl.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ts.huanxung.cn

[T56] Scala：样例类
来源：http://tw.gzmigu.cn

case class User(name: String, age: Int)
来源：http://fy.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://xw.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cv.9csxet.cn

[T58] Scala：函数定义
来源：http://zg.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jo.colortex.cn

[T59] Scala：循环
来源：http://oi.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://ur.muxihuayi.cn

[T60] Scala：折叠
来源：http://iy.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ev.shtwfgs.cn

================================================================================
来源：http://lx.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gc.szsharing.cn

================================================================================
来源：http://qr.bookmarksfly.cn

[U01] Py：创建虚拟环境
来源：http://gs.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sb.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://sh.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ib.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://yt.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qi.yuexingan06.cn

[U04] Py：变量调试打印
来源：http://ir.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vt.521024.cn

[U05] Py：列表去重且保序
来源：http://dr.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://xu.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://ci.huixiangedu.cn

{**a, **b}
来源：http://zr.newstarts.cn

[U07] Py：反转字典键值
来源：http://li.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://cd.shxzukj.cn

[U08] Py：展平二维列表
来源：http://pg.gzmigu.cn

[y for x in nested for y in x]
来源：http://pu.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://cu.hahajie.cn

max(d, key=d.get)
来源：http://hm.panjiajie.cn

[U10] Py：按值排序字典
来源：http://np.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yl.chemitech.net.cn

[U11] Py：生成器表达式
来源：http://zi.lnxyls.cn

(x * 2 for x in arr)
来源：http://ve.gzmigu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qu.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://ic.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://ch.521024.cn

deque(maxlen=10)
来源：http://vg.chemitech.net.cn

[U14] Py：分组收集到列表
来源：http://xk.huixinmuqiang.cn

defaultdict(list)
来源：http://tp.shxzukj.cn

[U15] Py：高精度计时
来源：http://kt.szsharing.cn

t = time.perf_counter()
来源：http://ht.9csxet.cn

[U16] Py：命令行参数解析
来源：http://sf.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://my.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://yq.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://tm.lnxyls.cn

[U18] Py：预编译正则
来源：http://qr.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://tm.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://kq.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vd.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://te.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ai.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://ps.chemitech.net.cn

@contextlib.contextmanager
来源：http://on.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://bi.colortex.cn

list(zip(*m))
来源：http://tf.hahajie.cn

[U23] Py：分块读取大文件
来源：http://vo.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vu.newstarts.cn

[U24] Py：路径操作
来源：http://bk.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xd.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://te.521024.cn

csv.DictReader(f)
来源：http://rb.szsharing.cn

[U26] Py：并发下载
来源：http://bk.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mz.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://jh.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://vt.gzmigu.cn

[U28] Py：类型别名
来源：http://oj.colortex.cn

UserId = int
来源：http://gw.muxihuayi.cn

[U29] Py：属性校验
来源：http://rb.newstarts.cn

@property 与 @x.setter 配合
来源：http://fs.haigaiapp.cn

[U30] Py：数据类
来源：http://ph.asd995.cn

@dataclass(slots=True)
来源：http://bk.bookmarksfly.cn

[U31] Py：单测
来源：http://yo.lnxyls.cn

python -m pytest -q
来源：http://rm.gzmigu.cn

[U32] Py：代码格式化
来源：http://ja.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://ud.shxzukj.cn

[U33] Py：打包发布
来源：http://zo.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://zc.wgjwhj.cn

[U34] Py：判断编码
来源：http://aj.bookmarksfly.cn

chardet.detect(raw)
来源：http://yt.shxzskj.cn

[U35] Py：发送邮件
来源：http://fx.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xh.shxzskj.cn

[U36] Py：定时任务
来源：http://gc.521024.cn

schedule.every(10).minutes.do(job)
来源：http://qx.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://rf.shxzukj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xu.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://ni.jctech888.com.cn

Path(__file__).resolve().parent
来源：http://mk.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://lf.nicolike.cn

sys.stdout.isatty()
来源：http://lt.521024.cn

[U40] Py：打印到标准错误
来源：http://gj.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://dq.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://pq.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cq.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://zq.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jw.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://ih.shxzskj.cn

namespace App\Http;
来源：http://if.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://lc.newstarts.cn

declare(strict_types=1);
来源：http://ur.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://bq.bookmarksfly.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sd.szsharing.cn

[U46] PHP：可空类型
来源：http://jp.521024.cn

?string $name = null
来源：http://wd.shxzukj.cn

[U47] PHP：联合类型
来源：http://pq.9csxet.cn

int|string $id
来源：http://bg.hnjuh.cn

[U48] PHP：纯枚举
来源：http://kq.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://af.huixiangedu.cn


<!-- 参考信息 -->