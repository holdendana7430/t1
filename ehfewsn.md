代发 wailian999

int main(int argc, char **argv)
来源：http://nh.521024.cn

[S19] C：快速排序
来源：http://hr.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qe.hahajie.cn

[S20] C：二分查找
来源：http://fl.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hk.haigaiapp.cn

[S21] C：字符类别判断
来源：http://lt.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ek.muxihuayi.cn

[S22] C：字符串转数字
来源：http://pr.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xl.9csxet.cn

[S23] C：随机数
来源：http://hy.shxzukj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pr.nszjky.cn

[S24] C：获取本地时间
来源：http://wv.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mn.521024.cn

[S25] C：内存拷贝
来源：http://wu.muxihuayi.cn

memcpy(dst, src, n);
来源：http://gd.newstarts.cn

[S26] C：内存清零
来源：http://xn.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://og.shxzskj.cn

[S27] C：定义常量
来源：http://qp.huixiangedu.cn

const double PI = 3.14159;
来源：http://pp.panjiajie.cn

[S28] C：静态变量
来源：http://wv.newstarts.cn

static int counter = 0;
来源：http://bg.newstarts.cn

[S29] C：变参函数
来源：http://ba.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oc.nicolike.cn

[S30] C：头文件保护
来源：http://qy.9csxet.cn

#ifndef X_H
来源：http://fc.yuntaijiaju.cn

#define X_H
来源：http://rz.wgjwhj.cn

#endif
来源：http://xr.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://rl.asd995.cn

#include <iostream>
来源：http://ao.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://bc.bookmarksfly.cn

[S32] C++：字符串
来源：http://pr.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://lh.hahajie.cn

[S33] C++：vector 增删
来源：http://wp.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fb.521024.cn

[S34] C++：遍历 vector
来源：http://nx.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://kr.shtwfgs.cn

[S35] C++：map
来源：http://pg.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wh.asd995.cn

[S36] C++：unordered_map
来源：http://qd.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ak.shtwfgs.cn

[S37] C++：set
来源：http://xw.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ck.muxihuayi.cn

[S38] C++：排序
来源：http://fe.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://ys.huanxung.cn

[S39] C++：自定义比较器排序
来源：http://jr.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ne.shtwfgs.cn

[S40] C++：查找元素
来源：http://hh.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qf.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://dl.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qx.chemitech.net.cn

[S42] C++：继承与虚函数
来源：http://wj.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://bw.szsharing.cn

[S43] C++：智能指针
来源：http://mn.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://wg.jctech888.com.cn

[S44] C++：引用传参
来源：http://tj.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://bq.huanxung.cn

[S45] C++：lambda
来源：http://hs.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fe.shxzskj.cn

[S46] C++：函数模板
来源：http://gg.asd995.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vw.yuntaijiaju.cn

[S47] C++：结构化绑定遍历
来源：http://hx.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ak.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://lr.newstarts.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eo.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://vw.gzmigu.cn

[S49] C++：写文件
来源：http://yd.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cv.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://mu.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yh.hahajie.cn

[S51] C++：显式类型转换
来源：http://bz.521024.cn

static_cast<double>(a) / b
来源：http://vv.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://lb.colortex.cn

int size() const noexcept { return n_; }
来源：http://be.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ne.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://og.shxzukj.cn

[S54] C++：异常处理
来源：http://qs.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bd.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://nk.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rq.lnxyls.cn

[S56] C++：optional
来源：http://ep.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qv.hnjuh.cn

[S57] C++：编译期常量
来源：http://is.szsharing.cn

constexpr int N = 10;
来源：http://fm.bookmarksfly.cn

[S58] C++：命名空间
来源：http://yb.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://mp.9csxet.cn

[S59] C++：静态断言
来源：http://cu.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gh.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://aq.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ne.colortex.cn

================================================================================
来源：http://fh.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ty.huanxung.cn

================================================================================
来源：http://dc.9csxet.cn

[T01] Kotlin：Hello World
来源：http://qh.huixinmuqiang.cn

println("Hello")
来源：http://jf.hnjuh.cn

[T02] Kotlin：变量
来源：http://hy.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sn.521024.cn

[T03] Kotlin：字符串模板
来源：http://hj.shxzukj.cn

"值: $b"
来源：http://uo.gzmigu.cn

