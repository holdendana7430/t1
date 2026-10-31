代发 wailian999

int main(int argc, char **argv)
来源：http://eg.nszjky.cn

[S19] C：快速排序
来源：http://td.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ke.hahajie.cn

[S20] C：二分查找
来源：http://la.panjiajie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wb.jctech888.com.cn

[S21] C：字符类别判断
来源：http://tr.panjiajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://te.nicolike.cn

[S22] C：字符串转数字
来源：http://fr.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vx.szsharing.cn

[S23] C：随机数
来源：http://rp.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vc.newstarts.cn

[S24] C：获取本地时间
来源：http://da.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cf.asd995.cn

[S25] C：内存拷贝
来源：http://ch.panjiajie.cn

memcpy(dst, src, n);
来源：http://ln.shtwfgs.cn

[S26] C：内存清零
来源：http://oh.asd995.cn

memset(a, 0, sizeof a);
来源：http://sx.huixinmuqiang.cn

[S27] C：定义常量
来源：http://nw.asd995.cn

const double PI = 3.14159;
来源：http://ks.haigaiapp.cn

[S28] C：静态变量
来源：http://rl.huixinmuqiang.cn

static int counter = 0;
来源：http://eg.9csxet.cn

[S29] C：变参函数
来源：http://bl.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vu.gzmigu.cn

[S30] C：头文件保护
来源：http://jy.yuexingan06.cn

#ifndef X_H
来源：http://fm.9csxet.cn

#define X_H
来源：http://mq.shxzukj.cn

#endif
来源：http://wn.huixiangedu.cn

[S31] C++：Hello World
来源：http://lx.jctech888.com.cn

#include <iostream>
来源：http://yv.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://lk.yuntaijiaju.cn

[S32] C++：字符串
来源：http://to.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://hf.muxihuayi.cn

[S33] C++：vector 增删
来源：http://ga.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ef.wgjwhj.cn

[S34] C++：遍历 vector
来源：http://fv.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://cn.asd995.cn

[S35] C++：map
来源：http://ip.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ng.szsharing.cn

[S36] C++：unordered_map
来源：http://ez.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wu.wgjwhj.cn

[S37] C++：set
来源：http://bv.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://up.huixinmuqiang.cn

[S38] C++：排序
来源：http://nb.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://gv.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://ul.szsharing.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pa.hnjuh.cn

[S40] C++：查找元素
来源：http://wu.jianghongdianzi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bp.hahajie.cn

[S41] C++：类与构造函数
来源：http://rq.jctech888.com.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vx.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://wr.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://oh.szsharing.cn

[S43] C++：智能指针
来源：http://yr.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://jf.yuexingan06.cn

[S44] C++：引用传参
来源：http://cp.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ko.yuexingan06.cn

[S45] C++：lambda
来源：http://dl.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hh.nicolike.cn

[S46] C++：函数模板
来源：http://is.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://is.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://kh.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ww.521024.cn

[S48] C++：逐行读文件
来源：http://bx.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nv.newstarts.cn

while (std::getline(in, line)) { }
来源：http://zs.hnjuh.cn

[S49] C++：写文件
来源：http://no.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eg.bjjhwx.cn

[S50] C++：格式化数字
来源：http://iy.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hb.huixiangedu.cn

[S51] C++：显式类型转换
来源：http://eh.huanxung.cn

static_cast<double>(a) / b
来源：http://na.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://md.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://zk.huanxung.cn

[S53] C++：移动语义
来源：http://bb.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://fq.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://eb.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lr.shxzskj.cn

[S55] C++：结构化绑定
来源：http://cf.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oq.shtwfgs.cn

[S56] C++：optional
来源：http://bg.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ub.521024.cn

[S57] C++：编译期常量
来源：http://pq.shxzukj.cn

constexpr int N = 10;
来源：http://jn.yuexingan06.cn

[S58] C++：命名空间
来源：http://vu.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://ug.huanxung.cn

[S59] C++：静态断言
来源：http://hd.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tk.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://zq.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rj.wgjwhj.cn

================================================================================
来源：http://qk.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ed.yuexingan06.cn

================================================================================
来源：http://xj.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://zw.chemitech.net.cn

println("Hello")
来源：http://dl.lnxyls.cn

[T02] Kotlin：变量
来源：http://yu.bjjhwx.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://da.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://sh.szxytkj.cn

"值: $b"
来源：http://fo.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://eo.chemitech.net.cn

val n: String? = null;  n?.length
来源：http://oq.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://ue.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nw.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://qd.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sy.colortex.cn

