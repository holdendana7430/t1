代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ey.szsharing.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ur.521024.cn

fclose(f);
来源：http://xh.bjjhwx.cn

[S12] C：写文件
来源：http://ka.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qn.chemitech.net.cn

[S13] C：宏定义
来源：http://lq.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://df.gzmigu.cn

[S14] C：枚举
来源：http://is.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://rf.szxytkj.cn

[S15] C：类型转换
来源：http://bm.bookmarksfly.cn

(double) a / b
来源：http://pk.gzmigu.cn

[S16] C：位操作置位
来源：http://ao.hnjuh.cn

x |= (1 << 3);
来源：http://mr.huanxung.cn

[S17] C：安全拼接字符串
来源：http://pb.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ny.hnjuh.cn

[S18] C：命令行参数
来源：http://hu.shtwfgs.cn

int main(int argc, char **argv)
来源：http://pj.colortex.cn

[S19] C：快速排序
来源：http://eq.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tt.chemitech.net.cn

[S20] C：二分查找
来源：http://ms.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ld.gzmigu.cn

[S21] C：字符类别判断
来源：http://da.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fq.colortex.cn

[S22] C：字符串转数字
来源：http://qo.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pd.9csxet.cn

[S23] C：随机数
来源：http://hx.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hn.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://ct.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xc.hnjuh.cn

[S25] C：内存拷贝
来源：http://ak.hahajie.cn

memcpy(dst, src, n);
来源：http://ly.shtwfgs.cn

[S26] C：内存清零
来源：http://ms.hahajie.cn

memset(a, 0, sizeof a);
来源：http://wq.gzmigu.cn

[S27] C：定义常量
来源：http://tu.shxzskj.cn

const double PI = 3.14159;
来源：http://vb.9csxet.cn

[S28] C：静态变量
来源：http://nr.chemitech.net.cn

static int counter = 0;
来源：http://sp.haigaiapp.cn

[S29] C：变参函数
来源：http://mj.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kz.521024.cn

[S30] C：头文件保护
来源：http://yf.lnxyls.cn

#ifndef X_H
来源：http://hx.newstarts.cn

#define X_H
来源：http://ym.huixinmuqiang.cn

#endif
来源：http://ub.muxihuayi.cn

[S31] C++：Hello World
来源：http://ch.yuexingan06.cn

#include <iostream>
来源：http://gc.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://fg.szxytkj.cn

[S32] C++：字符串
来源：http://ld.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://rv.shtwfgs.cn

[S33] C++：vector 增删
来源：http://am.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xz.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://ca.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://dl.huixinmuqiang.cn

[S35] C++：map
来源：http://dj.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yb.shtwfgs.cn

[S36] C++：unordered_map
来源：http://yf.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ie.jianghongdianzi.cn

[S37] C++：set
来源：http://co.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zm.nicolike.cn

[S38] C++：排序
来源：http://lv.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://ns.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://bs.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gm.shxzskj.cn

[S40] C++：查找元素
来源：http://cj.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nz.huanxung.cn

[S41] C++：类与构造函数
来源：http://qn.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bf.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://tp.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://fa.yuexingan06.cn

[S43] C++：智能指针
来源：http://xa.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://hc.nicolike.cn

[S44] C++：引用传参
来源：http://uh.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ho.shxzskj.cn

[S45] C++：lambda
来源：http://ou.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mi.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://da.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wz.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://do.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pe.hahajie.cn

[S48] C++：逐行读文件
来源：http://ta.shtwfgs.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zi.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://wb.chemitech.net.cn

[S49] C++：写文件
来源：http://hh.gzmigu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kt.huixiangedu.cn

[S50] C++：格式化数字
来源：http://wc.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://do.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://be.szxytkj.cn

static_cast<double>(a) / b
来源：http://hn.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://kf.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://zr.colortex.cn

[S53] C++：移动语义
来源：http://bu.lnxyls.cn

std::vector<int> w = std::move(v);
来源：http://si.wgjwhj.cn

[S54] C++：异常处理
来源：http://hl.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vg.huanxung.cn

[S55] C++：结构化绑定
来源：http://st.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kf.colortex.cn

[S56] C++：optional
来源：http://uc.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jh.nicolike.cn

[S57] C++：编译期常量
来源：http://yn.bjjhwx.cn

constexpr int N = 10;
来源：http://uc.yuexingan06.cn

[S58] C++：命名空间
来源：http://ja.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://wo.huixiangedu.cn

[S59] C++：静态断言
来源：http://fu.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://em.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://kb.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tj.lnxyls.cn

