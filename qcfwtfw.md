代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jm.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://ev.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lt.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://lf.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uv.9csxet.cn

[S10] C：指针与解引用
来源：http://pr.asd995.cn

int *p = &a;  *p = 5;
来源：http://go.szsharing.cn

[S11] C：逐行读文件
来源：http://od.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://fy.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yy.bjjhwx.cn

fclose(f);
来源：http://yy.hnjuh.cn

[S12] C：写文件
来源：http://sy.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kd.colortex.cn

[S13] C：宏定义
来源：http://tk.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zo.yuexingan06.cn

[S14] C：枚举
来源：http://dg.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://lr.gzmigu.cn

[S15] C：类型转换
来源：http://he.bjjhwx.cn

(double) a / b
来源：http://aq.szxytkj.cn

[S16] C：位操作置位
来源：http://hj.shxzskj.cn

x |= (1 << 3);
来源：http://re.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://hv.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://el.panjiajie.cn

[S18] C：命令行参数
来源：http://xy.gzmigu.cn

int main(int argc, char **argv)
来源：http://ql.wgjwhj.cn

[S19] C：快速排序
来源：http://yq.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cz.shtwfgs.cn

[S20] C：二分查找
来源：http://ry.huanxung.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kx.szsharing.cn

[S21] C：字符类别判断
来源：http://cm.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lj.jctech888.com.cn

[S22] C：字符串转数字
来源：http://li.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zy.szsharing.cn

[S23] C：随机数
来源：http://ji.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dr.muxihuayi.cn

[S24] C：获取本地时间
来源：http://cu.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ep.szxytkj.cn

[S25] C：内存拷贝
来源：http://sa.newstarts.cn

memcpy(dst, src, n);
来源：http://le.hnjuh.cn

[S26] C：内存清零
来源：http://sa.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://nc.jctech888.com.cn

[S27] C：定义常量
来源：http://by.shxzskj.cn

const double PI = 3.14159;
来源：http://ev.nicolike.cn

[S28] C：静态变量
来源：http://ce.huanxung.cn

static int counter = 0;
来源：http://zi.bjjhwx.cn

[S29] C：变参函数
来源：http://ri.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nj.newstarts.cn

[S30] C：头文件保护
来源：http://pv.szxytkj.cn

#ifndef X_H
来源：http://dy.asd995.cn

#define X_H
来源：http://ty.colortex.cn

#endif
来源：http://tt.muxihuayi.cn

[S31] C++：Hello World
来源：http://mu.haigaiapp.cn

#include <iostream>
来源：http://ul.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://qp.gzmigu.cn

[S32] C++：字符串
来源：http://qc.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://ej.panjiajie.cn

[S33] C++：vector 增删
来源：http://sn.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cg.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://zo.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://qs.szsharing.cn

[S35] C++：map
来源：http://uk.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bs.haigaiapp.cn

[S36] C++：unordered_map
来源：http://wi.9csxet.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cl.hahajie.cn

[S37] C++：set
来源：http://av.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pv.hahajie.cn

[S38] C++：排序
来源：http://kt.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://nd.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://vs.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://th.hahajie.cn

[S40] C++：查找元素
来源：http://rb.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gh.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://wx.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kq.hahajie.cn

[S42] C++：继承与虚函数
来源：http://ql.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://ir.9csxet.cn

[S43] C++：智能指针
来源：http://do.szxytkj.cn

auto p = std::make_unique<int>(5);
来源：http://ny.521024.cn

[S44] C++：引用传参
来源：http://je.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://yl.newstarts.cn

[S45] C++：lambda
来源：http://jf.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nx.lnxyls.cn

[S46] C++：函数模板
来源：http://gt.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qi.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://ay.colortex.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lt.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://gc.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yj.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://mk.newstarts.cn

[S49] C++：写文件
来源：http://sq.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uh.huixiangedu.cn

[S50] C++：格式化数字
来源：http://fs.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yo.nicolike.cn

[S51] C++：显式类型转换
来源：http://do.hnjuh.cn

static_cast<double>(a) / b
来源：http://ec.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://ot.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://fr.haigaiapp.cn

[S53] C++：移动语义
来源：http://mz.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://mv.szxytkj.cn

[S54] C++：异常处理
来源：http://gm.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://em.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://vc.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vz.haigaiapp.cn

[S56] C++：optional
来源：http://ip.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qy.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://ts.panjiajie.cn

