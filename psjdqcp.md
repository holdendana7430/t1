代发 wailian999

int main(int argc, char **argv)
来源：http://ke.haigaiapp.cn

[S19] C：快速排序
来源：http://gz.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bx.wgjwhj.cn

[S20] C：二分查找
来源：http://ey.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xf.szxytkj.cn

[S21] C：字符类别判断
来源：http://fg.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kv.panjiajie.cn

[S22] C：字符串转数字
来源：http://mi.bookmarksfly.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bd.szsharing.cn

[S23] C：随机数
来源：http://ff.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cx.huixiangedu.cn

[S24] C：获取本地时间
来源：http://wj.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ln.colortex.cn

[S25] C：内存拷贝
来源：http://gw.521024.cn

memcpy(dst, src, n);
来源：http://pw.hnjuh.cn

[S26] C：内存清零
来源：http://ik.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://km.bjjhwx.cn

[S27] C：定义常量
来源：http://pe.nicolike.cn

const double PI = 3.14159;
来源：http://ah.chemitech.net.cn

[S28] C：静态变量
来源：http://lg.shxzukj.cn

static int counter = 0;
来源：http://mi.jianghongdianzi.cn

[S29] C：变参函数
来源：http://yr.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rw.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ij.nicolike.cn

#ifndef X_H
来源：http://zy.chemitech.net.cn

#define X_H
来源：http://lf.shtwfgs.cn

#endif
来源：http://lm.asd995.cn

[S31] C++：Hello World
来源：http://ob.huixinmuqiang.cn

#include <iostream>
来源：http://yx.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://ur.jctech888.com.cn

[S32] C++：字符串
来源：http://jp.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://gx.panjiajie.cn

[S33] C++：vector 增删
来源：http://lu.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tw.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://vs.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://qp.szsharing.cn

[S35] C++：map
来源：http://ni.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jl.yuexingan06.cn

[S36] C++：unordered_map
来源：http://uj.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tc.bjjhwx.cn

[S37] C++：set
来源：http://cb.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yz.huanxung.cn

[S38] C++：排序
来源：http://lp.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://gf.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://nr.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ux.huanxung.cn

[S40] C++：查找元素
来源：http://nr.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tp.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://vw.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kd.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://td.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://fj.shxzskj.cn

[S43] C++：智能指针
来源：http://sc.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://vx.bjjhwx.cn

[S44] C++：引用传参
来源：http://nn.hahajie.cn

void inc(int &x) { ++x; }
来源：http://jp.asd995.cn

[S45] C++：lambda
来源：http://hn.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tr.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://dn.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pz.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://cm.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tl.nszjky.cn

[S48] C++：逐行读文件
来源：http://no.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rm.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://ou.huixiangedu.cn

[S49] C++：写文件
来源：http://jh.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tc.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://zc.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vn.shxzukj.cn

[S51] C++：显式类型转换
来源：http://fd.9csxet.cn

static_cast<double>(a) / b
来源：http://se.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://bj.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://go.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ii.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://oo.szsharing.cn

[S54] C++：异常处理
来源：http://qs.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sn.shxzukj.cn

[S55] C++：结构化绑定
来源：http://cf.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gv.jianghongdianzi.cn

[S56] C++：optional
来源：http://ac.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qi.asd995.cn

[S57] C++：编译期常量
来源：http://ve.szxytkj.cn

constexpr int N = 10;
来源：http://ke.shxzukj.cn

[S58] C++：命名空间
来源：http://ch.huixiangedu.cn

namespace ns { int f() { return 1; } }
来源：http://oq.gzmigu.cn

[S59] C++：静态断言
来源：http://li.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oq.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://nn.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ao.jianghongdianzi.cn

================================================================================
来源：http://mr.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cn.hnjuh.cn

================================================================================
来源：http://fb.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://dy.yuntaijiaju.cn

println("Hello")
来源：http://nv.wgjwhj.cn

[T02] Kotlin：变量
来源：http://hz.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dc.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://uf.panjiajie.cn

"值: $b"
来源：http://ga.huanxung.cn

[T04] Kotlin：空安全
来源：http://lx.gzmigu.cn

