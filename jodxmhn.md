代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://mx.bookmarksfly.cn

[S23] C：随机数
来源：http://kh.hahajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xt.huixinmuqiang.cn

[S24] C：获取本地时间
来源：http://cz.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wi.haigaiapp.cn

[S25] C：内存拷贝
来源：http://md.lnxyls.cn

memcpy(dst, src, n);
来源：http://oo.bjjhwx.cn

[S26] C：内存清零
来源：http://dm.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://jy.szsharing.cn

[S27] C：定义常量
来源：http://mo.panjiajie.cn

const double PI = 3.14159;
来源：http://yh.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ol.hahajie.cn

static int counter = 0;
来源：http://yt.9csxet.cn

[S29] C：变参函数
来源：http://jk.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ld.hahajie.cn

[S30] C：头文件保护
来源：http://cs.hnjuh.cn

#ifndef X_H
来源：http://nx.asd995.cn

#define X_H
来源：http://lw.jianghongdianzi.cn

#endif
来源：http://nh.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://ua.shtwfgs.cn

#include <iostream>
来源：http://ai.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://el.huanxung.cn

[S32] C++：字符串
来源：http://sd.nicolike.cn

std::string s = "hi";  s += "!";
来源：http://zf.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://hn.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cr.gzmigu.cn

[S34] C++：遍历 vector
来源：http://vb.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://qa.szxytkj.cn

[S35] C++：map
来源：http://na.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wi.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://vb.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yc.bjjhwx.cn

[S37] C++：set
来源：http://ti.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yb.haigaiapp.cn

[S38] C++：排序
来源：http://pj.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://xe.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://dz.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mb.lnxyls.cn

[S40] C++：查找元素
来源：http://ds.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hm.panjiajie.cn

[S41] C++：类与构造函数
来源：http://ex.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sj.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://nr.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://nb.hahajie.cn

[S43] C++：智能指针
来源：http://yj.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://ia.huanxung.cn

[S44] C++：引用传参
来源：http://it.newstarts.cn

void inc(int &x) { ++x; }
来源：http://zl.colortex.cn

[S45] C++：lambda
来源：http://oj.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://si.521024.cn

[S46] C++：函数模板
来源：http://tj.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rx.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://fi.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://af.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://ru.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hv.yuexingan06.cn

while (std::getline(in, line)) { }
来源：http://oo.asd995.cn

[S49] C++：写文件
来源：http://ju.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qi.asd995.cn

[S50] C++：格式化数字
来源：http://ap.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jk.szxytkj.cn

[S51] C++：显式类型转换
来源：http://vo.hnjuh.cn

static_cast<double>(a) / b
来源：http://yt.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://pp.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://in.muxihuayi.cn

[S53] C++：移动语义
来源：http://pu.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://pm.bjjhwx.cn

[S54] C++：异常处理
来源：http://mw.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://be.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://br.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ub.yuntaijiaju.cn

[S56] C++：optional
来源：http://zz.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zn.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://pr.shtwfgs.cn

constexpr int N = 10;
来源：http://va.colortex.cn

[S58] C++：命名空间
来源：http://lx.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://ya.chemitech.net.cn

[S59] C++：静态断言
来源：http://jt.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rs.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://hi.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://al.hahajie.cn

================================================================================
来源：http://rf.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ue.szxytkj.cn

================================================================================
来源：http://wh.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://rl.shtwfgs.cn

println("Hello")
来源：http://ef.colortex.cn

[T02] Kotlin：变量
来源：http://tu.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sl.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://re.nszjky.cn

"值: $b"
来源：http://ap.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://uf.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://ee.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://qy.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fp.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://ul.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://he.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://dm.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qg.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://ze.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://oh.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://ic.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://tl.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://re.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://th.nicolike.cn

[T11] Kotlin：协程
来源：http://uy.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yj.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://eo.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://dx.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://gq.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://jk.shxzskj.cn

[T14] Kotlin：循环
来源：http://it.szxytkj.cn

for (i in 1..10) println(i)
来源：http://yu.9csxet.cn

[T15] Kotlin：接口
来源：http://pk.nicolike.cn

interface Shape { fun area(): Double }
来源：http://sd.shtwfgs.cn

[T16] Swift：Hello World
来源：http://vo.panjiajie.cn

print("Hello")
来源：http://vp.hahajie.cn

[T17] Swift：变量与常量
来源：http://ag.gzmigu.cn