constexpr int N = 10;
来源：http://in.hahajie.cn

[S58] C++：命名空间
来源：http://zk.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://lr.nicolike.cn

[S59] C++：静态断言
来源：http://ho.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iv.asd995.cn

[S60] C++：遍历并删除元素
来源：http://kp.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jd.haigaiapp.cn

================================================================================
来源：http://bd.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sz.shtwfgs.cn

================================================================================
来源：http://tj.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://yz.hnjuh.cn

println("Hello")
来源：http://rd.521024.cn

[T02] Kotlin：变量
来源：http://gx.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ll.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://uf.asd995.cn

"值: $b"
来源：http://yq.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://lg.szxytkj.cn

val n: String? = null;  n?.length
来源：http://gu.asd995.cn

[T05] Kotlin：when 表达式
来源：http://zg.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jw.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://io.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yb.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://uh.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vn.gzmigu.cn

[T08] Kotlin：数据类
来源：http://rg.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://sc.521024.cn

[T09] Kotlin：扩展函数
来源：http://zc.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://jj.hahajie.cn

[T10] Kotlin：默认参数
来源：http://om.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iq.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://wm.bookmarksfly.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yo.nicolike.cn

[T12] Kotlin：解构声明
来源：http://bo.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://uo.521024.cn

[T13] Kotlin：只读 Map
来源：http://qe.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://dm.shtwfgs.cn

[T14] Kotlin：循环
来源：http://dz.szxytkj.cn

for (i in 1..10) println(i)
来源：http://cn.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://fd.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://ao.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://ng.9csxet.cn

print("Hello")
来源：http://ea.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://yl.9csxet.cn

var a = 1;  let b = 2
来源：http://rd.szsharing.cn

[T18] Swift：字符串插值
来源：http://hs.shtwfgs.cn

"值: \(b)"
来源：http://rr.huanxung.cn

[T19] Swift：可选绑定
来源：http://sh.newstarts.cn

if let n = opt { print(n) }
来源：http://iz.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://pk.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hm.521024.cn

[T21] Swift：遍历
来源：http://eo.shxzukj.cn

for x in a { print(x) }
来源：http://lo.huixiangedu.cn

[T22] Swift：字典
来源：http://jw.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ow.hahajie.cn

[T23] Swift：函数
来源：http://in.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ca.szxytkj.cn

[T24] Swift：闭包
来源：http://li.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tf.nicolike.cn

[T25] Swift：结构体
来源：http://tv.hnjuh.cn

struct P { var x: Int }
来源：http://dg.huanxung.cn

[T26] Swift：类与重写
来源：http://gp.hahajie.cn

class A: Base { override func f() {} }
来源：http://ty.shxzskj.cn

[T27] Swift：错误处理
来源：http://gc.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://jo.huanxung.cn

[T28] Swift：枚举
来源：http://kw.hnjuh.cn

enum Color { case red, green }
来源：http://ke.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://lo.szsharing.cn

guard let x = opt else { return }
来源：http://ma.yuexingan06.cn

[T30] Swift：协议
来源：http://ai.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://ur.wgjwhj.cn

[T31] Lua：Hello World
来源：http://tc.yuntaijiaju.cn

print("Hello")
来源：http://cc.asd995.cn

[T32] Lua：局部变量
来源：http://iu.haigaiapp.cn

local a = 1
来源：http://zs.szxytkj.cn

[T33] Lua：表（数组）
来源：http://vr.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cd.newstarts.cn

[T34] Lua：遍历表
来源：http://ee.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jw.wgjwhj.cn

[T35] Lua：字典表
来源：http://wy.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://be.colortex.cn

[T36] Lua：函数
来源：http://tm.shxzukj.cn

function add(a, b) return a + b end
来源：http://uu.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://li.nszjky.cn

"a" .. "b"
来源：http://zr.wgjwhj.cn

[T38] Lua：条件
来源：http://tr.szxytkj.cn

if x > 0 then print("正") end
来源：http://ud.nicolike.cn

[T39] Lua：模式匹配
来源：http://kt.shxzukj.cn

string.find(s, "%d+")
来源：http://bt.panjiajie.cn

[T40] Lua：元表
来源：http://vd.shxzskj.cn

setmetatable({}, { __index = base })
来源：http://xa.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://zg.muxihuayi.cn

print "Hello\n";
来源：http://wp.shxzskj.cn