val n: String? = null;  n?.length
来源：http://kx.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://cq.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kv.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://kb.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qw.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://jg.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qj.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://zr.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://oy.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://pl.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://is.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://wq.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tz.huixiangedu.cn

[T11] Kotlin：协程
来源：http://hp.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xu.newstarts.cn

[T12] Kotlin：解构声明
来源：http://pt.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://hf.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://ug.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://yz.9csxet.cn

[T14] Kotlin：循环
来源：http://yd.asd995.cn

for (i in 1..10) println(i)
来源：http://kl.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://vq.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://gx.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://rn.nszjky.cn

print("Hello")
来源：http://ia.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://on.szxytkj.cn

var a = 1;  let b = 2
来源：http://vm.szsharing.cn

[T18] Swift：字符串插值
来源：http://mi.gzmigu.cn

"值: \(b)"
来源：http://sn.9csxet.cn

[T19] Swift：可选绑定
来源：http://ei.hahajie.cn

if let n = opt { print(n) }
来源：http://bo.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://ds.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hs.haigaiapp.cn

[T21] Swift：遍历
来源：http://bn.chemitech.net.cn

for x in a { print(x) }
来源：http://cu.huixinmuqiang.cn

[T22] Swift：字典
来源：http://ru.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fs.szxytkj.cn

[T23] Swift：函数
来源：http://tw.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ld.gzmigu.cn

[T24] Swift：闭包
来源：http://ha.yuntaijiaju.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bb.gzmigu.cn

[T25] Swift：结构体
来源：http://js.huanxung.cn

struct P { var x: Int }
来源：http://uc.huanxung.cn

[T26] Swift：类与重写
来源：http://jv.szxytkj.cn

class A: Base { override func f() {} }
来源：http://ba.lnxyls.cn

[T27] Swift：错误处理
来源：http://fc.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://pe.huixiangedu.cn

[T28] Swift：枚举
来源：http://uk.9csxet.cn

enum Color { case red, green }
来源：http://qy.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://qd.muxihuayi.cn

guard let x = opt else { return }
来源：http://lo.huanxung.cn

[T30] Swift：协议
来源：http://uh.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://bw.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://gd.hnjuh.cn

print("Hello")
来源：http://qq.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://fo.hnjuh.cn

local a = 1
来源：http://ca.hnjuh.cn

[T33] Lua：表（数组）
来源：http://po.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vk.szsharing.cn

[T34] Lua：遍历表
来源：http://dc.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cs.colortex.cn

[T35] Lua：字典表
来源：http://wb.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://tl.jctech888.com.cn

[T36] Lua：函数
来源：http://rf.hnjuh.cn

function add(a, b) return a + b end
来源：http://aj.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://hy.colortex.cn

"a" .. "b"
来源：http://oa.huixiangedu.cn

[T38] Lua：条件
来源：http://qy.shxzukj.cn

if x > 0 then print("正") end
来源：http://py.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://uj.521024.cn

string.find(s, "%d+")
来源：http://fl.nicolike.cn

[T40] Lua：元表
来源：http://tl.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://ku.asd995.cn

[T41] Perl：Hello World
来源：http://co.gzmigu.cn

print "Hello\n";
来源：http://vt.shxzskj.cn

[T42] Perl：变量类型
来源：http://eq.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yl.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://ky.wgjwhj.cn

"值: $a"
来源：http://lp.jctech888.com.cn

[T44] Perl：条件
来源：http://zi.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://hp.lnxyls.cn

[T45] Perl：数组遍历
来源：http://tg.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://vu.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ze.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gu.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://wm.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gf.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://ud.lnxyls.cn

$s =~ s/old/new/g;
来源：http://uj.yuntaijiaju.cn

[T49] Perl：函数
来源：http://xz.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ms.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://tu.shxzukj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mv.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://du.hahajie.cn

[T51] Scala：Hello World
来源：http://vx.huanxung.cn

println("Hello")
来源：http://ro.hnjuh.cn

[T52] Scala：变量
来源：http://jx.gzmigu.cn

val a = 1;  var b = 2
来源：http://xl.newstarts.cn

[T53] Scala：字符串插值
来源：http://hd.nszjky.cn

s"值: $b"
来源：http://yw.panjiajie.cn