================================================================================
来源：http://br.nszjky.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zy.shxzukj.cn

================================================================================
来源：http://bp.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://gl.nszjky.cn

println("Hello")
来源：http://tz.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://cb.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://if.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://mh.muxihuayi.cn

"值: $b"
来源：http://cc.nicolike.cn

[T04] Kotlin：空安全
来源：http://ip.szsharing.cn

val n: String? = null;  n?.length
来源：http://pb.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://fa.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sp.9csxet.cn

[T06] Kotlin：集合映射
来源：http://qt.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://td.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://nn.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ym.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://bj.asd995.cn

data class User(val name: String, val age: Int)
来源：http://po.asd995.cn

[T09] Kotlin：扩展函数
来源：http://jq.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://tx.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://hm.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qz.yuexingan06.cn

[T11] Kotlin：协程
来源：http://os.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pf.nszjky.cn

[T12] Kotlin：解构声明
来源：http://fl.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://du.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://aw.9csxet.cn

val m = mapOf("a" to 1)
来源：http://py.wgjwhj.cn

[T14] Kotlin：循环
来源：http://vz.colortex.cn

for (i in 1..10) println(i)
来源：http://bg.shtwfgs.cn

[T15] Kotlin：接口
来源：http://gv.huanxung.cn

interface Shape { fun area(): Double }
来源：http://hm.szxytkj.cn

[T16] Swift：Hello World
来源：http://ok.newstarts.cn

print("Hello")
来源：http://pv.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://zq.yuexingan06.cn

var a = 1;  let b = 2
来源：http://bp.shxzukj.cn

[T18] Swift：字符串插值
来源：http://ud.9csxet.cn

"值: \(b)"
来源：http://kr.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://qq.szxytkj.cn

if let n = opt { print(n) }
来源：http://eh.hahajie.cn

[T20] Swift：数组操作
来源：http://yi.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://or.yuexingan06.cn

[T21] Swift：遍历
来源：http://pu.jianghongdianzi.cn

for x in a { print(x) }
来源：http://zp.lnxyls.cn

[T22] Swift：字典
来源：http://lb.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fc.lnxyls.cn

[T23] Swift：函数
来源：http://xb.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rd.shtwfgs.cn

[T24] Swift：闭包
来源：http://dx.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pf.bjjhwx.cn

[T25] Swift：结构体
来源：http://im.chemitech.net.cn

struct P { var x: Int }
来源：http://on.bjjhwx.cn

[T26] Swift：类与重写
来源：http://mq.colortex.cn

class A: Base { override func f() {} }
来源：http://wb.lnxyls.cn

[T27] Swift：错误处理
来源：http://rj.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://sf.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://mn.shxzskj.cn

enum Color { case red, green }
来源：http://pt.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://vi.hnjuh.cn

guard let x = opt else { return }
来源：http://re.panjiajie.cn

[T30] Swift：协议
来源：http://so.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://df.nicolike.cn

[T31] Lua：Hello World
来源：http://jh.hnjuh.cn

print("Hello")
来源：http://ph.muxihuayi.cn

[T32] Lua：局部变量
来源：http://op.huixinmuqiang.cn

local a = 1
来源：http://df.shxzskj.cn

[T33] Lua：表（数组）
来源：http://yk.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sk.hahajie.cn

[T34] Lua：遍历表
来源：http://vi.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fe.yuntaijiaju.cn

[T35] Lua：字典表
来源：http://vd.shtwfgs.cn

local d = { a = 1 };  d.b = 2
来源：http://lt.huixiangedu.cn

[T36] Lua：函数
来源：http://kd.newstarts.cn

function add(a, b) return a + b end
来源：http://jf.szsharing.cn

[T37] Lua：字符串拼接
来源：http://bc.chemitech.net.cn

"a" .. "b"
来源：http://gi.shtwfgs.cn

[T38] Lua：条件
来源：http://xu.haigaiapp.cn

if x > 0 then print("正") end
来源：http://zp.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://bh.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://ja.wgjwhj.cn

[T40] Lua：元表
来源：http://vd.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://az.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://zd.yuexingan06.cn

print "Hello\n";
来源：http://an.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://fd.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fi.nicolike.cn

[T43] Perl：字符串插值
来源：http://ye.newstarts.cn

"值: $a"
来源：http://kp.muxihuayi.cn

[T44] Perl：条件
来源：http://va.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://cl.panjiajie.cn

[T45] Perl：数组遍历
来源：http://fu.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://bj.huanxung.cn

[T46] Perl：哈希操作
来源：http://om.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aj.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://tx.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sm.yuexingan06.cn

