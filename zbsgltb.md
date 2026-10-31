代发 wailian999

int main(int argc, char **argv)
来源：http://zz.newstarts.cn

[S19] C：快速排序
来源：http://to.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://in.huixiangedu.cn

[S20] C：二分查找
来源：http://hv.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cr.muxihuayi.cn

[S21] C：字符类别判断
来源：http://ic.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mz.huanxung.cn

[S22] C：字符串转数字
来源：http://tm.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ui.521024.cn

[S23] C：随机数
来源：http://zn.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hv.9csxet.cn

[S24] C：获取本地时间
来源：http://ik.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vq.bjjhwx.cn

[S25] C：内存拷贝
来源：http://qw.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://cg.newstarts.cn

[S26] C：内存清零
来源：http://sp.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://xo.521024.cn

[S27] C：定义常量
来源：http://gk.shxzskj.cn

const double PI = 3.14159;
来源：http://dp.jctech888.com.cn

[S28] C：静态变量
来源：http://ho.yuexingan06.cn

static int counter = 0;
来源：http://wm.yuntaijiaju.cn

[S29] C：变参函数
来源：http://uh.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rm.newstarts.cn

[S30] C：头文件保护
来源：http://ka.huanxung.cn

#ifndef X_H
来源：http://we.yuntaijiaju.cn

#define X_H
来源：http://fv.panjiajie.cn

#endif
来源：http://hv.colortex.cn

[S31] C++：Hello World
来源：http://wc.lnxyls.cn

#include <iostream>
来源：http://id.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://er.huanxung.cn

[S32] C++：字符串
来源：http://lj.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://yu.shxzukj.cn

[S33] C++：vector 增删
来源：http://qw.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vy.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://jy.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://zi.yuexingan06.cn

[S35] C++：map
来源：http://wi.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://df.hahajie.cn

[S36] C++：unordered_map
来源：http://kx.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zp.chemitech.net.cn

[S37] C++：set
来源：http://kc.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ot.huixiangedu.cn

[S38] C++：排序
来源：http://pd.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://ji.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://dy.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ux.gzmigu.cn

[S40] C++：查找元素
来源：http://ak.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zc.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://es.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gf.huanxung.cn

[S42] C++：继承与虚函数
来源：http://km.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://rf.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://jf.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://al.shxzskj.cn

[S44] C++：引用传参
来源：http://tm.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://ss.shxzukj.cn

[S45] C++：lambda
来源：http://mi.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dm.gzmigu.cn

[S46] C++：函数模板
来源：http://tg.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cv.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://pe.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ct.huanxung.cn

[S48] C++：逐行读文件
来源：http://vm.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sj.521024.cn

while (std::getline(in, line)) { }
来源：http://qm.haigaiapp.cn

[S49] C++：写文件
来源：http://pv.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sl.hnjuh.cn

[S50] C++：格式化数字
来源：http://az.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ht.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://mv.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://tt.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://je.nszjky.cn

int size() const noexcept { return n_; }
来源：http://ej.shxzukj.cn

[S53] C++：移动语义
来源：http://bi.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://kb.yuexingan06.cn

[S54] C++：异常处理
来源：http://om.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rj.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://ih.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://py.panjiajie.cn

[S56] C++：optional
来源：http://wh.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bb.panjiajie.cn

[S57] C++：编译期常量
来源：http://wg.asd995.cn

constexpr int N = 10;
来源：http://tv.lnxyls.cn

[S58] C++：命名空间
来源：http://of.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://yl.szxytkj.cn

[S59] C++：静态断言
来源：http://lr.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jf.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://hh.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kv.yuntaijiaju.cn

================================================================================
来源：http://wj.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rr.nicolike.cn

================================================================================
来源：http://hh.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://ph.jianghongdianzi.cn

println("Hello")
来源：http://cq.9csxet.cn

[T02] Kotlin：变量
来源：http://lw.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wk.521024.cn

[T03] Kotlin：字符串模板
来源：http://bd.haigaiapp.cn

"值: $b"
来源：http://aq.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://ul.colortex.cn

val n: String? = null;  n?.length
来源：http://rb.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://ro.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zp.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://xq.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://el.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://dc.asd995.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xo.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://ow.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://mi.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://lf.hnjuh.cn

fun String.exclaim() = this + "!"
来源：http://dx.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://mb.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pz.huixiangedu.cn