var a = 1;  let b = 2
来源：http://be.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://jz.shtwfgs.cn

"值: \(b)"
来源：http://cz.huanxung.cn

[T19] Swift：可选绑定
来源：http://xz.bjjhwx.cn

if let n = opt { print(n) }
来源：http://mc.chemitech.net.cn

[T20] Swift：数组操作
来源：http://eb.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wh.haigaiapp.cn

[T21] Swift：遍历
来源：http://lb.nszjky.cn

for x in a { print(x) }
来源：http://bb.yuexingan06.cn

[T22] Swift：字典
来源：http://li.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wa.shxzskj.cn

[T23] Swift：函数
来源：http://ud.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yo.jctech888.com.cn

[T24] Swift：闭包
来源：http://bd.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qs.jctech888.com.cn

[T25] Swift：结构体
来源：http://jt.panjiajie.cn

struct P { var x: Int }
来源：http://bw.lnxyls.cn

[T26] Swift：类与重写
来源：http://um.hnjuh.cn

class A: Base { override func f() {} }
来源：http://ee.newstarts.cn

[T27] Swift：错误处理
来源：http://mg.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://md.chemitech.net.cn

[T28] Swift：枚举
来源：http://ss.9csxet.cn

enum Color { case red, green }
来源：http://vk.colortex.cn

[T29] Swift：guard 提前返回
来源：http://rd.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://xw.nicolike.cn

[T30] Swift：协议
来源：http://aj.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://bs.haigaiapp.cn

[T31] Lua：Hello World
来源：http://iq.wgjwhj.cn

print("Hello")
来源：http://yv.hnjuh.cn

[T32] Lua：局部变量
来源：http://tf.huixinmuqiang.cn

local a = 1
来源：http://bo.shxzukj.cn

[T33] Lua：表（数组）
来源：http://qn.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sc.hnjuh.cn

[T34] Lua：遍历表
来源：http://ua.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kx.wgjwhj.cn

[T35] Lua：字典表
来源：http://zl.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://oc.wgjwhj.cn

[T36] Lua：函数
来源：http://iy.huanxung.cn

function add(a, b) return a + b end
来源：http://gc.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://uy.nszjky.cn

"a" .. "b"
来源：http://km.jianghongdianzi.cn

[T38] Lua：条件
来源：http://ml.newstarts.cn

if x > 0 then print("正") end
来源：http://ux.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://xa.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://hh.huanxung.cn

[T40] Lua：元表
来源：http://si.hahajie.cn

setmetatable({}, { __index = base })
来源：http://ct.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://av.jianghongdianzi.cn

print "Hello\n";
来源：http://sw.hnjuh.cn

[T42] Perl：变量类型
来源：http://ai.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ds.shxzskj.cn

[T43] Perl：字符串插值
来源：http://nl.gzmigu.cn

"值: $a"
来源：http://hw.yuexingan06.cn

[T44] Perl：条件
来源：http://ax.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://di.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://wp.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://ra.nicolike.cn

[T46] Perl：哈希操作
来源：http://pc.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ji.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://dx.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rk.huixinmuqiang.cn

[T48] Perl：正则替换
来源：http://xb.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://fk.bookmarksfly.cn

[T49] Perl：函数
来源：http://wn.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tl.huanxung.cn

[T50] Perl：逐行读文件
来源：http://gp.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ge.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://mu.shtwfgs.cn

[T51] Scala：Hello World
来源：http://xt.szxytkj.cn

println("Hello")
来源：http://qt.hnjuh.cn

[T52] Scala：变量
来源：http://zz.muxihuayi.cn

val a = 1;  var b = 2
来源：http://ss.panjiajie.cn

[T53] Scala：字符串插值
来源：http://mz.szsharing.cn

s"值: $b"
来源：http://zy.yuexingan06.cn

[T54] Scala：集合映射
来源：http://le.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://tf.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://nd.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ks.newstarts.cn

[T56] Scala：样例类
来源：http://kz.521024.cn

case class User(name: String, age: Int)
来源：http://pp.lnxyls.cn

[T57] Scala：模式匹配
来源：http://kg.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ik.9csxet.cn

[T58] Scala：函数定义
来源：http://kn.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vc.haigaiapp.cn

[T59] Scala：循环
来源：http://zw.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://id.huanxung.cn

[T60] Scala：折叠
来源：http://ua.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cd.szsharing.cn

================================================================================
来源：http://ya.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kk.haigaiapp.cn

================================================================================
来源：http://nn.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://vz.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yc.nszjky.cn

