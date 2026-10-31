代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://pb.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://os.asd995.cn

fclose(f);
来源：http://cz.yuntaijiaju.cn

[S12] C：写文件
来源：http://ya.szsharing.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kr.shxzukj.cn

[S13] C：宏定义
来源：http://ba.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://az.gzmigu.cn

[S14] C：枚举
来源：http://ib.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://lf.hahajie.cn

[S15] C：类型转换
来源：http://ge.yuexingan06.cn

(double) a / b
来源：http://vd.yuexingan06.cn

[S16] C：位操作置位
来源：http://ub.asd995.cn

x |= (1 << 3);
来源：http://af.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://yt.huanxung.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qf.nicolike.cn

[S18] C：命令行参数
来源：http://wd.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://nb.haigaiapp.cn

[S19] C：快速排序
来源：http://fi.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rv.huixiangedu.cn

[S20] C：二分查找
来源：http://wb.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ki.haigaiapp.cn

[S21] C：字符类别判断
来源：http://ab.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hj.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://dj.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cp.shxzskj.cn

[S23] C：随机数
来源：http://rq.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ig.shtwfgs.cn

[S24] C：获取本地时间
来源：http://cx.nszjky.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eh.shxzskj.cn

[S25] C：内存拷贝
来源：http://as.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://jk.jianghongdianzi.cn

[S26] C：内存清零
来源：http://fz.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://oe.jianghongdianzi.cn

[S27] C：定义常量
来源：http://ou.yuexingan06.cn

const double PI = 3.14159;
来源：http://mo.yuexingan06.cn

[S28] C：静态变量
来源：http://xa.huixinmuqiang.cn

static int counter = 0;
来源：http://sj.huixiangedu.cn

[S29] C：变参函数
来源：http://cn.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://py.newstarts.cn

[S30] C：头文件保护
来源：http://xw.szxytkj.cn

#ifndef X_H
来源：http://ia.9csxet.cn

#define X_H
来源：http://iq.lnxyls.cn

#endif
来源：http://nw.huanxung.cn

[S31] C++：Hello World
来源：http://us.bookmarksfly.cn

#include <iostream>
来源：http://nk.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://uk.huixinmuqiang.cn

[S32] C++：字符串
来源：http://ef.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://wo.szsharing.cn

[S33] C++：vector 增删
来源：http://sy.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zy.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://ir.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://cz.huixinmuqiang.cn

[S35] C++：map
来源：http://kw.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jg.colortex.cn

[S36] C++：unordered_map
来源：http://vz.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wv.szxytkj.cn

[S37] C++：set
来源：http://aw.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rs.gzmigu.cn

[S38] C++：排序
来源：http://kk.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://mm.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://zl.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fg.muxihuayi.cn

[S40] C++：查找元素
来源：http://ow.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gr.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://zq.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xa.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://qk.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://xe.shxzskj.cn

[S43] C++：智能指针
来源：http://kp.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://cf.muxihuayi.cn

[S44] C++：引用传参
来源：http://jf.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://qp.hnjuh.cn

[S45] C++：lambda
来源：http://wq.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xk.asd995.cn

[S46] C++：函数模板
来源：http://zl.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pw.521024.cn

[S47] C++：结构化绑定遍历
来源：http://yr.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dv.521024.cn

[S48] C++：逐行读文件
来源：http://bf.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hq.asd995.cn

while (std::getline(in, line)) { }
来源：http://pz.yuntaijiaju.cn

[S49] C++：写文件
来源：http://nd.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pc.szsharing.cn

[S50] C++：格式化数字
来源：http://yi.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lk.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://pm.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://hi.colortex.cn

[S52] C++：const 与 noexcept
来源：http://iw.521024.cn

int size() const noexcept { return n_; }
来源：http://ce.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://cz.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://zw.jctech888.com.cn

[S54] C++：异常处理
来源：http://nt.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://br.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://zm.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wi.yuexingan06.cn

[S56] C++：optional
来源：http://kg.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ak.asd995.cn

[S57] C++：编译期常量
来源：http://zv.newstarts.cn

constexpr int N = 10;
来源：http://vg.panjiajie.cn

[S58] C++：命名空间
来源：http://gj.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://xg.521024.cn

[S59] C++：静态断言
来源：http://te.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fx.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://qv.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lh.huixiangedu.cn

================================================================================
来源：http://bf.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ae.nszjky.cn

================================================================================
来源：http://yx.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://ho.nicolike.cn

println("Hello")
来源：http://bp.huixiangedu.cn