[T11] Kotlin：协程
来源：http://ae.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wi.asd995.cn

[T12] Kotlin：解构声明
来源：http://jv.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://io.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://mv.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://lg.huixiangedu.cn

[T14] Kotlin：循环
来源：http://nz.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://zl.nicolike.cn

[T15] Kotlin：接口
来源：http://up.asd995.cn

interface Shape { fun area(): Double }
来源：http://lr.jctech888.com.cn

[T16] Swift：Hello World
来源：http://vn.gzmigu.cn

print("Hello")
来源：http://zu.nicolike.cn

[T17] Swift：变量与常量
来源：http://zi.lnxyls.cn

var a = 1;  let b = 2
来源：http://jc.szxytkj.cn

[T18] Swift：字符串插值
来源：http://ab.nicolike.cn

"值: \(b)"
来源：http://in.nicolike.cn

[T19] Swift：可选绑定
来源：http://dq.hnjuh.cn

if let n = opt { print(n) }
来源：http://da.panjiajie.cn

[T20] Swift：数组操作
来源：http://lg.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qz.bjjhwx.cn

[T21] Swift：遍历
来源：http://yj.haigaiapp.cn

for x in a { print(x) }
来源：http://op.chemitech.net.cn

[T22] Swift：字典
来源：http://le.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mg.panjiajie.cn

[T23] Swift：函数
来源：http://dq.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jv.bookmarksfly.cn

[T24] Swift：闭包
来源：http://zr.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zx.asd995.cn

[T25] Swift：结构体
来源：http://ti.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ik.shxzukj.cn

[T26] Swift：类与重写
来源：http://lv.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://xe.wgjwhj.cn

[T27] Swift：错误处理
来源：http://sk.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://aa.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://km.lnxyls.cn

enum Color { case red, green }
来源：http://uv.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://uj.shxzskj.cn

guard let x = opt else { return }
来源：http://bt.haigaiapp.cn

[T30] Swift：协议
来源：http://gj.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://ai.shxzukj.cn

[T31] Lua：Hello World
来源：http://al.muxihuayi.cn

print("Hello")
来源：http://cx.nicolike.cn

[T32] Lua：局部变量
来源：http://nw.panjiajie.cn

local a = 1
来源：http://mm.newstarts.cn

[T33] Lua：表（数组）
来源：http://zg.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oz.szxytkj.cn

[T34] Lua：遍历表
来源：http://kn.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zs.asd995.cn

[T35] Lua：字典表
来源：http://bo.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://la.muxihuayi.cn

[T36] Lua：函数
来源：http://ui.521024.cn

function add(a, b) return a + b end
来源：http://dc.szxytkj.cn

[T37] Lua：字符串拼接
来源：http://fv.huixinmuqiang.cn

"a" .. "b"
来源：http://kv.nszjky.cn

[T38] Lua：条件
来源：http://cb.chemitech.net.cn

if x > 0 then print("正") end
来源：http://gd.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://bk.panjiajie.cn

string.find(s, "%d+")
来源：http://in.hahajie.cn

[T40] Lua：元表
来源：http://mk.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://bs.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://oc.yuntaijiaju.cn

print "Hello\n";
来源：http://oy.gzmigu.cn

[T42] Perl：变量类型
来源：http://qg.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nb.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://ql.yuntaijiaju.cn

"值: $a"
来源：http://jc.huixiangedu.cn

[T44] Perl：条件
来源：http://ui.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://qw.521024.cn

[T45] Perl：数组遍历
来源：http://yu.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://hz.nszjky.cn

[T46] Perl：哈希操作
来源：http://nf.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zj.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://kc.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xg.colortex.cn

[T48] Perl：正则替换
来源：http://zl.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://qz.szxytkj.cn

[T49] Perl：函数
来源：http://qz.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ua.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://ba.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ui.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://bm.chemitech.net.cn

[T51] Scala：Hello World
来源：http://rl.521024.cn

println("Hello")
来源：http://ch.wgjwhj.cn

[T52] Scala：变量
来源：http://wa.shxzukj.cn

val a = 1;  var b = 2
来源：http://rq.gzmigu.cn

[T53] Scala：字符串插值
来源：http://bk.asd995.cn

s"值: $b"
来源：http://kd.shtwfgs.cn

[T54] Scala：集合映射
来源：http://kb.newstarts.cn