[T04] Kotlin：空安全
来源：http://tn.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://vd.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://oh.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fh.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://rx.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cw.asd995.cn

[T07] Kotlin：集合过滤
来源：http://yq.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dx.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://mk.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://kv.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://zg.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://jn.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://oa.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.shxzskj.cn

[T11] Kotlin：协程
来源：http://st.9csxet.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://et.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://cn.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://oa.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://fx.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://tc.lnxyls.cn

[T14] Kotlin：循环
来源：http://wg.szsharing.cn

for (i in 1..10) println(i)
来源：http://uj.wgjwhj.cn

[T15] Kotlin：接口
来源：http://js.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://xi.shxzukj.cn

[T16] Swift：Hello World
来源：http://mr.shxzukj.cn

print("Hello")
来源：http://rt.shxzskj.cn

[T17] Swift：变量与常量
来源：http://tg.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://sr.shxzukj.cn

[T18] Swift：字符串插值
来源：http://li.newstarts.cn

"值: \(b)"
来源：http://zg.huanxung.cn

[T19] Swift：可选绑定
来源：http://zn.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ie.huixiangedu.cn

[T20] Swift：数组操作
来源：http://qq.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sw.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://cx.wgjwhj.cn

for x in a { print(x) }
来源：http://ii.newstarts.cn

[T22] Swift：字典
来源：http://rj.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kx.nicolike.cn

[T23] Swift：函数
来源：http://et.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mr.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://on.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kp.chemitech.net.cn

[T25] Swift：结构体
来源：http://gz.panjiajie.cn

struct P { var x: Int }
来源：http://kn.hahajie.cn

[T26] Swift：类与重写
来源：http://zv.jctech888.com.cn

class A: Base { override func f() {} }
来源：http://by.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://vy.nicolike.cn

do { try f() } catch { print(error) }
来源：http://od.wgjwhj.cn

[T28] Swift：枚举
来源：http://ib.shxzukj.cn

enum Color { case red, green }
来源：http://hg.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://ny.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://zq.shxzukj.cn

[T30] Swift：协议
来源：http://dx.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://vj.muxihuayi.cn

[T31] Lua：Hello World
来源：http://hd.hnjuh.cn

print("Hello")
来源：http://ln.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://do.szsharing.cn

local a = 1
来源：http://nt.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://fl.521024.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fx.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://qt.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zk.shxzskj.cn

[T35] Lua：字典表
来源：http://gp.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://cn.lnxyls.cn

[T36] Lua：函数
来源：http://uh.haigaiapp.cn

function add(a, b) return a + b end
来源：http://mp.colortex.cn

[T37] Lua：字符串拼接
来源：http://ph.huixiangedu.cn

"a" .. "b"
来源：http://pm.wgjwhj.cn

[T38] Lua：条件
来源：http://qz.panjiajie.cn

if x > 0 then print("正") end
来源：http://ou.gzmigu.cn

[T39] Lua：模式匹配
来源：http://ey.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://ni.panjiajie.cn

[T40] Lua：元表
来源：http://fk.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://ot.nicolike.cn

[T41] Perl：Hello World
来源：http://dw.panjiajie.cn

print "Hello\n";
来源：http://cw.hahajie.cn

[T42] Perl：变量类型
来源：http://mq.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bv.colortex.cn

[T43] Perl：字符串插值
来源：http://cg.521024.cn

"值: $a"
来源：http://li.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ys.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://ls.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://gx.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://dy.hnjuh.cn

[T46] Perl：哈希操作
来源：http://tt.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zf.521024.cn

[T47] Perl：正则捕获
来源：http://si.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cy.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://vi.chemitech.net.cn

$s =~ s/old/new/g;
来源：http://ua.521024.cn

[T49] Perl：函数
来源：http://ma.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://si.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://of.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lj.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://oh.panjiajie.cn

[T51] Scala：Hello World
来源：http://bd.hnjuh.cn

println("Hello")
来源：http://ed.nszjky.cn

[T52] Scala：变量
来源：http://au.chemitech.net.cn

val a = 1;  var b = 2
来源：http://kd.szsharing.cn

[T53] Scala：字符串插值
来源：http://ni.huanxung.cn

s"值: $b"
来源：http://se.lnxyls.cn

[T54] Scala：集合映射
来源：http://zc.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://ju.nicolike.cn