[T54] Scala：集合映射
来源：http://xj.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://ai.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://vu.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ex.asd995.cn

[T56] Scala：样例类
来源：http://ag.hnjuh.cn

case class User(name: String, age: Int)
来源：http://ck.shxzukj.cn

[T57] Scala：模式匹配
来源：http://yg.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://om.yuexingan06.cn

[T58] Scala：函数定义
来源：http://qv.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gr.haigaiapp.cn

[T59] Scala：循环
来源：http://qc.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://om.gzmigu.cn

[T60] Scala：折叠
来源：http://yb.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ce.hahajie.cn

================================================================================
来源：http://dy.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ve.huixinmuqiang.cn

================================================================================
来源：http://ef.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://of.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gq.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://wa.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fu.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://gv.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eh.szxytkj.cn

[U04] Py：变量调试打印
来源：http://bn.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dz.asd995.cn

[U05] Py：列表去重且保序
来源：http://yj.haigaiapp.cn

list(dict.fromkeys(arr))
来源：http://kq.nicolike.cn

[U06] Py：合并两个字典
来源：http://mo.yuntaijiaju.cn

{**a, **b}
来源：http://wr.nicolike.cn

[U07] Py：反转字典键值
来源：http://zo.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://rl.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://tc.colortex.cn

[y for x in nested for y in x]
来源：http://gu.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://jl.szsharing.cn

max(d, key=d.get)
来源：http://dp.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://ju.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jp.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://im.nszjky.cn

(x * 2 for x in arr)
来源：http://xj.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kc.nszjky.cn

Counter(arr).most_common(3)
来源：http://xw.haigaiapp.cn

[U13] Py：固定长度队列
来源：http://ro.hnjuh.cn

deque(maxlen=10)
来源：http://ka.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://mc.szxytkj.cn

defaultdict(list)
来源：http://pn.nicolike.cn

[U15] Py：高精度计时
来源：http://xj.huixinmuqiang.cn

t = time.perf_counter()
来源：http://jn.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://tj.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oz.shxzskj.cn

[U17] Py：初始化日志
来源：http://fr.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ta.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://xg.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://la.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://jx.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qk.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://ph.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://qb.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://ry.asd995.cn

@contextlib.contextmanager
来源：http://eb.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://lj.bjjhwx.cn

list(zip(*m))
来源：http://vx.colortex.cn

[U23] Py：分块读取大文件
来源：http://ut.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://un.shxzukj.cn

[U24] Py：路径操作
来源：http://fp.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ay.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://he.bjjhwx.cn

csv.DictReader(f)
来源：http://pu.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://av.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nb.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://nj.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://eo.hahajie.cn

[U28] Py：类型别名
来源：http://dy.gzmigu.cn

UserId = int
来源：http://ur.wgjwhj.cn

[U29] Py：属性校验
来源：http://op.haigaiapp.cn

@property 与 @x.setter 配合
来源：http://jj.colortex.cn

[U30] Py：数据类
来源：http://go.haigaiapp.cn

@dataclass(slots=True)
来源：http://mp.nszjky.cn

[U31] Py：单测
来源：http://ns.asd995.cn

python -m pytest -q
来源：http://al.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://cb.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://id.nicolike.cn

[U33] Py：打包发布
来源：http://ly.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://ba.hahajie.cn

[U34] Py：判断编码
来源：http://cb.asd995.cn

chardet.detect(raw)
来源：http://qv.shxzskj.cn

[U35] Py：发送邮件
来源：http://vo.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hc.panjiajie.cn

[U36] Py：定时任务
来源：http://yv.szsharing.cn

schedule.every(10).minutes.do(job)
来源：http://vh.szxytkj.cn

[U37] Py：读写 Excel
来源：http://jz.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tv.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://bx.9csxet.cn

Path(__file__).resolve().parent
来源：http://oa.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://hx.shtwfgs.cn

sys.stdout.isatty()
来源：http://ji.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://zm.shxzukj.cn

print("err", file=sys.stderr)
来源：http://bm.huixinmuqiang.cn

[U41] PHP：初始化 Composer 项目
来源：http://lc.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yz.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://qe.gzmigu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ow.nicolike.cn


<!-- 参考信息 -->