List(1, 2, 3).map(_ * 2)
来源：http://tu.gzmigu.cn

[T55] Scala：集合过滤
来源：http://ui.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vy.shtwfgs.cn

[T56] Scala：样例类
来源：http://tm.szxytkj.cn

case class User(name: String, age: Int)
来源：http://kv.9csxet.cn

[T57] Scala：模式匹配
来源：http://qy.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tc.bjjhwx.cn

[T58] Scala：函数定义
来源：http://cm.yuntaijiaju.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kv.muxihuayi.cn

[T59] Scala：循环
来源：http://hi.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://kf.shxzukj.cn

[T60] Scala：折叠
来源：http://na.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qj.hnjuh.cn

================================================================================
来源：http://nt.nszjky.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xc.newstarts.cn

================================================================================
来源：http://of.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://ip.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://oe.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://lp.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zq.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://yz.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bo.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://ga.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ty.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://ul.panjiajie.cn

list(dict.fromkeys(arr))
来源：http://az.panjiajie.cn

[U06] Py：合并两个字典
来源：http://rw.bookmarksfly.cn

{**a, **b}
来源：http://nm.colortex.cn

[U07] Py：反转字典键值
来源：http://xi.nszjky.cn

{v: k for k, v in d.items()}
来源：http://wj.haigaiapp.cn

[U08] Py：展平二维列表
来源：http://bj.bjjhwx.cn

[y for x in nested for y in x]
来源：http://eb.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://po.jianghongdianzi.cn

max(d, key=d.get)
来源：http://tc.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://xk.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nn.hnjuh.cn

[U11] Py：生成器表达式
来源：http://zp.yuntaijiaju.cn

(x * 2 for x in arr)
来源：http://ms.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oz.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ak.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ts.gzmigu.cn

deque(maxlen=10)
来源：http://dh.bookmarksfly.cn

[U14] Py：分组收集到列表
来源：http://mh.shxzskj.cn

defaultdict(list)
来源：http://zf.gzmigu.cn

[U15] Py：高精度计时
来源：http://kn.haigaiapp.cn

t = time.perf_counter()
来源：http://pr.hahajie.cn

[U16] Py：命令行参数解析
来源：http://dz.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gk.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://my.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://wg.chemitech.net.cn

[U18] Py：预编译正则
来源：http://qb.nicolike.cn

pat = re.compile(r"\d+")
来源：http://zr.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://ch.jianghongdianzi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iy.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://eq.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://fx.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://gs.shxzukj.cn

@contextlib.contextmanager
来源：http://dw.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://lh.szsharing.cn

list(zip(*m))
来源：http://vo.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://zi.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pf.panjiajie.cn

[U24] Py：路径操作
来源：http://sj.shxzukj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uh.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://rp.panjiajie.cn

csv.DictReader(f)
来源：http://vv.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://up.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wr.hnjuh.cn

[U27] Py：异步 HTTP
来源：http://vn.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://co.521024.cn

[U28] Py：类型别名
来源：http://id.wgjwhj.cn

UserId = int
来源：http://qr.szxytkj.cn

[U29] Py：属性校验
来源：http://gy.lnxyls.cn

@property 与 @x.setter 配合
来源：http://zg.lnxyls.cn

[U30] Py：数据类
来源：http://qq.szsharing.cn

@dataclass(slots=True)
来源：http://ru.huixinmuqiang.cn

[U31] Py：单测
来源：http://mk.yuexingan06.cn

python -m pytest -q
来源：http://os.huanxung.cn

[U32] Py：代码格式化
来源：http://nm.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://pi.gzmigu.cn

[U33] Py：打包发布
来源：http://wv.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://lp.521024.cn

[U34] Py：判断编码
来源：http://ss.hnjuh.cn

chardet.detect(raw)
来源：http://ub.szsharing.cn

[U35] Py：发送邮件
来源：http://li.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jh.jctech888.com.cn

[U36] Py：定时任务
来源：http://ri.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://kg.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://ds.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vt.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://lj.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://dr.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://ba.hahajie.cn

sys.stdout.isatty()
来源：http://pm.gzmigu.cn

[U40] Py：打印到标准错误
来源：http://lb.huixiangedu.cn

print("err", file=sys.stderr)
来源：http://fo.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://rc.shxzskj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nk.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://oi.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bp.hahajie.cn


<!-- 参考信息 -->