[T07] Kotlin：集合过滤
来源：http://dv.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rb.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://jl.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://kn.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://yj.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://nb.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://tf.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yt.wgjwhj.cn

[T11] Kotlin：协程
来源：http://wo.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mx.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://mt.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://nf.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://xj.colortex.cn

val m = mapOf("a" to 1)
来源：http://nk.huixiangedu.cn

[T14] Kotlin：循环
来源：http://lj.colortex.cn

for (i in 1..10) println(i)
来源：http://pk.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://at.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://hh.jctech888.com.cn

[T16] Swift：Hello World
来源：http://yg.521024.cn

print("Hello")
来源：http://bd.szxytkj.cn

[T17] Swift：变量与常量
来源：http://qa.colortex.cn

var a = 1;  let b = 2
来源：http://vf.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://xs.asd995.cn

"值: \(b)"
来源：http://tx.szsharing.cn

[T19] Swift：可选绑定
来源：http://cu.hahajie.cn

if let n = opt { print(n) }
来源：http://gs.shtwfgs.cn

[T20] Swift：数组操作
来源：http://ry.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yx.szxytkj.cn

[T21] Swift：遍历
来源：http://yg.bookmarksfly.cn

for x in a { print(x) }
来源：http://kv.hnjuh.cn

[T22] Swift：字典
来源：http://gd.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wt.shxzukj.cn

[T23] Swift：函数
来源：http://fs.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rl.haigaiapp.cn

[T24] Swift：闭包
来源：http://lb.asd995.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://us.chemitech.net.cn

[T25] Swift：结构体
来源：http://bx.bjjhwx.cn

struct P { var x: Int }
来源：http://yw.bjjhwx.cn

[T26] Swift：类与重写
来源：http://sp.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://fm.shxzukj.cn

[T27] Swift：错误处理
来源：http://zx.nicolike.cn

do { try f() } catch { print(error) }
来源：http://zk.hahajie.cn

[T28] Swift：枚举
来源：http://nf.yuntaijiaju.cn

enum Color { case red, green }
来源：http://zh.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://dz.shtwfgs.cn

guard let x = opt else { return }
来源：http://lo.shtwfgs.cn

[T30] Swift：协议
来源：http://pu.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://ub.nicolike.cn

[T31] Lua：Hello World
来源：http://io.shxzskj.cn

print("Hello")
来源：http://qa.chemitech.net.cn

[T32] Lua：局部变量
来源：http://dw.lnxyls.cn

local a = 1
来源：http://we.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://cu.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://do.hnjuh.cn

[T34] Lua：遍历表
来源：http://uy.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uo.lnxyls.cn

[T35] Lua：字典表
来源：http://ek.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://dz.hnjuh.cn

[T36] Lua：函数
来源：http://ay.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://td.newstarts.cn

[T37] Lua：字符串拼接
来源：http://sr.shxzskj.cn

"a" .. "b"
来源：http://wi.chemitech.net.cn

[T38] Lua：条件
来源：http://ez.muxihuayi.cn

if x > 0 then print("正") end
来源：http://yx.hahajie.cn

[T39] Lua：模式匹配
来源：http://bh.bookmarksfly.cn

string.find(s, "%d+")
来源：http://id.521024.cn

[T40] Lua：元表
来源：http://gz.newstarts.cn

setmetatable({}, { __index = base })
来源：http://xp.huanxung.cn

[T41] Perl：Hello World
来源：http://ge.nszjky.cn

print "Hello\n";
来源：http://jj.hnjuh.cn

[T42] Perl：变量类型
来源：http://qa.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nz.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://ub.hnjuh.cn

"值: $a"
来源：http://md.nicolike.cn

[T44] Perl：条件
来源：http://hg.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://bf.nicolike.cn

[T45] Perl：数组遍历
来源：http://wf.asd995.cn

for my $x (@arr) { print $x; }
来源：http://ti.newstarts.cn

[T46] Perl：哈希操作
来源：http://tb.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bk.gzmigu.cn

[T47] Perl：正则捕获
来源：http://nk.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qo.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://un.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://hw.bookmarksfly.cn

[T49] Perl：函数
来源：http://oy.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zh.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://ib.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cd.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ff.yuexingan06.cn

[T51] Scala：Hello World
来源：http://wo.hnjuh.cn

println("Hello")
来源：http://pz.yuntaijiaju.cn

[T52] Scala：变量
来源：http://ox.newstarts.cn

val a = 1;  var b = 2
来源：http://pn.shxzukj.cn

[T53] Scala：字符串插值
来源：http://qx.jctech888.com.cn