[T02] Kotlin：变量
来源：http://kx.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cn.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://rz.panjiajie.cn

"值: $b"
来源：http://vf.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://gm.hahajie.cn

val n: String? = null;  n?.length
来源：http://ta.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://sb.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uq.jctech888.com.cn

[T06] Kotlin：集合映射
来源：http://yb.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ps.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ch.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://us.colortex.cn

[T08] Kotlin：数据类
来源：http://ni.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://ov.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://qx.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://rc.nszjky.cn

[T10] Kotlin：默认参数
来源：http://ye.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pd.yuexingan06.cn

[T11] Kotlin：协程
来源：http://zk.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ur.nszjky.cn

[T12] Kotlin：解构声明
来源：http://rb.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://pz.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://zb.521024.cn

val m = mapOf("a" to 1)
来源：http://tn.newstarts.cn

[T14] Kotlin：循环
来源：http://gr.newstarts.cn

for (i in 1..10) println(i)
来源：http://qg.huixiangedu.cn

[T15] Kotlin：接口
来源：http://wo.colortex.cn

interface Shape { fun area(): Double }
来源：http://lu.muxihuayi.cn

[T16] Swift：Hello World
来源：http://ba.jianghongdianzi.cn

print("Hello")
来源：http://nw.colortex.cn

[T17] Swift：变量与常量
来源：http://mm.shtwfgs.cn

var a = 1;  let b = 2
来源：http://ff.huixinmuqiang.cn

[T18] Swift：字符串插值
来源：http://gy.wgjwhj.cn

"值: \(b)"
来源：http://zr.gzmigu.cn

[T19] Swift：可选绑定
来源：http://ql.9csxet.cn

if let n = opt { print(n) }
来源：http://yj.hahajie.cn

[T20] Swift：数组操作
来源：http://nm.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kp.521024.cn

[T21] Swift：遍历
来源：http://mq.shxzukj.cn

for x in a { print(x) }
来源：http://xw.9csxet.cn

[T22] Swift：字典
来源：http://ko.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://it.hahajie.cn

[T23] Swift：函数
来源：http://kr.hahajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://as.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://js.yuexingan06.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ps.shxzukj.cn

[T25] Swift：结构体
来源：http://qf.haigaiapp.cn

struct P { var x: Int }
来源：http://xi.haigaiapp.cn

[T26] Swift：类与重写
来源：http://gs.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://he.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://sw.nszjky.cn

do { try f() } catch { print(error) }
来源：http://tt.colortex.cn

[T28] Swift：枚举
来源：http://fr.colortex.cn

enum Color { case red, green }
来源：http://jn.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://ho.bookmarksfly.cn

guard let x = opt else { return }
来源：http://dn.yuntaijiaju.cn

[T30] Swift：协议
来源：http://tz.colortex.cn

protocol Shape { func area() -> Double }
来源：http://xc.nicolike.cn

[T31] Lua：Hello World
来源：http://fm.shtwfgs.cn

print("Hello")
来源：http://xp.521024.cn

[T32] Lua：局部变量
来源：http://kc.chemitech.net.cn

local a = 1
来源：http://ew.shxzukj.cn

[T33] Lua：表（数组）
来源：http://gl.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wu.haigaiapp.cn

[T34] Lua：遍历表
来源：http://ev.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nw.wgjwhj.cn

[T35] Lua：字典表
来源：http://zo.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://wq.lnxyls.cn

[T36] Lua：函数
来源：http://cc.9csxet.cn

function add(a, b) return a + b end
来源：http://te.newstarts.cn

[T37] Lua：字符串拼接
来源：http://kc.yuexingan06.cn

"a" .. "b"
来源：http://tf.yuntaijiaju.cn

[T38] Lua：条件
来源：http://gp.lnxyls.cn

if x > 0 then print("正") end
来源：http://pv.colortex.cn

[T39] Lua：模式匹配
来源：http://rv.huanxung.cn

string.find(s, "%d+")
来源：http://sl.newstarts.cn

[T40] Lua：元表
来源：http://qn.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://kl.nszjky.cn

[T41] Perl：Hello World
来源：http://ys.shxzukj.cn

print "Hello\n";
来源：http://ky.szxytkj.cn

[T42] Perl：变量类型
来源：http://oc.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zn.hahajie.cn

[T43] Perl：字符串插值
来源：http://tt.jctech888.com.cn

"值: $a"
来源：http://gh.haigaiapp.cn

[T44] Perl：条件
来源：http://ju.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://of.szsharing.cn