[T42] Perl：变量类型
来源：http://uq.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vh.9csxet.cn

[T43] Perl：字符串插值
来源：http://bp.asd995.cn

"值: $a"
来源：http://zc.jianghongdianzi.cn

[T44] Perl：条件
来源：http://le.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://bj.szsharing.cn

[T45] Perl：数组遍历
来源：http://bw.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://vg.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://ax.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ve.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://ph.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vj.521024.cn

[T48] Perl：正则替换
来源：http://vj.yuntaijiaju.cn

$s =~ s/old/new/g;
来源：http://mm.lnxyls.cn

[T49] Perl：函数
来源：http://pq.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ge.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://zx.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://to.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://pr.nicolike.cn

[T51] Scala：Hello World
来源：http://eo.shtwfgs.cn

println("Hello")
来源：http://ky.wgjwhj.cn

[T52] Scala：变量
来源：http://pi.gzmigu.cn

val a = 1;  var b = 2
来源：http://sd.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://nt.chemitech.net.cn

s"值: $b"
来源：http://vm.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://yq.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://fw.szsharing.cn

[T55] Scala：集合过滤
来源：http://ox.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fc.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://mr.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://pd.huanxung.cn

[T57] Scala：模式匹配
来源：http://dj.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ur.huanxung.cn

[T58] Scala：函数定义
来源：http://qs.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dr.nszjky.cn

[T59] Scala：循环
来源：http://el.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://zt.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://jk.haigaiapp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fi.jctech888.com.cn

================================================================================
来源：http://xx.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fi.9csxet.cn

================================================================================
来源：http://vt.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://vn.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ev.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://fl.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vo.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://al.jianghongdianzi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xw.asd995.cn

[U04] Py：变量调试打印
来源：http://ah.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vi.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://xi.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://hp.hnjuh.cn

[U06] Py：合并两个字典
来源：http://df.muxihuayi.cn

{**a, **b}
来源：http://hq.colortex.cn

[U07] Py：反转字典键值
来源：http://sc.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://gg.521024.cn

[U08] Py：展平二维列表
来源：http://db.hnjuh.cn

[y for x in nested for y in x]
来源：http://ea.colortex.cn

[U09] Py：字典取最大值的键
来源：http://bl.9csxet.cn

max(d, key=d.get)
来源：http://sn.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://nj.9csxet.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ix.hahajie.cn

[U11] Py：生成器表达式
来源：http://jh.asd995.cn

(x * 2 for x in arr)
来源：http://on.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lk.shxzskj.cn

Counter(arr).most_common(3)
来源：http://qr.szsharing.cn

[U13] Py：固定长度队列
来源：http://lp.9csxet.cn

deque(maxlen=10)
来源：http://mw.huixiangedu.cn

[U14] Py：分组收集到列表
来源：http://lm.jianghongdianzi.cn

defaultdict(list)
来源：http://tx.huixiangedu.cn

[U15] Py：高精度计时
来源：http://oj.shxzukj.cn

t = time.perf_counter()
来源：http://aq.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://qr.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://if.521024.cn

[U17] Py：初始化日志
来源：http://eb.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://zf.hahajie.cn

[U18] Py：预编译正则
来源：http://tt.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://nm.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://df.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://az.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://cg.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://qp.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://mk.hnjuh.cn

@contextlib.contextmanager
来源：http://ry.szxytkj.cn

[U22] Py：矩阵转置
来源：http://mc.yuexingan06.cn

list(zip(*m))
来源：http://ef.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://tv.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xr.gzmigu.cn

[U24] Py：路径操作
来源：http://bd.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://am.huixinmuqiang.cn

[U25] Py：CSV 按字典读
来源：http://px.jianghongdianzi.cn

csv.DictReader(f)
来源：http://wx.huixiangedu.cn

[U26] Py：并发下载
来源：http://sx.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ua.521024.cn

[U27] Py：异步 HTTP
来源：http://jy.panjiajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://rr.muxihuayi.cn

[U28] Py：类型别名
来源：http://vk.bjjhwx.cn

UserId = int
来源：http://xb.asd995.cn

[U29] Py：属性校验
来源：http://lm.shxzukj.cn

@property 与 @x.setter 配合
来源：http://ha.asd995.cn

[U30] Py：数据类
来源：http://mx.panjiajie.cn

@dataclass(slots=True)
来源：http://yi.huanxung.cn


<!-- 参考信息 -->