[T48] Perl：正则替换
来源：http://rj.shxzukj.cn

$s =~ s/old/new/g;
来源：http://ml.9csxet.cn

[T49] Perl：函数
来源：http://to.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zq.szsharing.cn

[T50] Perl：逐行读文件
来源：http://by.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vy.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://yr.haigaiapp.cn

[T51] Scala：Hello World
来源：http://di.gzmigu.cn

println("Hello")
来源：http://kg.bjjhwx.cn

[T52] Scala：变量
来源：http://ze.muxihuayi.cn

val a = 1;  var b = 2
来源：http://hr.gzmigu.cn

[T53] Scala：字符串插值
来源：http://aj.jctech888.com.cn

s"值: $b"
来源：http://od.shxzukj.cn

[T54] Scala：集合映射
来源：http://oa.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://kn.hnjuh.cn

[T55] Scala：集合过滤
来源：http://vc.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xl.9csxet.cn

[T56] Scala：样例类
来源：http://zv.asd995.cn

case class User(name: String, age: Int)
来源：http://ga.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://xa.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nd.bjjhwx.cn

[T58] Scala：函数定义
来源：http://lx.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qr.newstarts.cn

[T59] Scala：循环
来源：http://lr.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://bt.muxihuayi.cn

[T60] Scala：折叠
来源：http://ak.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ei.shtwfgs.cn

================================================================================
来源：http://qv.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bl.hahajie.cn

================================================================================
来源：http://si.asd995.cn

[U01] Py：创建虚拟环境
来源：http://vq.bookmarksfly.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dz.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://lm.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://su.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://pi.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eq.521024.cn

[U04] Py：变量调试打印
来源：http://ue.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ml.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://gg.newstarts.cn

list(dict.fromkeys(arr))
来源：http://rd.nszjky.cn

[U06] Py：合并两个字典
来源：http://fw.newstarts.cn

{**a, **b}
来源：http://jn.lnxyls.cn

[U07] Py：反转字典键值
来源：http://sc.newstarts.cn

{v: k for k, v in d.items()}
来源：http://sl.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://ue.jctech888.com.cn

[y for x in nested for y in x]
来源：http://oy.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://hm.bookmarksfly.cn

max(d, key=d.get)
来源：http://tb.newstarts.cn

[U10] Py：按值排序字典
来源：http://wc.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nn.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://uo.chemitech.net.cn

(x * 2 for x in arr)
来源：http://zu.huixiangedu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://az.521024.cn

Counter(arr).most_common(3)
来源：http://ff.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://jw.wgjwhj.cn

deque(maxlen=10)
来源：http://mr.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://vv.lnxyls.cn

defaultdict(list)
来源：http://df.asd995.cn

[U15] Py：高精度计时
来源：http://vm.huixinmuqiang.cn

t = time.perf_counter()
来源：http://pw.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://ck.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yb.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://pg.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ld.panjiajie.cn

[U18] Py：预编译正则
来源：http://zf.521024.cn

pat = re.compile(r"\d+")
来源：http://yn.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://kl.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://si.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://cm.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://cr.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://to.hahajie.cn

@contextlib.contextmanager
来源：http://ek.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://bp.huanxung.cn

list(zip(*m))
来源：http://rr.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://te.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pa.panjiajie.cn

[U24] Py：路径操作
来源：http://ed.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wy.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://ag.szxytkj.cn

csv.DictReader(f)
来源：http://ar.wgjwhj.cn

[U26] Py：并发下载
来源：http://lx.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ew.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://cp.nicolike.cn

aiohttp.ClientSession() 配合 async with
来源：http://fx.bjjhwx.cn

[U28] Py：类型别名
来源：http://aw.nicolike.cn

UserId = int
来源：http://tw.gzmigu.cn

[U29] Py：属性校验
来源：http://ro.9csxet.cn

@property 与 @x.setter 配合
来源：http://ly.nicolike.cn

[U30] Py：数据类
来源：http://kz.521024.cn

@dataclass(slots=True)
来源：http://zl.hnjuh.cn

[U31] Py：单测
来源：http://ow.szxytkj.cn

python -m pytest -q
来源：http://ri.wgjwhj.cn

[U32] Py：代码格式化
来源：http://bk.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ms.huixiangedu.cn

[U33] Py：打包发布
来源：http://rv.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://fu.colortex.cn

[U34] Py：判断编码
来源：http://mt.jianghongdianzi.cn

chardet.detect(raw)
来源：http://qb.panjiajie.cn


<!-- 参考信息 -->