[T45] Perl：数组遍历
来源：http://wh.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://zq.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://rg.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dr.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://vc.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://et.521024.cn

[T48] Perl：正则替换
来源：http://qs.szsharing.cn

$s =~ s/old/new/g;
来源：http://jd.haigaiapp.cn

[T49] Perl：函数
来源：http://af.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fg.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://iz.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tv.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://ne.wgjwhj.cn

[T51] Scala：Hello World
来源：http://mc.wgjwhj.cn

println("Hello")
来源：http://in.jianghongdianzi.cn

[T52] Scala：变量
来源：http://iv.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://bf.wgjwhj.cn

[T53] Scala：字符串插值
来源：http://pt.9csxet.cn

s"值: $b"
来源：http://gp.newstarts.cn

[T54] Scala：集合映射
来源：http://nm.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://ye.521024.cn

[T55] Scala：集合过滤
来源：http://uq.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yi.muxihuayi.cn

[T56] Scala：样例类
来源：http://bw.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://vo.hnjuh.cn

[T57] Scala：模式匹配
来源：http://rl.haigaiapp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eo.huanxung.cn

[T58] Scala：函数定义
来源：http://gp.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ax.521024.cn

[T59] Scala：循环
来源：http://vu.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://zs.nszjky.cn

[T60] Scala：折叠
来源：http://zc.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kg.chemitech.net.cn

================================================================================
来源：http://zz.haigaiapp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tj.asd995.cn

================================================================================
来源：http://uf.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://sk.bjjhwx.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mv.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://ab.panjiajie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qi.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://vp.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ca.shxzukj.cn

[U04] Py：变量调试打印
来源：http://jc.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cx.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://js.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://mq.szxytkj.cn

[U06] Py：合并两个字典
来源：http://gr.huixiangedu.cn

{**a, **b}
来源：http://jc.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://xo.9csxet.cn

{v: k for k, v in d.items()}
来源：http://ae.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://ka.lnxyls.cn

[y for x in nested for y in x]
来源：http://zu.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://hz.colortex.cn

max(d, key=d.get)
来源：http://he.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://ee.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hi.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://wf.asd995.cn

(x * 2 for x in arr)
来源：http://ab.521024.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mw.gzmigu.cn

Counter(arr).most_common(3)
来源：http://jh.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://ng.521024.cn

deque(maxlen=10)
来源：http://va.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://dr.hahajie.cn

defaultdict(list)
来源：http://en.muxihuayi.cn

[U15] Py：高精度计时
来源：http://zj.yuexingan06.cn

t = time.perf_counter()
来源：http://tg.haigaiapp.cn

[U16] Py：命令行参数解析
来源：http://fa.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ak.nicolike.cn

[U17] Py：初始化日志
来源：http://tc.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://kj.shxzukj.cn

[U18] Py：预编译正则
来源：http://rc.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://oy.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://cg.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hv.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://it.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://pz.newstarts.cn

[U21] Py：自定义上下文管理器
来源：http://ep.yuntaijiaju.cn

@contextlib.contextmanager
来源：http://yv.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://zm.wgjwhj.cn

list(zip(*m))
来源：http://oe.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://eb.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yo.nszjky.cn

[U24] Py：路径操作
来源：http://ah.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vv.bjjhwx.cn

[U25] Py：CSV 按字典读
来源：http://kc.asd995.cn

csv.DictReader(f)
来源：http://ou.haigaiapp.cn

[U26] Py：并发下载
来源：http://sy.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sc.szsharing.cn

[U27] Py：异步 HTTP
来源：http://bm.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://cd.lnxyls.cn

[U28] Py：类型别名
来源：http://mj.hahajie.cn

UserId = int
来源：http://da.muxihuayi.cn

[U29] Py：属性校验
来源：http://zb.hnjuh.cn

@property 与 @x.setter 配合
来源：http://nk.szsharing.cn

[U30] Py：数据类
来源：http://lf.bookmarksfly.cn

@dataclass(slots=True)
来源：http://qs.hahajie.cn

[U31] Py：单测
来源：http://rg.9csxet.cn

python -m pytest -q
来源：http://km.hnjuh.cn

[U32] Py：代码格式化
来源：http://nu.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://et.hahajie.cn

[U33] Py：打包发布
来源：http://vn.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://cl.gzmigu.cn

[U34] Py：判断编码
来源：http://zv.hahajie.cn

chardet.detect(raw)
来源：http://fw.huixinmuqiang.cn


<!-- 参考信息 -->