[T55] Scala：集合过滤
来源：http://fd.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ol.shxzukj.cn

[T56] Scala：样例类
来源：http://ck.shxzskj.cn

case class User(name: String, age: Int)
来源：http://zi.szxytkj.cn

[T57] Scala：模式匹配
来源：http://gj.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ho.yuexingan06.cn

[T58] Scala：函数定义
来源：http://ht.yuexingan06.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ii.muxihuayi.cn

[T59] Scala：循环
来源：http://az.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://qd.shxzukj.cn

[T60] Scala：折叠
来源：http://ch.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lw.yuexingan06.cn

================================================================================
来源：http://ee.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tk.jianghongdianzi.cn

================================================================================
来源：http://de.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://ra.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vc.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://cu.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ez.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://zl.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mz.bjjhwx.cn

[U04] Py：变量调试打印
来源：http://wk.yuexingan06.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eh.9csxet.cn

[U05] Py：列表去重且保序
来源：http://ih.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://bt.nszjky.cn

[U06] Py：合并两个字典
来源：http://yl.wgjwhj.cn

{**a, **b}
来源：http://nz.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://ic.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://ia.nicolike.cn

[U08] Py：展平二维列表
来源：http://bw.nszjky.cn

[y for x in nested for y in x]
来源：http://af.muxihuayi.cn

[U09] Py：字典取最大值的键
来源：http://xk.hnjuh.cn

max(d, key=d.get)
来源：http://vr.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://il.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wv.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ey.shtwfgs.cn

(x * 2 for x in arr)
来源：http://xt.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sj.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://py.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://jq.nszjky.cn

deque(maxlen=10)
来源：http://yt.asd995.cn

[U14] Py：分组收集到列表
来源：http://rl.shxzskj.cn

defaultdict(list)
来源：http://xd.shxzukj.cn

[U15] Py：高精度计时
来源：http://xt.szsharing.cn

t = time.perf_counter()
来源：http://mf.nicolike.cn

[U16] Py：命令行参数解析
来源：http://lt.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mr.521024.cn

[U17] Py：初始化日志
来源：http://oz.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ty.chemitech.net.cn

[U18] Py：预编译正则
来源：http://kp.wgjwhj.cn

pat = re.compile(r"\d+")
来源：http://ae.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://np.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xt.colortex.cn

[U20] Py：缓存函数结果
来源：http://zu.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://vy.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://qr.muxihuayi.cn

@contextlib.contextmanager
来源：http://td.gzmigu.cn

[U22] Py：矩阵转置
来源：http://tg.shxzukj.cn

list(zip(*m))
来源：http://ue.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://wt.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hs.chemitech.net.cn

[U24] Py：路径操作
来源：http://eq.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ei.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://oz.asd995.cn

csv.DictReader(f)
来源：http://ls.bjjhwx.cn

[U26] Py：并发下载
来源：http://os.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://da.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://nd.lnxyls.cn

aiohttp.ClientSession() 配合 async with
来源：http://lm.521024.cn

[U28] Py：类型别名
来源：http://js.nicolike.cn

UserId = int
来源：http://sw.szxytkj.cn

[U29] Py：属性校验
来源：http://tz.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://ix.huixinmuqiang.cn

[U30] Py：数据类
来源：http://ss.bookmarksfly.cn

@dataclass(slots=True)
来源：http://zg.szxytkj.cn

[U31] Py：单测
来源：http://qg.nszjky.cn

python -m pytest -q
来源：http://wh.lnxyls.cn

[U32] Py：代码格式化
来源：http://jc.nicolike.cn

ruff format . && ruff check --fix .
来源：http://ro.huanxung.cn

[U33] Py：打包发布
来源：http://qd.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://yc.nszjky.cn

[U34] Py：判断编码
来源：http://mv.shxzukj.cn

chardet.detect(raw)
来源：http://vq.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://ce.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zs.colortex.cn

[U36] Py：定时任务
来源：http://xh.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://pq.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://tu.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://za.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://zl.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://ku.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://oo.chemitech.net.cn

sys.stdout.isatty()
来源：http://sm.9csxet.cn

[U40] Py：打印到标准错误
来源：http://wb.newstarts.cn

print("err", file=sys.stderr)
来源：http://vm.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://hq.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fm.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://th.jianghongdianzi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hs.bookmarksfly.cn


<!-- 参考信息 -->