s"值: $b"
来源：http://yn.521024.cn

[T54] Scala：集合映射
来源：http://ko.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://tb.asd995.cn

[T55] Scala：集合过滤
来源：http://qq.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ov.bookmarksfly.cn

[T56] Scala：样例类
来源：http://mf.szxytkj.cn

case class User(name: String, age: Int)
来源：http://cv.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://xb.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jb.shtwfgs.cn

[T58] Scala：函数定义
来源：http://dm.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://to.chemitech.net.cn

[T59] Scala：循环
来源：http://bx.nszjky.cn

for (i <- 1 to 10) println(i)
来源：http://hf.chemitech.net.cn

[T60] Scala：折叠
来源：http://vc.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rn.yuexingan06.cn

================================================================================
来源：http://vt.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xr.yuexingan06.cn

================================================================================
来源：http://yh.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://fx.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bi.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://hq.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nk.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://ba.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xr.szxytkj.cn

[U04] Py：变量调试打印
来源：http://ch.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qe.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://lc.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://zb.colortex.cn

[U06] Py：合并两个字典
来源：http://jx.shxzskj.cn

{**a, **b}
来源：http://xz.yuexingan06.cn

[U07] Py：反转字典键值
来源：http://yu.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://yk.panjiajie.cn

[U08] Py：展平二维列表
来源：http://dl.nicolike.cn

[y for x in nested for y in x]
来源：http://vq.jianghongdianzi.cn

[U09] Py：字典取最大值的键
来源：http://rm.yuntaijiaju.cn

max(d, key=d.get)
来源：http://qa.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ql.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://an.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://po.hnjuh.cn

(x * 2 for x in arr)
来源：http://ii.nicolike.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mk.bookmarksfly.cn

Counter(arr).most_common(3)
来源：http://ii.huanxung.cn

[U13] Py：固定长度队列
来源：http://sp.shxzukj.cn

deque(maxlen=10)
来源：http://mo.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://qc.bjjhwx.cn

defaultdict(list)
来源：http://il.szxytkj.cn

[U15] Py：高精度计时
来源：http://gs.yuexingan06.cn

t = time.perf_counter()
来源：http://mc.521024.cn

[U16] Py：命令行参数解析
来源：http://al.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jw.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://xk.bjjhwx.cn

logging.basicConfig(level=logging.INFO)
来源：http://am.yuexingan06.cn

[U18] Py：预编译正则
来源：http://bf.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://ao.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://ag.haigaiapp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ts.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://mh.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://dd.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://wa.bookmarksfly.cn

@contextlib.contextmanager
来源：http://mu.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://zv.huixinmuqiang.cn

list(zip(*m))
来源：http://hw.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://qb.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://my.bookmarksfly.cn

[U24] Py：路径操作
来源：http://sr.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://um.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://hj.yuexingan06.cn

csv.DictReader(f)
来源：http://nj.521024.cn

[U26] Py：并发下载
来源：http://sk.chemitech.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yj.9csxet.cn

[U27] Py：异步 HTTP
来源：http://tb.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://jv.hahajie.cn

[U28] Py：类型别名
来源：http://ra.nicolike.cn

UserId = int
来源：http://em.nszjky.cn

[U29] Py：属性校验
来源：http://hj.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://cq.haigaiapp.cn

[U30] Py：数据类
来源：http://er.shtwfgs.cn

@dataclass(slots=True)
来源：http://rc.yuexingan06.cn

[U31] Py：单测
来源：http://gf.hahajie.cn

python -m pytest -q
来源：http://nf.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://uv.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://ds.wgjwhj.cn

[U33] Py：打包发布
来源：http://ax.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://te.shtwfgs.cn

[U34] Py：判断编码
来源：http://hw.yuntaijiaju.cn

chardet.detect(raw)
来源：http://eb.shxzskj.cn

[U35] Py：发送邮件
来源：http://yy.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ql.shxzskj.cn

[U36] Py：定时任务
来源：http://cc.lnxyls.cn

schedule.every(10).minutes.do(job)
来源：http://wh.newstarts.cn

[U37] Py：读写 Excel
来源：http://ru.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mv.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://xo.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://kl.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://fm.bookmarksfly.cn

sys.stdout.isatty()
来源：http://fw.9csxet.cn

[U40] Py：打印到标准错误
来源：http://zf.huanxung.cn

print("err", file=sys.stderr)
来源：http://vv.shtwfgs.cn

[U41] PHP：初始化 Composer 项目
来源：http://bt.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fi.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://dr.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wi.szsharing.cn


<!-- 参考信息 -->