[U02] Py：导出 / 安装依赖
来源：http://ot.nicolike.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ce.gzmigu.cn

[U03] Py：加载 .env 配置
来源：http://hx.nszjky.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://br.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://nv.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ov.huanxung.cn

[U05] Py：列表去重且保序
来源：http://hj.nicolike.cn

list(dict.fromkeys(arr))
来源：http://dr.huixiangedu.cn

[U06] Py：合并两个字典
来源：http://dk.gzmigu.cn

{**a, **b}
来源：http://su.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://xy.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://jk.hahajie.cn

[U08] Py：展平二维列表
来源：http://dy.nszjky.cn

[y for x in nested for y in x]
来源：http://za.jctech888.com.cn

[U09] Py：字典取最大值的键
来源：http://xa.lnxyls.cn

max(d, key=d.get)
来源：http://ur.asd995.cn

[U10] Py：按值排序字典
来源：http://er.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bq.haigaiapp.cn

[U11] Py：生成器表达式
来源：http://ao.panjiajie.cn

(x * 2 for x in arr)
来源：http://lb.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qk.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://er.szsharing.cn

[U13] Py：固定长度队列
来源：http://ze.shxzukj.cn

deque(maxlen=10)
来源：http://yt.jctech888.com.cn

[U14] Py：分组收集到列表
来源：http://jd.haigaiapp.cn

defaultdict(list)
来源：http://lk.nicolike.cn

[U15] Py：高精度计时
来源：http://qs.newstarts.cn

t = time.perf_counter()
来源：http://hp.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://gl.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ms.521024.cn

[U17] Py：初始化日志
来源：http://gy.haigaiapp.cn

logging.basicConfig(level=logging.INFO)
来源：http://oh.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://tu.9csxet.cn

pat = re.compile(r"\d+")
来源：http://wg.newstarts.cn

[U19] Py：正则替换带回调
来源：http://zz.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gc.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://ok.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://je.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://wj.nicolike.cn

@contextlib.contextmanager
来源：http://cs.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://tr.nszjky.cn

list(zip(*m))
来源：http://xf.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://lt.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ud.wgjwhj.cn

[U24] Py：路径操作
来源：http://ha.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gv.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://at.chemitech.net.cn

csv.DictReader(f)
来源：http://tb.huanxung.cn

[U26] Py：并发下载
来源：http://sr.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sx.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://dy.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://us.521024.cn

[U28] Py：类型别名
来源：http://at.9csxet.cn

UserId = int
来源：http://um.haigaiapp.cn

[U29] Py：属性校验
来源：http://rv.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://tk.panjiajie.cn

[U30] Py：数据类
来源：http://sx.nicolike.cn

@dataclass(slots=True)
来源：http://ir.hnjuh.cn

[U31] Py：单测
来源：http://zy.hnjuh.cn

python -m pytest -q
来源：http://gq.yuexingan06.cn

[U32] Py：代码格式化
来源：http://rn.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://fd.nszjky.cn

[U33] Py：打包发布
来源：http://np.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://hb.bookmarksfly.cn

[U34] Py：判断编码
来源：http://ho.newstarts.cn

chardet.detect(raw)
来源：http://cs.nszjky.cn

[U35] Py：发送邮件
来源：http://sf.chemitech.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://at.nszjky.cn

[U36] Py：定时任务
来源：http://qx.nicolike.cn

schedule.every(10).minutes.do(job)
来源：http://pv.colortex.cn

[U37] Py：读写 Excel
来源：http://fl.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vm.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://ft.newstarts.cn

Path(__file__).resolve().parent
来源：http://fk.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://ma.hnjuh.cn

sys.stdout.isatty()
来源：http://ji.chemitech.net.cn

[U40] Py：打印到标准错误
来源：http://pp.lnxyls.cn

print("err", file=sys.stderr)
来源：http://pz.szsharing.cn

[U41] PHP：初始化 Composer 项目
来源：http://xi.huanxung.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yz.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://sx.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vj.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://yn.bjjhwx.cn

namespace App\Http;
来源：http://ya.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://bw.wgjwhj.cn

declare(strict_types=1);
来源：http://km.wgjwhj.cn

[U45] PHP：类型声明与返回类型
来源：http://gs.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://es.panjiajie.cn

[U46] PHP：可空类型
来源：http://ms.lnxyls.cn

?string $name = null
来源：http://tw.asd995.cn


<!-- 参考信息 -->